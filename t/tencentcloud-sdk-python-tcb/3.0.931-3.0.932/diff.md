# Comparing `tmp/tencentcloud-sdk-python-tcb-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-tcb-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.931.tar", last modified: Mon Jul 10 00:52:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.932.tar", last modified: Tue Jul 11 01:00:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcb-3.0.931.tar` & `tencentcloud-sdk-python-tcb-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   549244 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)    83901 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/tcb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:52:58.000000 tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   549856 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)    83901 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/tcb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:00:12.000000 tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.932/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/setup.py` & `tencentcloud-sdk-python-tcb-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.932/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/README.rst` & `tencentcloud-sdk-python-tcb-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/errorcodes.py` & `tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/models.py` & `tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15153,16 +15153,18 @@
     """安全网关版本路由信息限额配置
 
     """
 
     def __init__(self):
         r"""
         :param _LimitObject: 限额对象 "ConnectionsLimit" 或 "QPSLimit"
+注意：此字段可能返回 null，表示取不到有效值。
         :type LimitObject: str
         :param _LimitConfig: 限额配置
+注意：此字段可能返回 null，表示取不到有效值。
         :type LimitConfig: str
         """
         self._LimitObject = None
         self._LimitConfig = None
 
     @property
     def LimitObject(self):
@@ -19345,14 +19347,17 @@
         :type GatewayRoutePath: str
         :param _GatewayRouteMethod: 请求模式
 注意：此字段可能返回 null，表示取不到有效值。
         :type GatewayRouteMethod: str
         :param _GatewayRoutePort: 4层端口
 注意：此字段可能返回 null，表示取不到有效值。
         :type GatewayRoutePort: int
+        :param _GatewayRouteEnvId: 路由环境ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRouteEnvId: str
         """
         self._GatewayRouteName = None
         self._GatewayRouteProtocol = None
         self._GatewayRouteAddr = None
         self._GatewayRouteDesc = None
         self._GatewayRouteClusterId = None
         self._GatewayRouteCreateTime = None
@@ -19360,14 +19365,15 @@
         self._GatewayRouteServerType = None
         self._GatewayRouteServerName = None
         self._GatewayRewriteHost = None
         self._GatewayVersion = None
         self._GatewayRoutePath = None
         self._GatewayRouteMethod = None
         self._GatewayRoutePort = None
+        self._GatewayRouteEnvId = None
 
     @property
     def GatewayRouteName(self):
         return self._GatewayRouteName
 
     @GatewayRouteName.setter
     def GatewayRouteName(self, GatewayRouteName):
@@ -19473,14 +19479,22 @@
     def GatewayRoutePort(self):
         return self._GatewayRoutePort
 
     @GatewayRoutePort.setter
     def GatewayRoutePort(self, GatewayRoutePort):
         self._GatewayRoutePort = GatewayRoutePort
 
+    @property
+    def GatewayRouteEnvId(self):
+        return self._GatewayRouteEnvId
+
+    @GatewayRouteEnvId.setter
+    def GatewayRouteEnvId(self, GatewayRouteEnvId):
+        self._GatewayRouteEnvId = GatewayRouteEnvId
+
 
     def _deserialize(self, params):
         self._GatewayRouteName = params.get("GatewayRouteName")
         self._GatewayRouteProtocol = params.get("GatewayRouteProtocol")
         self._GatewayRouteAddr = params.get("GatewayRouteAddr")
         self._GatewayRouteDesc = params.get("GatewayRouteDesc")
         self._GatewayRouteClusterId = params.get("GatewayRouteClusterId")
@@ -19494,14 +19508,15 @@
         self._GatewayRouteServerType = params.get("GatewayRouteServerType")
         self._GatewayRouteServerName = params.get("GatewayRouteServerName")
         self._GatewayRewriteHost = params.get("GatewayRewriteHost")
         self._GatewayVersion = params.get("GatewayVersion")
         self._GatewayRoutePath = params.get("GatewayRoutePath")
         self._GatewayRouteMethod = params.get("GatewayRouteMethod")
         self._GatewayRoutePort = params.get("GatewayRoutePort")
+        self._GatewayRouteEnvId = params.get("GatewayRouteEnvId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/tcb/v20180608/tcb_client.py` & `tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/tcb/v20180608/tcb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcb-3.0.932/tencentcloud/__init__.py`

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

