# Comparing `tmp/tencentcloud-sdk-python-ecm-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-ecm-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.931.tar", last modified: Mon Jul 10 00:40:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.932.tar", last modified: Tue Jul 11 00:42:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecm-3.0.931.tar` & `tencentcloud-sdk-python-ecm-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)   126245 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)    23407 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   702119 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:06.000000 tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)   135627 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)    23498 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   731878 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:42:50.000000 tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/__init__.py
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/setup.py` & `tencentcloud-sdk-python-ecm-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.932/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/README.rst` & `tencentcloud-sdk-python-ecm-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.932/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def AllocateIpv6AddressesBandwidth(self, request):
+        """本接口用于给IPv6地址分配公网带宽
+
+        :param request: Request instance for AllocateIpv6AddressesBandwidth.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.AllocateIpv6AddressesBandwidthRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.AllocateIpv6AddressesBandwidthResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AllocateIpv6AddressesBandwidth", params, headers=headers)
+            response = json.loads(body)
+            model = models.AllocateIpv6AddressesBandwidthResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def AssignIpv6Addresses(self, request):
         """本接口（AssignIpv6Addresses）用于弹性网卡申请IPv6地址。
 
         :param request: Request instance for AssignIpv6Addresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6AddressesRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6AddressesResponse`
 
@@ -68,14 +91,91 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def AssignIpv6CidrBlock(self, request):
+        """本接口（AssignIpv6CidrBlock）用于分配IPv6网段。
+
+        使用本接口前，您需要已有VPC实例，如果没有可通过接口CreateVpc创建。
+
+        :param request: Request instance for AssignIpv6CidrBlock.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6CidrBlockRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6CidrBlockResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AssignIpv6CidrBlock", params, headers=headers)
+            response = json.loads(body)
+            model = models.AssignIpv6CidrBlockResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def AssignIpv6CidrBlocks(self, request):
+        """本接口（AssignIpv6CidrBlocks）用于分配IPv6网段。
+
+        使用本接口前，您需要已有VPC实例，如果没有可通过接口CreateVpc创建。
+        每个VPC 可以同时支持运营商网络('CMCC'-中国移动, 'CTCC'-中国电信, 'CUCC'-中国联调)。本接口可以同时申请不同类型的IPv6网段
+
+        :param request: Request instance for AssignIpv6CidrBlocks.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6CidrBlocksRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6CidrBlocksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AssignIpv6CidrBlocks", params, headers=headers)
+            response = json.loads(body)
+            model = models.AssignIpv6CidrBlocksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def AssignIpv6SubnetCidrBlock(self, request):
+        """本接口（AssignIpv6SubnetCidrBlock）用于分配IPv6子网段。
+
+        给子网分配 IPv6 网段，要求子网所属 VPC 已获得 IPv6 网段。如果尚未分配，请先通过接口 AssignIpv6CidrBlock 给子网所属 VPC 分配一个 IPv6 网段。否则无法分配 IPv6 子网段。
+        每个子网只能分配一个IPv6网段。
+
+        :param request: Request instance for AssignIpv6SubnetCidrBlock.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6SubnetCidrBlockRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6SubnetCidrBlockResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AssignIpv6SubnetCidrBlock", params, headers=headers)
+            response = json.loads(body)
+            model = models.AssignIpv6SubnetCidrBlockResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def AssignPrivateIpAddresses(self, request):
         """弹性网卡申请内网 IP
 
         :param request: Request instance for AssignPrivateIpAddresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AssignPrivateIpAddressesRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.AssignPrivateIpAddressesResponse`
 
@@ -1525,14 +1625,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeRegionIpv6Addresses(self, request):
+        """该接口（DescribeRegionIpv6Addresses）用于查询ECM地域之下的IPV6地址信息。
+
+        :param request: Request instance for DescribeRegionIpv6Addresses.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeRegionIpv6AddressesRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.DescribeRegionIpv6AddressesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRegionIpv6Addresses", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRegionIpv6AddressesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeRouteConflicts(self, request):
         """查询自定义路由策略与云联网路由策略冲突列表
 
         :param request: Request instance for DescribeRouteConflicts.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeRouteConflictsRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.DescribeRouteConflictsResponse`
 
@@ -2249,14 +2372,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyIpv6AddressesBandwidth(self, request):
+        """该接口(ModifyIpv6AddressesBandwidth)用于修改IPV6地址访问internet的带宽
+
+        :param request: Request instance for ModifyIpv6AddressesBandwidth.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyIpv6AddressesBandwidthRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.ModifyIpv6AddressesBandwidthResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyIpv6AddressesBandwidth", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyIpv6AddressesBandwidthResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyListener(self, request):
         """修改负载均衡监听器属性。
 
         :param request: Request instance for ModifyListener.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyListenerRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.ModifyListenerResponse`
 
@@ -2640,14 +2786,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def QueryVpcTaskResult(self, request):
+        """查询私有网络下Vpc、子网、havip等异步任务请求结果
+
+        :param request: Request instance for QueryVpcTaskResult.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.QueryVpcTaskResultRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.QueryVpcTaskResultResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryVpcTaskResult", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryVpcTaskResultResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RebootInstances(self, request):
         """只有状态为RUNNING的实例才可以进行此操作；接口调用成功时，实例会进入REBOOTING状态；重启实例成功时，实例会进入RUNNING状态；支持强制重启，强制重启的效果等同于关闭物理计算机的电源开关再重新启动。强制重启可能会导致数据丢失或文件系统损坏，请仅在服务器不能正常重启时使用。
 
         :param request: Request instance for RebootInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.RebootInstancesRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.RebootInstancesResponse`
 
@@ -2711,14 +2880,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ReleaseIpv6AddressesBandwidth(self, request):
+        """该接口用于给弹性公网IPv6地址释放带宽。
+
+        :param request: Request instance for ReleaseIpv6AddressesBandwidth.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.ReleaseIpv6AddressesBandwidthRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.ReleaseIpv6AddressesBandwidthResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ReleaseIpv6AddressesBandwidth", params, headers=headers)
+            response = json.loads(body)
+            model = models.ReleaseIpv6AddressesBandwidthResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RemovePrivateIpAddresses(self, request):
         """弹性网卡退还内网 IP。
         退还弹性网卡上的辅助内网IP，接口自动解关联弹性公网 IP。不能退还弹性网卡的主内网IP。
 
         :param request: Request instance for RemovePrivateIpAddresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.RemovePrivateIpAddressesRequest`
         :rtype: :class:`tencentcloud.ecm.v20190719.models.RemovePrivateIpAddressesResponse`
@@ -3060,8 +3252,32 @@
             model = models.TerminateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UnassignIpv6SubnetCidrBlock(self, request):
+        """本接口（UnassignIpv6SubnetCidrBlock）用于释放IPv6子网段。
+        子网段如果还有IP占用且未回收，则子网段无法释放。
+
+        :param request: Request instance for UnassignIpv6SubnetCidrBlock.
+        :type request: :class:`tencentcloud.ecm.v20190719.models.UnassignIpv6SubnetCidrBlockRequest`
+        :rtype: :class:`tencentcloud.ecm.v20190719.models.UnassignIpv6SubnetCidrBlockResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UnassignIpv6SubnetCidrBlock", params, headers=headers)
+            response = json.loads(body)
+            model = models.UnassignIpv6SubnetCidrBlockResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,17 @@
 
 # 资源被占用。
 RESOURCEINUSE = 'ResourceInUse'
 
 # 资源不足。
 RESOURCEINSUFFICIENT = 'ResourceInsufficient'
 
+# 网段资源不足。
+RESOURCEINSUFFICIENT_CIDRBLOCK = 'ResourceInsufficient.CidrBlock'
+
 # IP资源不足。
 RESOURCEINSUFFICIENT_IPQUOTANOTENOUGH = 'ResourceInsufficient.IPQuotaNotEnough'
 
 # 实例资源不足。
 RESOURCEINSUFFICIENT_INSTANCEQUOTANOTENOUGH = 'ResourceInsufficient.InstanceQuotaNotEnough'
 
 # 私有镜像数量超出限制。
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.931/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-ecm-3.0.932/tencentcloud/ecm/v20190719/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,133 @@
 
     def _deserialize(self, params):
         self._AddressSet = params.get("AddressSet")
         self._TaskId = params.get("TaskId")
         self._RequestId = params.get("RequestId")
 
 
+class AllocateIpv6AddressesBandwidthRequest(AbstractModel):
+    """AllocateIpv6AddressesBandwidth请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _EcmRegion: ECM 地域。
+        :type EcmRegion: str
+        :param _Ipv6Addresses: 需要开通公网访问能力的IPV6地址。
+        :type Ipv6Addresses: list of str
+        :param _InternetMaxBandwidthOut: 带宽，单位Mbps，默认是1Mbps。
+        :type InternetMaxBandwidthOut: int
+        :param _InternetChargeType: 网络计费模式，当前支持 BANDWIDTH_PACKAGE。
+        :type InternetChargeType: str
+        """
+        self._EcmRegion = None
+        self._Ipv6Addresses = None
+        self._InternetMaxBandwidthOut = None
+        self._InternetChargeType = None
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+    @property
+    def Ipv6Addresses(self):
+        return self._Ipv6Addresses
+
+    @Ipv6Addresses.setter
+    def Ipv6Addresses(self, Ipv6Addresses):
+        self._Ipv6Addresses = Ipv6Addresses
+
+    @property
+    def InternetMaxBandwidthOut(self):
+        return self._InternetMaxBandwidthOut
+
+    @InternetMaxBandwidthOut.setter
+    def InternetMaxBandwidthOut(self, InternetMaxBandwidthOut):
+        self._InternetMaxBandwidthOut = InternetMaxBandwidthOut
+
+    @property
+    def InternetChargeType(self):
+        return self._InternetChargeType
+
+    @InternetChargeType.setter
+    def InternetChargeType(self, InternetChargeType):
+        self._InternetChargeType = InternetChargeType
+
+
+    def _deserialize(self, params):
+        self._EcmRegion = params.get("EcmRegion")
+        self._Ipv6Addresses = params.get("Ipv6Addresses")
+        self._InternetMaxBandwidthOut = params.get("InternetMaxBandwidthOut")
+        self._InternetChargeType = params.get("InternetChargeType")
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
+class AllocateIpv6AddressesBandwidthResponse(AbstractModel):
+    """AllocateIpv6AddressesBandwidth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AddressSet: 弹性公网 IPV6 的唯一 ID 列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AddressSet: list of str
+        :param _TaskId: 异步任务TaskId。
+        :type TaskId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._AddressSet = None
+        self._TaskId = None
+        self._RequestId = None
+
+    @property
+    def AddressSet(self):
+        return self._AddressSet
+
+    @AddressSet.setter
+    def AddressSet(self, AddressSet):
+        self._AddressSet = AddressSet
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
+        self._AddressSet = params.get("AddressSet")
+        self._TaskId = params.get("TaskId")
+        self._RequestId = params.get("RequestId")
+
+
 class Area(AbstractModel):
     """区域信息
 
     """
 
     def __init__(self):
         r"""
@@ -730,14 +849,316 @@
             for item in params.get("Ipv6AddressSet"):
                 obj = Ipv6Address()
                 obj._deserialize(item)
                 self._Ipv6AddressSet.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class AssignIpv6CidrBlockRequest(AbstractModel):
+    """AssignIpv6CidrBlock请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _VpcId: `VPC`实例`ID`，形如：`vpc-f49l6u0z`。	
+        :type VpcId: str
+        :param _ISPType: 网络运营商类型 'CMCC'-中国移动, 'CTCC'-中国电信, 'CUCC'-中国联调	
+        :type ISPType: str
+        :param _EcmRegion: ECM地域。
+        :type EcmRegion: str
+        """
+        self._VpcId = None
+        self._ISPType = None
+        self._EcmRegion = None
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def ISPType(self):
+        return self._ISPType
+
+    @ISPType.setter
+    def ISPType(self, ISPType):
+        self._ISPType = ISPType
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+
+    def _deserialize(self, params):
+        self._VpcId = params.get("VpcId")
+        self._ISPType = params.get("ISPType")
+        self._EcmRegion = params.get("EcmRegion")
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
+class AssignIpv6CidrBlockResponse(AbstractModel):
+    """AssignIpv6CidrBlock返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Ipv6CidrBlock: 分配的 `IPv6` 网段。形如：`3402:4e00:20:1000::/56`。	
+        :type Ipv6CidrBlock: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Ipv6CidrBlock = None
+        self._RequestId = None
+
+    @property
+    def Ipv6CidrBlock(self):
+        return self._Ipv6CidrBlock
+
+    @Ipv6CidrBlock.setter
+    def Ipv6CidrBlock(self, Ipv6CidrBlock):
+        self._Ipv6CidrBlock = Ipv6CidrBlock
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
+        self._Ipv6CidrBlock = params.get("Ipv6CidrBlock")
+        self._RequestId = params.get("RequestId")
+
+
+class AssignIpv6CidrBlocksRequest(AbstractModel):
+    """AssignIpv6CidrBlocks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _VpcId: `VPC`实例`ID`，形如：`vpc-f49l6u0z`。	
+        :type VpcId: str
+        :param _ISPTypes: 网络运营商类型 取值范围:'CMCC'-中国移动, 'CTCC'-中国电信, 'CUCC'-中国联调	
+        :type ISPTypes: list of ISPTypeItem
+        :param _EcmRegion: ECM地域。
+        :type EcmRegion: str
+        """
+        self._VpcId = None
+        self._ISPTypes = None
+        self._EcmRegion = None
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def ISPTypes(self):
+        return self._ISPTypes
+
+    @ISPTypes.setter
+    def ISPTypes(self, ISPTypes):
+        self._ISPTypes = ISPTypes
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+
+    def _deserialize(self, params):
+        self._VpcId = params.get("VpcId")
+        if params.get("ISPTypes") is not None:
+            self._ISPTypes = []
+            for item in params.get("ISPTypes"):
+                obj = ISPTypeItem()
+                obj._deserialize(item)
+                self._ISPTypes.append(obj)
+        self._EcmRegion = params.get("EcmRegion")
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
+class AssignIpv6CidrBlocksResponse(AbstractModel):
+    """AssignIpv6CidrBlocks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _IPv6CidrBlockSet: IPv6网段和所属运营商。	
+        :type IPv6CidrBlockSet: list of ISPIPv6CidrBlock
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._IPv6CidrBlockSet = None
+        self._RequestId = None
+
+    @property
+    def IPv6CidrBlockSet(self):
+        return self._IPv6CidrBlockSet
+
+    @IPv6CidrBlockSet.setter
+    def IPv6CidrBlockSet(self, IPv6CidrBlockSet):
+        self._IPv6CidrBlockSet = IPv6CidrBlockSet
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
+        if params.get("IPv6CidrBlockSet") is not None:
+            self._IPv6CidrBlockSet = []
+            for item in params.get("IPv6CidrBlockSet"):
+                obj = ISPIPv6CidrBlock()
+                obj._deserialize(item)
+                self._IPv6CidrBlockSet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class AssignIpv6SubnetCidrBlockRequest(AbstractModel):
+    """AssignIpv6SubnetCidrBlock请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _VpcId: 子网所在私有网络`ID`。形如：`vpc-f49l6u0z`。	
+        :type VpcId: str
+        :param _Ipv6SubnetCidrBlocks: 分配 `IPv6` 子网段列表。
+        :type Ipv6SubnetCidrBlocks: list of Ipv6SubnetCidrBlock
+        :param _EcmRegion: ECM地域。
+        :type EcmRegion: str
+        """
+        self._VpcId = None
+        self._Ipv6SubnetCidrBlocks = None
+        self._EcmRegion = None
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def Ipv6SubnetCidrBlocks(self):
+        return self._Ipv6SubnetCidrBlocks
+
+    @Ipv6SubnetCidrBlocks.setter
+    def Ipv6SubnetCidrBlocks(self, Ipv6SubnetCidrBlocks):
+        self._Ipv6SubnetCidrBlocks = Ipv6SubnetCidrBlocks
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+
+    def _deserialize(self, params):
+        self._VpcId = params.get("VpcId")
+        if params.get("Ipv6SubnetCidrBlocks") is not None:
+            self._Ipv6SubnetCidrBlocks = []
+            for item in params.get("Ipv6SubnetCidrBlocks"):
+                obj = Ipv6SubnetCidrBlock()
+                obj._deserialize(item)
+                self._Ipv6SubnetCidrBlocks.append(obj)
+        self._EcmRegion = params.get("EcmRegion")
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
+class AssignIpv6SubnetCidrBlockResponse(AbstractModel):
+    """AssignIpv6SubnetCidrBlock返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Ipv6SubnetCidrBlockSet: 分配 `IPv6` 子网段列表。	
+        :type Ipv6SubnetCidrBlockSet: list of Ipv6SubnetCidrBlock
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Ipv6SubnetCidrBlockSet = None
+        self._RequestId = None
+
+    @property
+    def Ipv6SubnetCidrBlockSet(self):
+        return self._Ipv6SubnetCidrBlockSet
+
+    @Ipv6SubnetCidrBlockSet.setter
+    def Ipv6SubnetCidrBlockSet(self, Ipv6SubnetCidrBlockSet):
+        self._Ipv6SubnetCidrBlockSet = Ipv6SubnetCidrBlockSet
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
+        if params.get("Ipv6SubnetCidrBlockSet") is not None:
+            self._Ipv6SubnetCidrBlockSet = []
+            for item in params.get("Ipv6SubnetCidrBlockSet"):
+                obj = Ipv6SubnetCidrBlock()
+                obj._deserialize(item)
+                self._Ipv6SubnetCidrBlockSet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class AssignPrivateIpAddressesRequest(AbstractModel):
     """AssignPrivateIpAddresses请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7702,14 +8123,149 @@
     def _deserialize(self, params):
         if params.get("InstancePrice") is not None:
             self._InstancePrice = InstancesPrice()
             self._InstancePrice._deserialize(params.get("InstancePrice"))
         self._RequestId = params.get("RequestId")
 
 
+class DescribeRegionIpv6AddressesRequest(AbstractModel):
+    """DescribeRegionIpv6Addresses请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _EcmRegion: ECM 地域，为空时返回所有地域的IPv6地址。
+        :type EcmRegion: str
+        :param _Filters: 详细的过滤条件如下：
+address-id - String - 是否必填：否 - （过滤条件）按照 EIP 的 ID 过滤。
+address-ip - String - 是否必填：否 - （过滤条件）按照 EIP 的 IP 地址过滤。
+network-interface-id - String - 是否必填：否 - （过滤条件）按照弹性网卡的唯一ID过滤。
+instance-id - String - 是否必填：否 - （过滤条件）按照 EIP 所绑定的实例 ID 过滤。
+vpc-id - String - 是否必填：否 - （过滤条件）按照 EIP 所在 VPC 的 ID 进行过滤。
+address-isp - String - 是否必填：否 - （过滤条件）按照 EIP 的运营商进行过滤。
+address-status  - String - 是否必填：否 - （过滤条件）按照 EIP  的状态信息进行过滤。
+        :type Filters: list of Filter
+        :param _Offset: 偏移量，默认为0。关于Offset的更进一步介绍请参考 API 简介中的相关小节。
+        :type Offset: int
+        :param _Limit: 返回数量，默认为20，最大值为100。关于Limit的更进一步介绍请参考 API 简介中的相关小节。
+        :type Limit: int
+        """
+        self._EcmRegion = None
+        self._Filters = None
+        self._Offset = None
+        self._Limit = None
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
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
+
+    def _deserialize(self, params):
+        self._EcmRegion = params.get("EcmRegion")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
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
+class DescribeRegionIpv6AddressesResponse(AbstractModel):
+    """DescribeRegionIpv6Addresses返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 符合条件的 IPV6 数量。
+        :type TotalCount: int
+        :param _AddressSet: IPV6 详细信息列表。
+        :type AddressSet: list of Address
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._AddressSet = None
+        self._RequestId = None
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
+    def AddressSet(self):
+        return self._AddressSet
+
+    @AddressSet.setter
+    def AddressSet(self, AddressSet):
+        self._AddressSet = AddressSet
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("AddressSet") is not None:
+            self._AddressSet = []
+            for item in params.get("AddressSet"):
+                obj = Address()
+                obj._deserialize(item)
+                self._AddressSet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeRouteConflictsRequest(AbstractModel):
     """DescribeRouteConflicts请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10894,14 +11450,59 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ISPTypeItem(AbstractModel):
+    """申请ipv6 cidr block的信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ISPType: IPv6 Cidr所属运营商类型，支持的类型有 'CMCC'-中国移动, 'CTCC'-中国电信, 'CUCC'-中国联调。作为入参数时为必选。
+        :type ISPType: str
+        :param _Count: 申请IPv6 Cidr Block的个数。作为入参数时为必选。
+        :type Count: int
+        """
+        self._ISPType = None
+        self._Count = None
+
+    @property
+    def ISPType(self):
+        return self._ISPType
+
+    @ISPType.setter
+    def ISPType(self, ISPType):
+        self._ISPType = ISPType
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+
+    def _deserialize(self, params):
+        self._ISPType = params.get("ISPType")
+        self._Count = params.get("Count")
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
 class Image(AbstractModel):
     """镜像信息
 
     """
 
     def __init__(self):
         r"""
@@ -12758,14 +13359,61 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Ipv6SubnetCidrBlock(AbstractModel):
+    """IPv6子网段对象。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _SubnetId: 子网实例`ID`。形如：`subnet-pxir56ns`。	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param _Ipv6CidrBlock: `IPv6`子网段。形如：`3402:4e00:20:1001::/64`	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Ipv6CidrBlock: str
+        """
+        self._SubnetId = None
+        self._Ipv6CidrBlock = None
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+    @property
+    def Ipv6CidrBlock(self):
+        return self._Ipv6CidrBlock
+
+    @Ipv6CidrBlock.setter
+    def Ipv6CidrBlock(self, Ipv6CidrBlock):
+        self._Ipv6CidrBlock = Ipv6CidrBlock
+
+
+    def _deserialize(self, params):
+        self._SubnetId = params.get("SubnetId")
+        self._Ipv6CidrBlock = params.get("Ipv6CidrBlock")
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
 class KeyPair(AbstractModel):
     """描述密钥对信息
 
     """
 
     def __init__(self):
         r"""
@@ -14336,14 +14984,113 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyIpv6AddressesBandwidthRequest(AbstractModel):
+    """ModifyIpv6AddressesBandwidth请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _EcmRegion: ECM 地域
+        :type EcmRegion: str
+        :param _InternetMaxBandwidthOut: 修改的目标带宽，单位Mbps
+        :type InternetMaxBandwidthOut: int
+        :param _Ipv6Addresses: IPV6地址。Ipv6Addresses和Ipv6AddressId必须且只能传一个
+        :type Ipv6Addresses: list of Ipv6Address
+        :param _Ipv6AddressIds: IPV6地址对应的唯一ID，形如eip-xxxxxxxx。Ipv6Addresses和Ipv6AddressId必须且只能传一个
+        :type Ipv6AddressIds: list of str
+        """
+        self._EcmRegion = None
+        self._InternetMaxBandwidthOut = None
+        self._Ipv6Addresses = None
+        self._Ipv6AddressIds = None
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+    @property
+    def InternetMaxBandwidthOut(self):
+        return self._InternetMaxBandwidthOut
+
+    @InternetMaxBandwidthOut.setter
+    def InternetMaxBandwidthOut(self, InternetMaxBandwidthOut):
+        self._InternetMaxBandwidthOut = InternetMaxBandwidthOut
+
+    @property
+    def Ipv6Addresses(self):
+        return self._Ipv6Addresses
+
+    @Ipv6Addresses.setter
+    def Ipv6Addresses(self, Ipv6Addresses):
+        self._Ipv6Addresses = Ipv6Addresses
+
+    @property
+    def Ipv6AddressIds(self):
+        return self._Ipv6AddressIds
+
+    @Ipv6AddressIds.setter
+    def Ipv6AddressIds(self, Ipv6AddressIds):
+        self._Ipv6AddressIds = Ipv6AddressIds
+
+
+    def _deserialize(self, params):
+        self._EcmRegion = params.get("EcmRegion")
+        self._InternetMaxBandwidthOut = params.get("InternetMaxBandwidthOut")
+        if params.get("Ipv6Addresses") is not None:
+            self._Ipv6Addresses = []
+            for item in params.get("Ipv6Addresses"):
+                obj = Ipv6Address()
+                obj._deserialize(item)
+                self._Ipv6Addresses.append(obj)
+        self._Ipv6AddressIds = params.get("Ipv6AddressIds")
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
+class ModifyIpv6AddressesBandwidthResponse(AbstractModel):
+    """ModifyIpv6AddressesBandwidth返回参数结构体
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
 class ModifyListenerRequest(AbstractModel):
     """ModifyListener请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18198,14 +18945,96 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class QueryVpcTaskResultRequest(AbstractModel):
+    """QueryVpcTaskResult请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 无
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
+class QueryVpcTaskResultResponse(AbstractModel):
+    """QueryVpcTaskResult返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: 执行结果，包括"SUCCESS", "FAILED", "RUNNING"
+        :type Status: str
+        :param _Output: 异步任务执行输出。
+        :type Output: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Status = None
+        self._Output = None
+        self._RequestId = None
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
+    def Output(self):
+        return self._Output
+
+    @Output.setter
+    def Output(self, Output):
+        self._Output = Output
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
+        self._Status = params.get("Status")
+        self._Output = params.get("Output")
+        self._RequestId = params.get("RequestId")
+
+
 class RebootInstancesRequest(AbstractModel):
     """RebootInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18427,14 +19256,108 @@
 
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._RequestId = params.get("RequestId")
 
 
+class ReleaseIpv6AddressesBandwidthRequest(AbstractModel):
+    """ReleaseIpv6AddressesBandwidth请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _EcmRegion: ECM 地域。
+        :type EcmRegion: str
+        :param _Ipv6Addresses: IPV6地址。Ipv6Addresses和Ipv6AddressIds必须且只能传一个。
+        :type Ipv6Addresses: list of str
+        :param _Ipv6AddressIds: IPV6地址对应的唯一ID，形如eip-xxxxxxxx。Ipv6Addresses和Ipv6AddressIds必须且只能传一个。
+        :type Ipv6AddressIds: list of str
+        """
+        self._EcmRegion = None
+        self._Ipv6Addresses = None
+        self._Ipv6AddressIds = None
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+    @property
+    def Ipv6Addresses(self):
+        return self._Ipv6Addresses
+
+    @Ipv6Addresses.setter
+    def Ipv6Addresses(self, Ipv6Addresses):
+        self._Ipv6Addresses = Ipv6Addresses
+
+    @property
+    def Ipv6AddressIds(self):
+        return self._Ipv6AddressIds
+
+    @Ipv6AddressIds.setter
+    def Ipv6AddressIds(self, Ipv6AddressIds):
+        self._Ipv6AddressIds = Ipv6AddressIds
+
+
+    def _deserialize(self, params):
+        self._EcmRegion = params.get("EcmRegion")
+        self._Ipv6Addresses = params.get("Ipv6Addresses")
+        self._Ipv6AddressIds = params.get("Ipv6AddressIds")
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
+class ReleaseIpv6AddressesBandwidthResponse(AbstractModel):
+    """ReleaseIpv6AddressesBandwidth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 异步任务TaskId。
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
 class ReleaseIpv6AddressesRequest(AbstractModel):
     """ReleaseIpv6Addresses请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -22420,14 +23343,101 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class UnassignIpv6SubnetCidrBlockRequest(AbstractModel):
+    """UnassignIpv6SubnetCidrBlock请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _VpcId: 子网所在私有网络`ID`。形如：`vpc-f49l6u0z`。	
+        :type VpcId: str
+        :param _Ipv6SubnetCidrBlocks: `IPv6` 子网段列表。	
+        :type Ipv6SubnetCidrBlocks: list of Ipv6SubnetCidrBlock
+        :param _EcmRegion: ECM地域。
+        :type EcmRegion: str
+        """
+        self._VpcId = None
+        self._Ipv6SubnetCidrBlocks = None
+        self._EcmRegion = None
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def Ipv6SubnetCidrBlocks(self):
+        return self._Ipv6SubnetCidrBlocks
+
+    @Ipv6SubnetCidrBlocks.setter
+    def Ipv6SubnetCidrBlocks(self, Ipv6SubnetCidrBlocks):
+        self._Ipv6SubnetCidrBlocks = Ipv6SubnetCidrBlocks
+
+    @property
+    def EcmRegion(self):
+        return self._EcmRegion
+
+    @EcmRegion.setter
+    def EcmRegion(self, EcmRegion):
+        self._EcmRegion = EcmRegion
+
+
+    def _deserialize(self, params):
+        self._VpcId = params.get("VpcId")
+        if params.get("Ipv6SubnetCidrBlocks") is not None:
+            self._Ipv6SubnetCidrBlocks = []
+            for item in params.get("Ipv6SubnetCidrBlocks"):
+                obj = Ipv6SubnetCidrBlock()
+                obj._deserialize(item)
+                self._Ipv6SubnetCidrBlocks.append(obj)
+        self._EcmRegion = params.get("EcmRegion")
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
+class UnassignIpv6SubnetCidrBlockResponse(AbstractModel):
+    """UnassignIpv6SubnetCidrBlock返回参数结构体
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
 class VirtualPrivateCloud(AbstractModel):
     """私有网络相关信息配置。
 
     """
 
     def __init__(self):
         r"""
@@ -22852,15 +23862,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Zone: 创建实例的可用区。
         :type Zone: str
-        :param _InstanceCount: 在当前可用区欲创建的实例数目。
+        :param _InstanceCount: 在当前可用区创建的实例数目。
         :type InstanceCount: int
         :param _ISP: 运营商如下：
 CTCC：中国电信
 CUCC：中国联通
 CMCC：中国移动
 多个运营商用英文分号连接";"，例如："CMCC;CUCC;CTCC"。多运营商需要开通白名单，请直接联系腾讯云客服。
         :type ISP: str
```

