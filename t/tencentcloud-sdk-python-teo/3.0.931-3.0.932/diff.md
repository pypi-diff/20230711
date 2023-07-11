# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.931.tar", last modified: Mon Jul 10 00:54:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.932.tar", last modified: Tue Jul 11 01:01:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.931.tar` & `tencentcloud-sdk-python-teo-3.0.932.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    22836 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   605318 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    60328 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:54:08.000000 tencentcloud-sdk-python-teo-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    23221 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605318 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    60328 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:01:40.000000 tencentcloud-sdk-python-teo-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.931/setup.py` & `tencentcloud-sdk-python-teo-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.931/README.rst` & `tencentcloud-sdk-python-teo-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,17 @@
 
 # 无效的token鉴权密钥。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPESECRETKEY = 'InvalidParameter.InvalidAuthenticationTypeSecretKey'
 
 # 无效的token鉴权参数。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPESIGNPARAM = 'InvalidParameter.InvalidAuthenticationTypeSignParam'
 
+# 无效的token鉴权时间格式。
+INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPETIMEFORMAT = 'InvalidParameter.InvalidAuthenticationTypeTimeFormat'
+
 # 无效的第三方对象存储。
 INVALIDPARAMETER_INVALIDAWSPRIVATEACCESS = 'InvalidParameter.InvalidAwsPrivateAccess'
 
 # 无效的备源回源Host。
 INVALIDPARAMETER_INVALIDBACKUPSERVERNAME = 'InvalidParameter.InvalidBackupServerName'
 
 # 无效的节点缓存。
@@ -253,14 +256,17 @@
 
 # 无效的HTTPS TLS版本。
 INVALIDPARAMETER_INVALIDHTTPSTLSVERSION = 'InvalidParameter.InvalidHttpsTlsVersion'
 
 # 无效的Ipv6开关配置。
 INVALIDPARAMETER_INVALIDIPV6SWITCH = 'InvalidParameter.InvalidIpv6Switch'
 
+# 无效的浏览器缓存。
+INVALIDPARAMETER_INVALIDMAXAGETIME = 'InvalidParameter.InvalidMaxAgeTime'
+
 # 无效的源站。
 INVALIDPARAMETER_INVALIDORIGIN = 'InvalidParameter.InvalidOrigin'
 
 # 不支持填写内网IP/回环地址作为源站地址
 INVALIDPARAMETER_INVALIDORIGINIP = 'InvalidParameter.InvalidOriginIp'
 
 # 参数错误。
@@ -313,14 +319,17 @@
 
 # 无效的规则引擎URL条件。
 INVALIDPARAMETER_INVALIDRULEENGINETARGETSURL = 'InvalidParameter.InvalidRuleEngineTargetsUrl'
 
 # 无效的回源Host。
 INVALIDPARAMETER_INVALIDSERVERNAME = 'InvalidParameter.InvalidServerName'
 
+# 无效的客户端ip或ip段。
+INVALIDPARAMETER_INVALIDSTANDARDDEBUGCLIENTIP = 'InvalidParameter.InvalidStandardDebugClientIp'
+
 # 无效的回源请求参数设置-无效查询字符串值。
 INVALIDPARAMETER_INVALIDUPSTREAMREQUESTQUERYSTRINGVALUE = 'InvalidParameter.InvalidUpstreamRequestQueryStringValue'
 
 # URL重写的目标HOST无效。
 INVALIDPARAMETER_INVALIDURLREDIRECTHOST = 'InvalidParameter.InvalidUrlRedirectHost'
 
 # URL重写的目标URL无效。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.932/tencentcloud/__init__.py`

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

