# Comparing `tmp/tencentcloud-sdk-python-cms-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-cms-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.931.tar", last modified: Mon Jul 10 00:34:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.932.tar", last modified: Tue Jul 11 00:37:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cms-3.0.931.tar` & `tencentcloud-sdk-python-cms-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/
--rw-r--r--   0 root         (0) root         (0)     4152 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/cms_client.py
--rw-r--r--   0 root         (0) root         (0)    96019 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:34:31.000000 tencentcloud-sdk-python-cms-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6573 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/cms_client.py
+-rw-r--r--   0 root         (0) root         (0)    97349 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:37:10.000000 tencentcloud-sdk-python-cms-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cms-3.0.931/setup.py` & `tencentcloud-sdk-python-cms-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.931/tencentcloud_sdk_python_cms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.932/tencentcloud_sdk_python_cms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.931/README.rst` & `tencentcloud-sdk-python-cms-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/errorcodes.py` & `tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/cms_client.py` & `tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/cms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.931/tencentcloud/cms/v20190321/models.py` & `tencentcloud-sdk-python-cms-3.0.932/tencentcloud/cms/v20190321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,37 +381,48 @@
     """
 
     def __init__(self):
         r"""
         :param _SampleIDs: 添加成功的关键词ID列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type SampleIDs: list of str
+        :param _SuccessInfos: 成功入库关键词列表
+        :type SuccessInfos: list of UserKeywordInfo
         :param _DupInfos: 重复关键词列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type DupInfos: list of UserKeywordInfo
         :param _InvalidSamples: 无效关键词列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type InvalidSamples: list of InvalidSample
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._SampleIDs = None
+        self._SuccessInfos = None
         self._DupInfos = None
         self._InvalidSamples = None
         self._RequestId = None
 
     @property
     def SampleIDs(self):
         return self._SampleIDs
 
     @SampleIDs.setter
     def SampleIDs(self, SampleIDs):
         self._SampleIDs = SampleIDs
 
     @property
+    def SuccessInfos(self):
+        return self._SuccessInfos
+
+    @SuccessInfos.setter
+    def SuccessInfos(self, SuccessInfos):
+        self._SuccessInfos = SuccessInfos
+
+    @property
     def DupInfos(self):
         return self._DupInfos
 
     @DupInfos.setter
     def DupInfos(self, DupInfos):
         self._DupInfos = DupInfos
 
@@ -430,14 +441,20 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._SampleIDs = params.get("SampleIDs")
+        if params.get("SuccessInfos") is not None:
+            self._SuccessInfos = []
+            for item in params.get("SuccessInfos"):
+                obj = UserKeywordInfo()
+                obj._deserialize(item)
+                self._SuccessInfos.append(obj)
         if params.get("DupInfos") is not None:
             self._DupInfos = []
             for item in params.get("DupInfos"):
                 obj = UserKeywordInfo()
                 obj._deserialize(item)
                 self._DupInfos.append(obj)
         if params.get("InvalidSamples") is not None:
@@ -521,21 +538,24 @@
 class DeleteLibSamplesRequest(AbstractModel):
     """DeleteLibSamples请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _SampleIDs: 关键词ID
+        :param _SampleIDs: 关键词ID列表
         :type SampleIDs: list of str
         :param _LibID: 词库ID
         :type LibID: str
+        :param _SampleContents: 关键词内容列表
+        :type SampleContents: list of str
         """
         self._SampleIDs = None
         self._LibID = None
+        self._SampleContents = None
 
     @property
     def SampleIDs(self):
         return self._SampleIDs
 
     @SampleIDs.setter
     def SampleIDs(self, SampleIDs):
@@ -545,18 +565,27 @@
     def LibID(self):
         return self._LibID
 
     @LibID.setter
     def LibID(self, LibID):
         self._LibID = LibID
 
+    @property
+    def SampleContents(self):
+        return self._SampleContents
+
+    @SampleContents.setter
+    def SampleContents(self, SampleContents):
+        self._SampleContents = SampleContents
+
 
     def _deserialize(self, params):
         self._SampleIDs = params.get("SampleIDs")
         self._LibID = params.get("LibID")
+        self._SampleContents = params.get("SampleContents")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -815,20 +844,23 @@
         :type Offset: int
         :param _LibID: 词库ID
         :type LibID: str
         :param _Content: 词内容过滤
         :type Content: str
         :param _EvilTypeList: 违规类型列表过滤
         :type EvilTypeList: list of int
+        :param _SampleIDs: 样本词ID列表过滤
+        :type SampleIDs: list of str
         """
         self._Limit = None
         self._Offset = None
         self._LibID = None
         self._Content = None
         self._EvilTypeList = None
+        self._SampleIDs = None
 
     @property
     def Limit(self):
         return self._Limit
 
     @Limit.setter
     def Limit(self, Limit):
@@ -862,21 +894,30 @@
     def EvilTypeList(self):
         return self._EvilTypeList
 
     @EvilTypeList.setter
     def EvilTypeList(self, EvilTypeList):
         self._EvilTypeList = EvilTypeList
 
+    @property
+    def SampleIDs(self):
+        return self._SampleIDs
+
+    @SampleIDs.setter
+    def SampleIDs(self, SampleIDs):
+        self._SampleIDs = SampleIDs
+
 
     def _deserialize(self, params):
         self._Limit = params.get("Limit")
         self._Offset = params.get("Offset")
         self._LibID = params.get("LibID")
         self._Content = params.get("Content")
         self._EvilTypeList = params.get("EvilTypeList")
+        self._SampleIDs = params.get("SampleIDs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cms-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cms-3.0.932/tencentcloud/__init__.py`

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

