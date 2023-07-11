# Comparing `tmp/google-cloud-video-transcoder-1.9.0.tar.gz` & `tmp/google-cloud-video-transcoder-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-transcoder-1.9.0.tar", last modified: Thu Apr 13 14:17:14 2023, max compression
+gzip compressed data, was "google-cloud-video-transcoder-1.9.1.tar", last modified: Wed Jul  5 15:27:19 2023, max compression
```

## Comparing `google-cloud-video-transcoder-1.9.0.tar` & `google-cloud-video-transcoder-1.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4752 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3809 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/
--rw-rw-r--   0 root         (0)     1003     2310 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/
--rw-rw-r--   0 root         (0)     1003     2120 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    44332 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    55027 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/client.py
--rw-rw-r--   0 root         (0)     1003    10757 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8996 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19710 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20116 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    45416 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/
--rw-rw-r--   0 root         (0)     1003     1810 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    81436 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003     9069 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/services.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/
--rw-r--r--   0 root         (0)     1003     4752 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1828 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       39 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2985 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   256938 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/test_transcoder_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4752 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3809 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.343568 google-cloud-video-transcoder-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.343568 google-cloud-video-transcoder-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.343568 google-cloud-video-transcoder-1.9.1/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/
+-rw-rw-r--   0 root         (0)     1003     2310 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/
+-rw-rw-r--   0 root         (0)     1003     2120 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44366 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    55027 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10757 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8996 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19710 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20116 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    45416 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.347568 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1810 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81436 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     9069 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/services.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/
+-rw-r--r--   0 root         (0)     1003     4752 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1828 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       39 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:27:19.000000 google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2985 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:27:19.351568 google-cloud-video-transcoder-1.9.1/tests/unit/gapic/transcoder_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/tests/unit/gapic/transcoder_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   257336 2023-07-05 15:24:37.000000 google-cloud-video-transcoder-1.9.1/tests/unit/gapic/transcoder_v1/test_transcoder_service.py
```

### Comparing `google-cloud-video-transcoder-1.9.0/LICENSE` & `google-cloud-video-transcoder-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/MANIFEST.in` & `google-cloud-video-transcoder-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/PKG-INFO` & `google-cloud-video-transcoder-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-transcoder
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Video Transcoder API client library
 Home-page: https://github.com/googleapis/python-video-transcoder
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-transcoder-1.9.0/README.rst` & `google-cloud-video-transcoder-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/gapic_version.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_metadata.json` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_version.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1073,15 +1073,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "TranscoderServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/client.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/__init__.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/resources.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/services.py` & `google-cloud-video-transcoder-1.9.1/google/cloud/video/transcoder_v1/types/services.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/PKG-INFO` & `google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-transcoder
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Video Transcoder API client library
 Home-page: https://github.com/googleapis/python-video-transcoder
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/SOURCES.txt` & `google-cloud-video-transcoder-1.9.1/google_cloud_video_transcoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/setup.py` & `google-cloud-video-transcoder-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/tests/__init__.py` & `google-cloud-video-transcoder-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/tests/unit/__init__.py` & `google-cloud-video-transcoder-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-video-transcoder-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/__init__.py` & `google-cloud-video-transcoder-1.9.1/tests/unit/gapic/transcoder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/test_transcoder_service.py` & `google-cloud-video-transcoder-1.9.1/tests/unit/gapic/transcoder_v1/test_transcoder_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1407,17 +1407,19 @@
                     resources.Job(),
                     resources.Job(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2588,17 +2590,19 @@
                     resources.JobTemplate(),
                     resources.JobTemplate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_job_templates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

