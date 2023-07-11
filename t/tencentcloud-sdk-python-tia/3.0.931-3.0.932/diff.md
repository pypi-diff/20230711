# Comparing `tmp/tencentcloud-sdk-python-tia-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-tia-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.931.tar", last modified: Mon Jul 10 00:54:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.932.tar", last modified: Tue Jul 11 01:01:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tia-3.0.931.tar` & `tencentcloud-sdk-python-tia-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/
--rw-r--r--   0 root         (0) root         (0)    10642 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/tia_client.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49879 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:54:19.000000 tencentcloud-sdk-python-tia-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/tia_client.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49879 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:01:51.000000 tencentcloud-sdk-python-tia-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-tia-3.0.931/setup.py` & `tencentcloud-sdk-python-tia-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.931/README.rst` & `tencentcloud-sdk-python-tia-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.931/tencentcloud_sdk_python_tia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.932/tencentcloud_sdk_python_tia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/tia_client.py` & `tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/tia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/errorcodes.py` & `tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.931/tencentcloud/tia/v20180226/models.py` & `tencentcloud-sdk-python-tia-3.0.932/tencentcloud/tia/v20180226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tia-3.0.932/tencentcloud/__init__.py`

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
