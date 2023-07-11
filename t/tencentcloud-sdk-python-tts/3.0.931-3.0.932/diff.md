# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.931.tar", last modified: Mon Jul 10 00:56:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.932.tar", last modified: Tue Jul 11 01:03:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.931.tar` & `tencentcloud-sdk-python-tts-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:56:03.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23530 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:56:02.000000 tencentcloud-sdk-python-tts-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23658 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:03:51.000000 tencentcloud-sdk-python-tts-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-tts-3.0.931/setup.py` & `tencentcloud-sdk-python-tts-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.932/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.931/README.rst` & `tencentcloud-sdk-python-tts-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.931/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.932/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -510,15 +510,18 @@
         :type ProjectId: int
         :param _ModelType: 模型类型，1-默认模型。
         :type ModelType: int
         :param _VoiceType: 音色 ID，包括标准音色与精品音色，精品音色拟真度更高，价格不同于标准音色，请参见[购买指南](https://cloud.tencent.com/document/product/1073/34112)。完整的音色 ID 列表请参见[音色列表](https://cloud.tencent.com/document/product/1073/92668)。
         :type VoiceType: int
         :param _PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li>
         :type PrimaryLanguage: int
-        :param _SampleRate: 音频采样率：<li>16000：16k（默认）</li><li>8000：8k</li>
+        :param _SampleRate: 音频采样率：
+<li>24000：24k（部分音色支持，请参见[音色列表](https://cloud.tencent.com/document/product/1073/92668)）</li>
+<li>16000：16k（默认）</li>
+<li>8000：8k</li>
         :type SampleRate: int
         :param _Codec: 返回音频格式，可取值：wav（默认），mp3，pcm
         :type Codec: str
         :param _EnableSubtitle: 是否开启时间戳功能，默认为false。
         :type EnableSubtitle: bool
         :param _SegmentRate: 断句敏感阈值，默认值为：0，取值范围：[0,1,2]。该值越大越不容易断句，模型会更倾向于仅按照标点符号断句。此参数建议不要随意调整，可能会影响合成效果。
         :type SegmentRate: int
```

### Comparing `tencentcloud-sdk-python-tts-3.0.931/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.932/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.932/tencentcloud/__init__.py`

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

