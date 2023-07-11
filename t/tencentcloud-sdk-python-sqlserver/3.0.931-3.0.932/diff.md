# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.931.tar", last modified: Mon Jul 10 00:51:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.932.tar", last modified: Tue Jul 11 00:58:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.931.tar` & `tencentcloud-sdk-python-sqlserver-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:22.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)     9722 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   571541 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108601 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:51:21.000000 tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   571881 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108720 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:58:42.000000 tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.932/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12278,17 +12278,23 @@
 class InquiryPriceCreateDBInstancesResponse(AbstractModel):
     """InquiryPriceCreateDBInstances返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _OriginalPrice: 未打折前价格，其值除以100表示多少钱。例如10010表示100.10元
+        :param _OriginalPrice: 未打折前价格，其值除以100表示最终的价格。
+InstanceChargeType=PREPAID时，单位是"每月"。
+InstanceChargeType=POSTPAID时，单位是"每小时"。
+例如10010，在InstanceChargeType=PREPAID情况下，表示每月100.10元。
         :type OriginalPrice: int
-        :param _Price: 实际需要支付的价格，其值除以100表示多少钱。例如10010表示100.10元
+        :param _Price: 实际需要支付的价格，其值除以100表示最终的价格。
+InstanceChargeType=PREPAID时，单位是"每月"。
+InstanceChargeType=POSTPAID时，单位是"每小时"。
+例如10010，在InstanceChargeType=PREPAID情况下，表示每月100.10元。
         :type Price: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._OriginalPrice = None
         self._Price = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1564,15 +1564,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def InquiryPriceRenewDBInstance(self, request):
-        """本接口（InquiryPriceRenewDBInstance）用于查询续费实例的价格。
+        """本接口（InquiryPriceRenewDBInstance）用于查询包年包月实例的续费价格。
 
         :param request: Request instance for InquiryPriceRenewDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceRenewDBInstanceRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceRenewDBInstanceResponse`
 
         """
         try:
@@ -1587,15 +1587,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def InquiryPriceUpgradeDBInstance(self, request):
-        """本接口（InquiryPriceUpgradeDBInstance）用于查询升级实例的价格。
+        """本接口（InquiryPriceUpgradeDBInstance）用于查询包年包月实例升级变配的价格。
+        按量计费实例变配后的价格参考InquiryPriceCreateDBInstances接口。
 
         :param request: Request instance for InquiryPriceUpgradeDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceUpgradeDBInstanceRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceUpgradeDBInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.932/tencentcloud/__init__.py`

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

