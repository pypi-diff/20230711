# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.931.tar", last modified: Mon Jul 10 00:38:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.932.tar", last modified: Tue Jul 11 00:41:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.931.tar` & `tencentcloud-sdk-python-cynosdb-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    11292 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   679291 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   118494 2023-07-10 00:38:22.000000 tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   679294 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   118494 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/cynosdb_client.py
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
         :param _DbType: 数据库类型，取值范围: 
 <li> MYSQL </li>
         :type DbType: str
         :param _OrderSource: 订单来源，字符串长度范围为[0,64)
         :type OrderSource: str
         :param _DealMode: 交易模式 0-下单并支付 1-下单
         :type DealMode: int
-        :param _ParamTemplateId: 参数模版ID
+        :param _ParamTemplateId: 参数模板ID
         :type ParamTemplateId: int
         :param _InstanceParams: 参数列表，ParamTemplateId 传入时InstanceParams才有效
         :type InstanceParams: list of ModifyParamItem
         :param _SecurityGroupIds: 安全组ID，新建只读实例时可以指定安全组。
         :type SecurityGroupIds: list of str
         """
         self._ClusterId = None
@@ -3670,21 +3670,21 @@
 class CreateParamTemplateRequest(AbstractModel):
     """CreateParamTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateName: 模版名称
+        :param _TemplateName: 模板名称
         :type TemplateName: str
         :param _EngineVersion: mysql版本号
         :type EngineVersion: str
-        :param _TemplateDescription: 模版描述
+        :param _TemplateDescription: 模板描述
         :type TemplateDescription: str
-        :param _TemplateId: 可选参数，需要复制的模版ID
+        :param _TemplateId: 可选参数，需要复制的模板ID
         :type TemplateId: int
         :param _DbMode: 数据库类型，可选值：NORMAL（默认值），SERVERLESS
         :type DbMode: str
         :param _ParamList: 参数列表
         :type ParamList: list of ParamItem
         """
         self._TemplateName = None
@@ -3768,15 +3768,15 @@
 class CreateParamTemplateResponse(AbstractModel):
     """CreateParamTemplate返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 模版ID
+        :param _TemplateId: 模板ID
         :type TemplateId: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TemplateId = None
         self._RequestId = None
 
@@ -3815,15 +3815,15 @@
         :type UniqueVpcId: str
         :param _UniqueSubnetId: 私有网络子网ID，默认与集群子网ID保持一致
         :type UniqueSubnetId: str
         :param _ConnectionPoolType: 连接池类型：SessionConnectionPool(会话级别连接池 )
         :type ConnectionPoolType: str
         :param _OpenConnectionPool: 是否开启连接池,yes-开启，no-不开启
         :type OpenConnectionPool: str
-        :param _ConnectionPoolTimeOut: 连接池阀值：单位（秒）
+        :param _ConnectionPoolTimeOut: 连接池阈值：单位（秒）
         :type ConnectionPoolTimeOut: int
         :param _SecurityGroupIds: 安全组ID数组
         :type SecurityGroupIds: list of str
         :param _Description: 描述说明
         :type Description: str
         :param _Vip: vip信息
         :type Vip: str
@@ -4128,15 +4128,15 @@
         :type UniqueSubnetId: str
         :param _ProxyCount: 数据库代理组节点个数
         :type ProxyCount: int
         :param _ConnectionPoolType: 连接池类型：SessionConnectionPool(会话级别连接池 )
         :type ConnectionPoolType: str
         :param _OpenConnectionPool: 是否开启连接池,yes-开启，no-不开启
         :type OpenConnectionPool: str
-        :param _ConnectionPoolTimeOut: 连接池阀值：单位（秒）
+        :param _ConnectionPoolTimeOut: 连接池阈值：单位（秒）
         :type ConnectionPoolTimeOut: int
         :param _SecurityGroupIds: 安全组ID数组
         :type SecurityGroupIds: list of str
         :param _Description: 描述说明
         :type Description: str
         :param _ProxyZones: 数据库节点信息
         :type ProxyZones: list of ProxyZone
@@ -7893,15 +7893,15 @@
 class DeleteParamTemplateRequest(AbstractModel):
     """DeleteParamTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 参数模版ID
+        :param _TemplateId: 参数模板ID
         :type TemplateId: int
         """
         self._TemplateId = None
 
     @property
     def TemplateId(self):
         return self._TemplateId
@@ -11648,27 +11648,27 @@
 
     """
 
     def __init__(self):
         r"""
         :param _EngineVersions: 数据库引擎版本号
         :type EngineVersions: list of str
-        :param _TemplateNames: 模版名称
+        :param _TemplateNames: 模板名称
         :type TemplateNames: list of str
-        :param _TemplateIds: 模版ID
+        :param _TemplateIds: 模板ID
         :type TemplateIds: list of int
         :param _DbModes: 数据库类型，可选值：NORMAL，SERVERLESS
         :type DbModes: list of str
         :param _Offset: 查询偏移量
         :type Offset: int
         :param _Limit: 查询限制条数
         :type Limit: int
         :param _Products: 查询的模板对应的产品类型
         :type Products: list of str
-        :param _TemplateTypes: 模版类型
+        :param _TemplateTypes: 模板类型
         :type TemplateTypes: list of str
         :param _EngineTypes: 版本类型
         :type EngineTypes: list of str
         :param _OrderBy: 返回结果的排序字段
         :type OrderBy: str
         :param _OrderDirection: 排序方式（asc、desc）
         :type OrderDirection: str
@@ -16970,19 +16970,19 @@
 class ModifyParamTemplateRequest(AbstractModel):
     """ModifyParamTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 模版ID
+        :param _TemplateId: 模板ID
         :type TemplateId: int
-        :param _TemplateName: 模版名
+        :param _TemplateName: 模板名
         :type TemplateName: str
-        :param _TemplateDescription: 模版描述
+        :param _TemplateDescription: 模板描述
         :type TemplateDescription: str
         :param _ParamList: 参数列表
         :type ParamList: list of ModifyParamItem
         """
         self._TemplateId = None
         self._TemplateName = None
         self._TemplateDescription = None
@@ -19883,15 +19883,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Action: 策略，ACCEPT或者DROP
         :type Action: str
-        :param _CidrIp: 来源Ip或Ip段，例如192.168.0.0/16
+        :param _CidrIp: 来源IP或IP段，例如192.168.0.0/16
         :type CidrIp: str
         :param _PortRange: 端口
         :type PortRange: str
         :param _IpProtocol: 网络协议，支持udp、tcp等
         :type IpProtocol: str
         :param _ServiceModule: 协议端口ID或者协议端口组ID。
         :type ServiceModule: str
@@ -20004,15 +20004,15 @@
         r"""
         :param _ConnectionPoolTimeOut: 连接池保持阈值：单位（秒）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ConnectionPoolTimeOut: int
         :param _OpenConnectionPool: 是否开启了连接池
 注意：此字段可能返回 null，表示取不到有效值。
         :type OpenConnectionPool: str
-        :param _ConnectionPoolType: 连接池类型：SessionConnectionPool（会话级别连接池
+        :param _ConnectionPoolType: 连接池类型：SessionConnectionPool（会话级别连接池）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ConnectionPoolType: str
         """
         self._ConnectionPoolTimeOut = None
         self._OpenConnectionPool = None
         self._ConnectionPoolType = None
 
@@ -22660,15 +22660,15 @@
         :type Database: str
         :param _LockTime: 锁时长，单位秒
         :type LockTime: float
         :param _RowsExamined: 扫描行数
         :type RowsExamined: int
         :param _RowsSent: 返回行数
         :type RowsSent: int
-        :param _SqlTemplate: sql模版
+        :param _SqlTemplate: sql模板
         :type SqlTemplate: str
         :param _SqlMd5: sql语句md5
         :type SqlMd5: str
         """
         self._Timestamp = None
         self._QueryTime = None
         self._SqlText = None
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.931/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

