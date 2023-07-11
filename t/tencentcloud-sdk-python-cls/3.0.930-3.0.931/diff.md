# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.930.tar", last modified: Fri Jul  7 00:20:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.931.tar", last modified: Mon Jul 10 00:34:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.930.tar` & `tencentcloud-sdk-python-cls-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8715 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    73424 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)   438700 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:20:38.000000 tencentcloud-sdk-python-cls-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    77073 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)   460959 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:34:11.000000 tencentcloud-sdk-python-cls-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/setup.py` & `tencentcloud-sdk-python-cls-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.931/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.931/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/README.rst` & `tencentcloud-sdk-python-cls-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,26 +97,35 @@
 
 # 相同的采集配置规则已经存在。
 INVALIDPARAMETER_CONFIGCONFLICT = 'InvalidParameter.ConfigConflict'
 
 # 无效的Content。
 INVALIDPARAMETER_CONTENT = 'InvalidParameter.Content'
 
+# 数据加工任务冲突。
+INVALIDPARAMETER_DATAFROMTASKCONFLICT = 'InvalidParameter.DataFromTaskConflict'
+
+# 数据加工任务不存在。
+INVALIDPARAMETER_DATAFROMTASKNOTEXIST = 'InvalidParameter.DataFromTaskNotExist'
+
 # 数据库唯一键冲突。
 INVALIDPARAMETER_DBDUPLICATION = 'InvalidParameter.DbDuplication'
 
 # 导出任务已经存在。
 INVALIDPARAMETER_EXPORTCONFLICT = 'InvalidParameter.ExportConflict'
 
 # 低频不支持配置kv和tag索引。
 INVALIDPARAMETER_INVALIDINDEXRULEFORSEARCHLOW = 'InvalidParameter.InValidIndexRuleForSearchLow'
 
 # 指定日志主题已经存在索引规则。
 INVALIDPARAMETER_INDEXCONFLICT = 'InvalidParameter.IndexConflict'
 
+# 无效的数据加工语句。
+INVALIDPARAMETER_INVALIDETLCONTENT = 'InvalidParameter.InvalidEtlContent'
+
 # 相同的日志集已存在。
 INVALIDPARAMETER_LOGSETCONFLICT = 'InvalidParameter.LogsetConflict'
 
 # 同名机器组已经存在。
 INVALIDPARAMETER_MACHINEGROUPCONFLICT = 'InvalidParameter.MachineGroupConflict'
 
 # 投递规则命名冲突。
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateDataTransform(self, request):
+        """本接口用于创建数据加工任务。
+
+        :param request: Request instance for CreateDataTransform.
+        :type request: :class:`tencentcloud.cls.v20201016.models.CreateDataTransformRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.CreateDataTransformResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDataTransform", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDataTransformResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateExport(self, request):
         """本接口仅创建下载任务，任务返回的下载地址，请用户调用DescribeExports查看任务列表。其中有下载地址CosPath参数。参考文档https://cloud.tencent.com/document/product/614/56449
 
         :param request: Request instance for CreateExport.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateExportRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.CreateExportResponse`
 
@@ -551,14 +574,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteDataTransform(self, request):
+        """本接口用于删除数据加工任务
+
+        :param request: Request instance for DeleteDataTransform.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DeleteDataTransformRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteDataTransformResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteDataTransform", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteDataTransformResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteExport(self, request):
         """本接口用于删除日志下载任务
 
         :param request: Request instance for DeleteExport.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteExportRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteExportResponse`
 
@@ -919,14 +965,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDataTransformInfo(self, request):
+        """本接口用于获取数据加工任务列表基本信息
+
+        :param request: Request instance for DescribeDataTransformInfo.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DescribeDataTransformInfoRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeDataTransformInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataTransformInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataTransformInfoResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeExports(self, request):
         """本接口用于获取日志下载任务列表
 
         :param request: Request instance for DescribeExports.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeExportsRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeExportsResponse`
 
@@ -1400,14 +1469,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyDataTransform(self, request):
+        """本接口用于修改数据加工任务
+
+        :param request: Request instance for ModifyDataTransform.
+        :type request: :class:`tencentcloud.cls.v20201016.models.ModifyDataTransformRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.ModifyDataTransformResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDataTransform", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDataTransformResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyIndex(self, request):
         """本接口用于修改索引配置，该接口除受默认接口请求频率限制外，针对单个日志主题，并发数不能超过1，即同一时间同一个日志主题只能有一个正在执行的索引配置修改操作。
 
         :param request: Request instance for ModifyIndex.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyIndexRequest`
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.931/tencentcloud/cls/v20201016/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3662,14 +3662,178 @@
 
 
     def _deserialize(self, params):
         self._Id = params.get("Id")
         self._RequestId = params.get("RequestId")
 
 
+class CreateDataTransformRequest(AbstractModel):
+    """CreateDataTransform请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FuncType: 任务类型. 1: 指定主题；2:动态创建
+        :type FuncType: int
+        :param _SrcTopicId: 源日志主题
+        :type SrcTopicId: str
+        :param _Name: 加工任务名称
+        :type Name: str
+        :param _EtlContent: 加工语句
+        :type EtlContent: str
+        :param _TaskType: 加工类型  1 使用源日志主题中的随机数据，进行加工预览 :2 使用用户自定义测试数据，进行加工预览 3 创建真实加工任务
+        :type TaskType: int
+        :param _EnableFlag: 任务启动状态.   默认为1:开启,  2:关闭
+        :type EnableFlag: int
+        :param _DstResources: 加工任务目的topic_id以及别名
+        :type DstResources: list of DataTransformResouceInfo
+        :param _PreviewLogStatistics: 用于预览加工结果的测试数据
+        :type PreviewLogStatistics: list of PreviewLogStatistic
+        """
+        self._FuncType = None
+        self._SrcTopicId = None
+        self._Name = None
+        self._EtlContent = None
+        self._TaskType = None
+        self._EnableFlag = None
+        self._DstResources = None
+        self._PreviewLogStatistics = None
+
+    @property
+    def FuncType(self):
+        return self._FuncType
+
+    @FuncType.setter
+    def FuncType(self, FuncType):
+        self._FuncType = FuncType
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def EtlContent(self):
+        return self._EtlContent
+
+    @EtlContent.setter
+    def EtlContent(self, EtlContent):
+        self._EtlContent = EtlContent
+
+    @property
+    def TaskType(self):
+        return self._TaskType
+
+    @TaskType.setter
+    def TaskType(self, TaskType):
+        self._TaskType = TaskType
+
+    @property
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def DstResources(self):
+        return self._DstResources
+
+    @DstResources.setter
+    def DstResources(self, DstResources):
+        self._DstResources = DstResources
+
+    @property
+    def PreviewLogStatistics(self):
+        return self._PreviewLogStatistics
+
+    @PreviewLogStatistics.setter
+    def PreviewLogStatistics(self, PreviewLogStatistics):
+        self._PreviewLogStatistics = PreviewLogStatistics
+
+
+    def _deserialize(self, params):
+        self._FuncType = params.get("FuncType")
+        self._SrcTopicId = params.get("SrcTopicId")
+        self._Name = params.get("Name")
+        self._EtlContent = params.get("EtlContent")
+        self._TaskType = params.get("TaskType")
+        self._EnableFlag = params.get("EnableFlag")
+        if params.get("DstResources") is not None:
+            self._DstResources = []
+            for item in params.get("DstResources"):
+                obj = DataTransformResouceInfo()
+                obj._deserialize(item)
+                self._DstResources.append(obj)
+        if params.get("PreviewLogStatistics") is not None:
+            self._PreviewLogStatistics = []
+            for item in params.get("PreviewLogStatistics"):
+                obj = PreviewLogStatistic()
+                obj._deserialize(item)
+                self._PreviewLogStatistics.append(obj)
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
+class CreateDataTransformResponse(AbstractModel):
+    """CreateDataTransform返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务id
+        :type TaskId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TaskId = None
+        self._RequestId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
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
+        self._TaskId = params.get("TaskId")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateExportRequest(AbstractModel):
     """CreateExport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4865,14 +5029,241 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DataTransformResouceInfo(AbstractModel):
+    """数据加工的资源信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TopicId: 目标主题id
+        :type TopicId: str
+        :param _Alias: 别名
+        :type Alias: str
+        """
+        self._TopicId = None
+        self._Alias = None
+
+    @property
+    def TopicId(self):
+        return self._TopicId
+
+    @TopicId.setter
+    def TopicId(self, TopicId):
+        self._TopicId = TopicId
+
+    @property
+    def Alias(self):
+        return self._Alias
+
+    @Alias.setter
+    def Alias(self, Alias):
+        self._Alias = Alias
+
+
+    def _deserialize(self, params):
+        self._TopicId = params.get("TopicId")
+        self._Alias = params.get("Alias")
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
+class DataTransformTaskInfo(AbstractModel):
+    """数据加工任务基本详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 数据加工任务名称
+        :type Name: str
+        :param _TaskId: 数据加工任务id
+        :type TaskId: str
+        :param _EnableFlag: 任务启用状态，默认为1，正常开启,  2关闭
+        :type EnableFlag: int
+        :param _Type: 加工任务类型，1： DSL， 2：SQL
+        :type Type: int
+        :param _SrcTopicId: 源日志主题
+        :type SrcTopicId: str
+        :param _Status: 当前加工任务状态（1准备中/2运行中/3停止中/4已停止）
+        :type Status: int
+        :param _CreateTime: 加工任务创建时间
+        :type CreateTime: str
+        :param _UpdateTime: 最近修改时间
+        :type UpdateTime: str
+        :param _LastEnableTime: 最后启用时间，如果需要重建集群，修改该时间
+        :type LastEnableTime: str
+        :param _SrcTopicName: 日志主题名称
+        :type SrcTopicName: str
+        :param _LogsetId: 日志集id
+        :type LogsetId: str
+        :param _DstResources: 加工任务目的topic_id以及别名
+        :type DstResources: list of DataTransformResouceInfo
+        :param _EtlContent: 加工逻辑函数
+        :type EtlContent: str
+        """
+        self._Name = None
+        self._TaskId = None
+        self._EnableFlag = None
+        self._Type = None
+        self._SrcTopicId = None
+        self._Status = None
+        self._CreateTime = None
+        self._UpdateTime = None
+        self._LastEnableTime = None
+        self._SrcTopicName = None
+        self._LogsetId = None
+        self._DstResources = None
+        self._EtlContent = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def LastEnableTime(self):
+        return self._LastEnableTime
+
+    @LastEnableTime.setter
+    def LastEnableTime(self, LastEnableTime):
+        self._LastEnableTime = LastEnableTime
+
+    @property
+    def SrcTopicName(self):
+        return self._SrcTopicName
+
+    @SrcTopicName.setter
+    def SrcTopicName(self, SrcTopicName):
+        self._SrcTopicName = SrcTopicName
+
+    @property
+    def LogsetId(self):
+        return self._LogsetId
+
+    @LogsetId.setter
+    def LogsetId(self, LogsetId):
+        self._LogsetId = LogsetId
+
+    @property
+    def DstResources(self):
+        return self._DstResources
+
+    @DstResources.setter
+    def DstResources(self, DstResources):
+        self._DstResources = DstResources
+
+    @property
+    def EtlContent(self):
+        return self._EtlContent
+
+    @EtlContent.setter
+    def EtlContent(self, EtlContent):
+        self._EtlContent = EtlContent
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._TaskId = params.get("TaskId")
+        self._EnableFlag = params.get("EnableFlag")
+        self._Type = params.get("Type")
+        self._SrcTopicId = params.get("SrcTopicId")
+        self._Status = params.get("Status")
+        self._CreateTime = params.get("CreateTime")
+        self._UpdateTime = params.get("UpdateTime")
+        self._LastEnableTime = params.get("LastEnableTime")
+        self._SrcTopicName = params.get("SrcTopicName")
+        self._LogsetId = params.get("LogsetId")
+        if params.get("DstResources") is not None:
+            self._DstResources = []
+            for item in params.get("DstResources"):
+                obj = DataTransformResouceInfo()
+                obj._deserialize(item)
+                self._DstResources.append(obj)
+        self._EtlContent = params.get("EtlContent")
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
 class DeleteAlarmNoticeRequest(AbstractModel):
     """DeleteAlarmNotice请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5225,14 +5616,72 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteDataTransformRequest(AbstractModel):
+    """DeleteDataTransform请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 数据加工任务id
+        :type TaskId: str
+        """
+        self._TaskId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
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
+class DeleteDataTransformResponse(AbstractModel):
+    """DeleteDataTransform返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteExportRequest(AbstractModel):
     """DeleteExport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6681,14 +7130,175 @@
             for item in params.get("Data"):
                 obj = CosRechargeInfo()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDataTransformInfoRequest(AbstractModel):
+    """DescribeDataTransformInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Filters: <br><li> taskName
+
+按照【加工任务名称】进行过滤。
+类型：String
+
+必选：否
+
+<br><li> taskId
+
+按照【加工任务id】进行过滤。
+类型：String
+
+必选：否
+
+<br><li> srctopicId
+
+按照【源topicId】进行过滤。
+类型：String
+
+必选：否
+
+每次请求的Filters的上限为10，Filter.Values的上限为100。
+        :type Filters: list of Filter
+        :param _Offset: 分页的偏移量，默认值为0。
+        :type Offset: int
+        :param _Limit: 分页单页限制数目，默认值为20，最大值100。
+        :type Limit: int
+        :param _Type: 默认值为2.   1: 获取单个任务的详细信息 2：获取任务列表
+        :type Type: int
+        :param _TaskId: Type为1， 此参数必填
+        :type TaskId: str
+        """
+        self._Filters = None
+        self._Offset = None
+        self._Limit = None
+        self._Type = None
+        self._TaskId = None
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._Type = params.get("Type")
+        self._TaskId = params.get("TaskId")
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
+class DescribeDataTransformInfoResponse(AbstractModel):
+    """DescribeDataTransformInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DataTransformTaskInfos: 数据加工任务列表信息
+        :type DataTransformTaskInfos: list of DataTransformTaskInfo
+        :param _TotalCount: 任务总次数
+        :type TotalCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DataTransformTaskInfos = None
+        self._TotalCount = None
+        self._RequestId = None
+
+    @property
+    def DataTransformTaskInfos(self):
+        return self._DataTransformTaskInfos
+
+    @DataTransformTaskInfos.setter
+    def DataTransformTaskInfos(self, DataTransformTaskInfos):
+        self._DataTransformTaskInfos = DataTransformTaskInfos
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
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
+        if params.get("DataTransformTaskInfos") is not None:
+            self._DataTransformTaskInfos = []
+            for item in params.get("DataTransformTaskInfos"):
+                obj = DataTransformTaskInfo()
+                obj._deserialize(item)
+                self._DataTransformTaskInfos.append(obj)
+        self._TotalCount = params.get("TotalCount")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeExportsRequest(AbstractModel):
     """DescribeExports请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11994,14 +12604,125 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyDataTransformRequest(AbstractModel):
+    """ModifyDataTransform请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 加工任务id
+        :type TaskId: str
+        :param _Name: 加工任务名称
+        :type Name: str
+        :param _EtlContent: 加工语句
+        :type EtlContent: str
+        :param _EnableFlag: 任务启动状态. 默认为1，开启,  2关闭
+        :type EnableFlag: int
+        :param _DstResources: 加工任务目的topic_id以及别名
+        :type DstResources: list of DataTransformResouceInfo
+        """
+        self._TaskId = None
+        self._Name = None
+        self._EtlContent = None
+        self._EnableFlag = None
+        self._DstResources = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def EtlContent(self):
+        return self._EtlContent
+
+    @EtlContent.setter
+    def EtlContent(self, EtlContent):
+        self._EtlContent = EtlContent
+
+    @property
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def DstResources(self):
+        return self._DstResources
+
+    @DstResources.setter
+    def DstResources(self, DstResources):
+        self._DstResources = DstResources
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._Name = params.get("Name")
+        self._EtlContent = params.get("EtlContent")
+        self._EnableFlag = params.get("EnableFlag")
+        if params.get("DstResources") is not None:
+            self._DstResources = []
+            for item in params.get("DstResources"):
+                obj = DataTransformResouceInfo()
+                obj._deserialize(item)
+                self._DstResources.append(obj)
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
+class ModifyDataTransformResponse(AbstractModel):
+    """ModifyDataTransform返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyIndexRequest(AbstractModel):
     """ModifyIndex请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13598,14 +14319,108 @@
 
     def _deserialize(self, params):
         self._LogSample = params.get("LogSample")
         self._LogData = params.get("LogData")
         self._RequestId = params.get("RequestId")
 
 
+class PreviewLogStatistic(AbstractModel):
+    """预览数据详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _LogContent: 日志内容
+        :type LogContent: str
+        :param _LineNum: 行号
+        :type LineNum: int
+        :param _DstTopicId: 目标日志主题
+        :type DstTopicId: str
+        :param _FailReason: 失败错误码， 空字符串""表示正常
+        :type FailReason: str
+        :param _Time: 日志时间戳
+        :type Time: str
+        :param _DstTopicName: 目标topic-name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DstTopicName: str
+        """
+        self._LogContent = None
+        self._LineNum = None
+        self._DstTopicId = None
+        self._FailReason = None
+        self._Time = None
+        self._DstTopicName = None
+
+    @property
+    def LogContent(self):
+        return self._LogContent
+
+    @LogContent.setter
+    def LogContent(self, LogContent):
+        self._LogContent = LogContent
+
+    @property
+    def LineNum(self):
+        return self._LineNum
+
+    @LineNum.setter
+    def LineNum(self, LineNum):
+        self._LineNum = LineNum
+
+    @property
+    def DstTopicId(self):
+        return self._DstTopicId
+
+    @DstTopicId.setter
+    def DstTopicId(self, DstTopicId):
+        self._DstTopicId = DstTopicId
+
+    @property
+    def FailReason(self):
+        return self._FailReason
+
+    @FailReason.setter
+    def FailReason(self, FailReason):
+        self._FailReason = FailReason
+
+    @property
+    def Time(self):
+        return self._Time
+
+    @Time.setter
+    def Time(self, Time):
+        self._Time = Time
+
+    @property
+    def DstTopicName(self):
+        return self._DstTopicName
+
+    @DstTopicName.setter
+    def DstTopicName(self, DstTopicName):
+        self._DstTopicName = DstTopicName
+
+
+    def _deserialize(self, params):
+        self._LogContent = params.get("LogContent")
+        self._LineNum = params.get("LineNum")
+        self._DstTopicId = params.get("DstTopicId")
+        self._FailReason = params.get("FailReason")
+        self._Time = params.get("Time")
+        self._DstTopicName = params.get("DstTopicName")
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
 class RetryShipperTaskRequest(AbstractModel):
     """RetryShipperTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cls-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.931/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.930'
+__version__ = '3.0.931'
```

