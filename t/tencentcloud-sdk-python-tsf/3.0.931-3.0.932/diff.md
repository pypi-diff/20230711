# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.931.tar", last modified: Mon Jul 10 00:55:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.932.tar", last modified: Tue Jul 11 01:03:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.931.tar` & `tencentcloud-sdk-python-tsf-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49851 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1288536 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   196318 2023-07-10 00:55:51.000000 tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/tsf_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    50111 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1288536 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196318 2023-07-11 01:03:39.000000 tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/tsf_client.py
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/setup.py` & `tencentcloud-sdk-python-tsf-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.932/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/README.rst` & `tencentcloud-sdk-python-tsf-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.932/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,17 @@
 
 # TKE 集群删除失败。
 FAILEDOPERATION_TKECLUSTERDELETEFAILED = 'FailedOperation.TkeClusterDeleteFailed'
 
 # TKE 集群查询失败。
 FAILEDOPERATION_TKECLUSTERQUERYFAILED = 'FailedOperation.TkeClusterQueryFailed'
 
+# TOKEN查询失败。
+FAILEDOPERATION_TOKENQUERYFAILED = 'FailedOperation.TokenQueryFailed'
+
 # TSF应用性能管理任务数据库查询失败。
 FAILEDOPERATION_TSFAPMAGENTTASKQUERYERROR = 'FailedOperation.TsfApmAgentTaskQueryError'
 
 # TSF应用性能管理任务数据库写入失败。
 FAILEDOPERATION_TSFAPMAGENTTASKWRITEERROR = 'FailedOperation.TsfApmAgentTaskWriteError'
 
 # TSF应用性能管理apm-agent无法与该实例建立连接。
@@ -643,14 +646,17 @@
 
 # 所属应用ID不能为空。
 INVALIDPARAMETERVALUE_CONTAINERGROUPAPPLICATIONIDNULL = 'InvalidParameterValue.ContainergroupApplicationIdNull'
 
 # 集群 CPU 资源不足。
 INVALIDPARAMETERVALUE_CONTAINERGROUPCPULIMITOVER = 'InvalidParameterValue.ContainergroupCpulimitOver'
 
+# 容器 Env 的 Value 和 ValueFrom 至少要有一个。
+INVALIDPARAMETERVALUE_CONTAINERGROUPENVVALUENOTSET = 'InvalidParameterValue.ContainergroupEnvValueNotSet'
+
 # 部署组ID不能为空。
 INVALIDPARAMETERVALUE_CONTAINERGROUPGROUPIDNULL = 'InvalidParameterValue.ContainergroupGroupidNull'
 
 # 部署组名不能大于60个字符。
 INVALIDPARAMETERVALUE_CONTAINERGROUPGROUPNAMELEGNTH = 'InvalidParameterValue.ContainergroupGroupnameLegnth'
 
 # 部署组名不能为空。
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.931/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.932/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

