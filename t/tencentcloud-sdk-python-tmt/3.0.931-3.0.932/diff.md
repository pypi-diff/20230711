# Comparing `tmp/tencentcloud-sdk-python-tmt-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-tmt-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.931.tar", last modified: Mon Jul 10 00:55:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.932.tar", last modified: Tue Jul 11 01:03:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tmt-3.0.931.tar` & `tencentcloud-sdk-python-tmt-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)     9401 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46724 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:55:16.000000 tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)     9401 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46724 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:03:01.000000 tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.932/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/setup.py` & `tencentcloud-sdk-python-tmt-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.932/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/README.rst` & `tencentcloud-sdk-python-tmt-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tmt-3.0.932/tencentcloud/__init__.py`

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

