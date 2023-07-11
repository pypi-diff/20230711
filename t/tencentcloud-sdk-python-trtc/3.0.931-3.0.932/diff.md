# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.931.tar", last modified: Mon Jul 10 00:55:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.932.tar", last modified: Tue Jul 11 01:03:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.931.tar` & `tencentcloud-sdk-python-trtc-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)    58535 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   298259 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:41.000000 tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)    57241 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   287746 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:27.000000 tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/__init__.py
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/setup.py` & `tencentcloud-sdk-python-trtc-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/README.rst` & `tencentcloud-sdk-python-trtc-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.932/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,40 +175,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeExternalTrtcMeasure(self, request):
-        """接口内部调用计量接口，计量接口迁通用集群后不可用。目前已有新的对外接口可以供用户使用。
-
-        获取Trtc的用量统计数据。走计费渠道二期 只允许查两天的数据。
-        当前接口已不再更新维护，请使用新版音视频用量接口：DescribeTrtcUsage （https://cloud.tencent.com/document/product/647/81425）
-
-        :param request: Request instance for DescribeExternalTrtcMeasure.
-        :type request: :class:`tencentcloud.trtc.v20190722.models.DescribeExternalTrtcMeasureRequest`
-        :rtype: :class:`tencentcloud.trtc.v20190722.models.DescribeExternalTrtcMeasureResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeExternalTrtcMeasure", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeExternalTrtcMeasureResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeMixTranscodingUsage(self, request):
         """获取TRTC混流转码的用量明细。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
         - 该接口只用于历史用量数据统计或核对数据使用，关键业务逻辑不能使用。
         - 默认接口请求频率限制：5次/秒。
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.931/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.932/tencentcloud/trtc/v20190722/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1283,137 +1283,14 @@
             for item in params.get("StorageFileList"):
                 obj = StorageFile()
                 obj._deserialize(item)
                 self._StorageFileList.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeExternalTrtcMeasureRequest(AbstractModel):
-    """DescribeExternalTrtcMeasure请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 查询开始日期。
-        :type StartTime: str
-        :param _EndTime: 查询结束日期。
-        :type EndTime: str
-        :param _SdkAppId: 对应的应用。如果没有这个参数，表示获取用户名下全部实时音视频应用的汇总。
-        :type SdkAppId: int
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._SdkAppId = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def SdkAppId(self):
-        return self._SdkAppId
-
-    @SdkAppId.setter
-    def SdkAppId(self, SdkAppId):
-        self._SdkAppId = SdkAppId
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._SdkAppId = params.get("SdkAppId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeExternalTrtcMeasureResponse(AbstractModel):
-    """DescribeExternalTrtcMeasure返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SdkAppIdTrtrTimeUsages: 每个SdkAppId的时长使用信息
-        :type SdkAppIdTrtrTimeUsages: list of SdkAppIdNewTrtcTimeUsage
-        :param _AnchorUsageMode: 主播的用量统计方式。取值"InRoomTime":房间时长,"SubscribeTime":"订阅时长","Bandwidth":带宽
-        :type AnchorUsageMode: str
-        :param _AudienceUsageMode: 观众的用量统计方式。取值"InRoomTime":在房间时长,"SubscribeTime":"订阅时长","Bandwidth":带宽,"MergeWithAnchor":"不区分麦上麦下"
-        :type AudienceUsageMode: str
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._SdkAppIdTrtrTimeUsages = None
-        self._AnchorUsageMode = None
-        self._AudienceUsageMode = None
-        self._RequestId = None
-
-    @property
-    def SdkAppIdTrtrTimeUsages(self):
-        return self._SdkAppIdTrtrTimeUsages
-
-    @SdkAppIdTrtrTimeUsages.setter
-    def SdkAppIdTrtrTimeUsages(self, SdkAppIdTrtrTimeUsages):
-        self._SdkAppIdTrtrTimeUsages = SdkAppIdTrtrTimeUsages
-
-    @property
-    def AnchorUsageMode(self):
-        return self._AnchorUsageMode
-
-    @AnchorUsageMode.setter
-    def AnchorUsageMode(self, AnchorUsageMode):
-        self._AnchorUsageMode = AnchorUsageMode
-
-    @property
-    def AudienceUsageMode(self):
-        return self._AudienceUsageMode
-
-    @AudienceUsageMode.setter
-    def AudienceUsageMode(self, AudienceUsageMode):
-        self._AudienceUsageMode = AudienceUsageMode
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("SdkAppIdTrtrTimeUsages") is not None:
-            self._SdkAppIdTrtrTimeUsages = []
-            for item in params.get("SdkAppIdTrtrTimeUsages"):
-                obj = SdkAppIdNewTrtcTimeUsage()
-                obj._deserialize(item)
-                self._SdkAppIdTrtrTimeUsages.append(obj)
-        self._AnchorUsageMode = params.get("AnchorUsageMode")
-        self._AudienceUsageMode = params.get("AudienceUsageMode")
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeMixTranscodingUsageRequest(AbstractModel):
     """DescribeMixTranscodingUsage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6850,81 +6727,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class SdkAppIdNewTrtcTimeUsage(AbstractModel):
-    """SdkAppId级别实时音视频的用量数据
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SdkAppId: SdkAppId的值。
-        :type SdkAppId: str
-        :param _TrtcTimeUsages: 统计的时间点数据。
-        :type TrtcTimeUsages: list of TrtcTimeNewUsage
-        :param _AudienceTrtcTimeUsages: 统计的麦下用量的时间点数据。
-        :type AudienceTrtcTimeUsages: list of TrtcTimeNewUsage
-        """
-        self._SdkAppId = None
-        self._TrtcTimeUsages = None
-        self._AudienceTrtcTimeUsages = None
-
-    @property
-    def SdkAppId(self):
-        return self._SdkAppId
-
-    @SdkAppId.setter
-    def SdkAppId(self, SdkAppId):
-        self._SdkAppId = SdkAppId
-
-    @property
-    def TrtcTimeUsages(self):
-        return self._TrtcTimeUsages
-
-    @TrtcTimeUsages.setter
-    def TrtcTimeUsages(self, TrtcTimeUsages):
-        self._TrtcTimeUsages = TrtcTimeUsages
-
-    @property
-    def AudienceTrtcTimeUsages(self):
-        return self._AudienceTrtcTimeUsages
-
-    @AudienceTrtcTimeUsages.setter
-    def AudienceTrtcTimeUsages(self, AudienceTrtcTimeUsages):
-        self._AudienceTrtcTimeUsages = AudienceTrtcTimeUsages
-
-
-    def _deserialize(self, params):
-        self._SdkAppId = params.get("SdkAppId")
-        if params.get("TrtcTimeUsages") is not None:
-            self._TrtcTimeUsages = []
-            for item in params.get("TrtcTimeUsages"):
-                obj = TrtcTimeNewUsage()
-                obj._deserialize(item)
-                self._TrtcTimeUsages.append(obj)
-        if params.get("AudienceTrtcTimeUsages") is not None:
-            self._AudienceTrtcTimeUsages = []
-            for item in params.get("AudienceTrtcTimeUsages"):
-                obj = TrtcTimeNewUsage()
-                obj._deserialize(item)
-                self._AudienceTrtcTimeUsages.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class SdkAppIdRecordUsage(AbstractModel):
     """SdkAppId级别录制时长数据。
 
     """
 
     def __init__(self):
         r"""
@@ -8349,155 +8159,14 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class TrtcTimeNewUsage(AbstractModel):
-    """实时音视频用量的某一时间段的统计信息.
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TimeKey: 时间点。
-        :type TimeKey: str
-        :param _VoiceUserNum: 通话人数。仅供参考。在线人数以仪表盘查询结果为准。
-        :type VoiceUserNum: int
-        :param _VideoTime: 音视频通话收费时长。单位：秒。
-        :type VideoTime: int
-        :param _Class1VideoTime: 标清视频通话收费时长。单位：秒。
-        :type Class1VideoTime: int
-        :param _Class2VideoTime: 高清视频通话收费时长。单位：秒。
-        :type Class2VideoTime: int
-        :param _Class3VideoTime: 超高清视频通话收费时长。单位：秒。
-        :type Class3VideoTime: int
-        :param _AudioTime: 音频通话收费时长。单位：秒。
-        :type AudioTime: int
-        :param _Bandwidth: 带宽。单位：Mbps。
-        :type Bandwidth: float
-        :param _Video2KTime: 2k视频通话收费时长。单位：秒。
-        :type Video2KTime: int
-        :param _Video4KTime: 4k视频通话收费时长。单位：秒。
-        :type Video4KTime: int
-        """
-        self._TimeKey = None
-        self._VoiceUserNum = None
-        self._VideoTime = None
-        self._Class1VideoTime = None
-        self._Class2VideoTime = None
-        self._Class3VideoTime = None
-        self._AudioTime = None
-        self._Bandwidth = None
-        self._Video2KTime = None
-        self._Video4KTime = None
-
-    @property
-    def TimeKey(self):
-        return self._TimeKey
-
-    @TimeKey.setter
-    def TimeKey(self, TimeKey):
-        self._TimeKey = TimeKey
-
-    @property
-    def VoiceUserNum(self):
-        return self._VoiceUserNum
-
-    @VoiceUserNum.setter
-    def VoiceUserNum(self, VoiceUserNum):
-        self._VoiceUserNum = VoiceUserNum
-
-    @property
-    def VideoTime(self):
-        return self._VideoTime
-
-    @VideoTime.setter
-    def VideoTime(self, VideoTime):
-        self._VideoTime = VideoTime
-
-    @property
-    def Class1VideoTime(self):
-        return self._Class1VideoTime
-
-    @Class1VideoTime.setter
-    def Class1VideoTime(self, Class1VideoTime):
-        self._Class1VideoTime = Class1VideoTime
-
-    @property
-    def Class2VideoTime(self):
-        return self._Class2VideoTime
-
-    @Class2VideoTime.setter
-    def Class2VideoTime(self, Class2VideoTime):
-        self._Class2VideoTime = Class2VideoTime
-
-    @property
-    def Class3VideoTime(self):
-        return self._Class3VideoTime
-
-    @Class3VideoTime.setter
-    def Class3VideoTime(self, Class3VideoTime):
-        self._Class3VideoTime = Class3VideoTime
-
-    @property
-    def AudioTime(self):
-        return self._AudioTime
-
-    @AudioTime.setter
-    def AudioTime(self, AudioTime):
-        self._AudioTime = AudioTime
-
-    @property
-    def Bandwidth(self):
-        return self._Bandwidth
-
-    @Bandwidth.setter
-    def Bandwidth(self, Bandwidth):
-        self._Bandwidth = Bandwidth
-
-    @property
-    def Video2KTime(self):
-        return self._Video2KTime
-
-    @Video2KTime.setter
-    def Video2KTime(self, Video2KTime):
-        self._Video2KTime = Video2KTime
-
-    @property
-    def Video4KTime(self):
-        return self._Video4KTime
-
-    @Video4KTime.setter
-    def Video4KTime(self, Video4KTime):
-        self._Video4KTime = Video4KTime
-
-
-    def _deserialize(self, params):
-        self._TimeKey = params.get("TimeKey")
-        self._VoiceUserNum = params.get("VoiceUserNum")
-        self._VideoTime = params.get("VideoTime")
-        self._Class1VideoTime = params.get("Class1VideoTime")
-        self._Class2VideoTime = params.get("Class2VideoTime")
-        self._Class3VideoTime = params.get("Class3VideoTime")
-        self._AudioTime = params.get("AudioTime")
-        self._Bandwidth = params.get("Bandwidth")
-        self._Video2KTime = params.get("Video2KTime")
-        self._Video4KTime = params.get("Video4KTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TrtcUsage(AbstractModel):
     """实时音视频用量在某一时间段的统计信息。
 
     """
```

