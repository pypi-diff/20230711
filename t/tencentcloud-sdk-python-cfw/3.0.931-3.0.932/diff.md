# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.931.tar", last modified: Mon Jul 10 00:33:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.932.tar", last modified: Tue Jul 11 00:33:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.931.tar` & `tencentcloud-sdk-python-cfw-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   356341 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67446 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:33:16.000000 tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   356341 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67446 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:33:39.000000 tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/setup.py` & `tencentcloud-sdk-python-cfw-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/README.rst` & `tencentcloud-sdk-python-cfw-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.932/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.932/tencentcloud/__init__.py`

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

