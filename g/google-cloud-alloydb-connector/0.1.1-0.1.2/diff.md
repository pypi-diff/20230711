# Comparing `tmp/google-cloud-alloydb-connector-0.1.1.tar.gz` & `tmp/google-cloud-alloydb-connector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-connector-0.1.1.tar", last modified: Tue Jun 13 16:10:44 2023, max compression
+gzip compressed data, was "google-cloud-alloydb-connector-0.1.2.tar", last modified: Tue Jul 11 18:22:32 2023, max compression
```

## Comparing `google-cloud-alloydb-connector-0.1.1.tar` & `google-cloud-alloydb-connector-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11357 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/LICENSE
--rw-r--r--   0 root         (0)     1003     9258 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     8390 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/google/
--rw-rw-r--   0 root         (0)     1003      746 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/google/cloud/
--rw-rw-r--   0 root         (0)     1003      746 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/
--rw-rw-r--   0 root         (0)     1003      746 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/
--rw-rw-r--   0 root         (0)     1003      803 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     6271 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/client.py
--rw-rw-r--   0 root         (0)     1003     7945 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/connector.py
--rw-rw-r--   0 root         (0)     1003      616 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003     8388 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1970 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003     2764 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     4328 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/refresh.py
--rw-rw-r--   0 root         (0)     1003     2713 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/
--rw-r--r--   0 root         (0)     1003     9258 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      926 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       75 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-13 16:10:44.000000 google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-13 16:10:44.624765 google-cloud-alloydb-connector-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2519 2023-06-13 16:08:27.000000 google-cloud-alloydb-connector-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/
+-rw-rw-r--   0 root         (0)     1003    11357 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/LICENSE
+-rw-r--r--   0 root         (0)     1003     9269 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     8401 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.806615 google-cloud-alloydb-connector-0.1.2/google/
+-rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/
+-rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/
+-rw-rw-r--   0 root         (0)     1003      803 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6271 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/client.py
+-rw-rw-r--   0 root         (0)     1003     7945 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003      616 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     8388 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1970 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003     2764 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     4328 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/refresh.py
+-rw-rw-r--   0 root         (0)     1003     2713 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003     9269 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      926 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       75 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2519 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/setup.py
```

### Comparing `google-cloud-alloydb-connector-0.1.1/LICENSE` & `google-cloud-alloydb-connector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/PKG-INFO` & `google-cloud-alloydb-connector-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -238,19 +238,19 @@
 bug fixes, but do not receive new features. Deprecated versions will be publicly
 supported for 1 year.
 **Unsupported** - Any major version that has been deprecated for >=1 year is
 considered publicly unsupported.
 
 ## Supported Python Versions
 
-We test and support at a minimum, every [active version until it's
-end-of-life date][pyver]. Changes in supported Python versions will be
+We follow the [Python Version Support Policy][pyver] used by Google Cloud
+Libraries for Python. Changes in supported Python versions will be
 considered a minor change, and will be listed in the release notes.
 
-[pyver]: https://devguide.python.org/#status-of-python-branches
+[pyver]: https://cloud.google.com/python/docs/supported-python-versions
 
 ### Release cadence
 
 This project aims for a minimum monthly release cadence. If no new
 features or fixes have been added, a new PATCH version with the latest
 dependencies is released.
```

### Comparing `google-cloud-alloydb-connector-0.1.1/README.md` & `google-cloud-alloydb-connector-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -216,19 +216,19 @@
 bug fixes, but do not receive new features. Deprecated versions will be publicly
 supported for 1 year.
 **Unsupported** - Any major version that has been deprecated for >=1 year is
 considered publicly unsupported.
 
 ## Supported Python Versions
 
-We test and support at a minimum, every [active version until it's
-end-of-life date][pyver]. Changes in supported Python versions will be
+We follow the [Python Version Support Policy][pyver] used by Google Cloud
+Libraries for Python. Changes in supported Python versions will be
 considered a minor change, and will be listed in the release notes.
 
-[pyver]: https://devguide.python.org/#status-of-python-branches
+[pyver]: https://cloud.google.com/python/docs/supported-python-versions
 
 ### Release cadence
 
 This project aims for a minimum monthly release cadence. If no new
 features or fixes have been added, a new PATCH version with the latest
 dependencies is released.
```

### Comparing `google-cloud-alloydb-connector-0.1.1/google/__init__.py` & `google-cloud-alloydb-connector-0.1.2/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/__init__.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/__init__.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/__init__.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/client.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/connector.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/connector.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/exceptions.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/instance.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/pg8000.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/rate_limiter.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/refresh.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/refresh.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/utils.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/google/cloud/alloydb/connector/version.py` & `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/PKG-INFO` & `google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -238,19 +238,19 @@
 bug fixes, but do not receive new features. Deprecated versions will be publicly
 supported for 1 year.
 **Unsupported** - Any major version that has been deprecated for >=1 year is
 considered publicly unsupported.
 
 ## Supported Python Versions
 
-We test and support at a minimum, every [active version until it's
-end-of-life date][pyver]. Changes in supported Python versions will be
+We follow the [Python Version Support Policy][pyver] used by Google Cloud
+Libraries for Python. Changes in supported Python versions will be
 considered a minor change, and will be listed in the release notes.
 
-[pyver]: https://devguide.python.org/#status-of-python-branches
+[pyver]: https://cloud.google.com/python/docs/supported-python-versions
 
 ### Release cadence
 
 This project aims for a minimum monthly release cadence. If no new
 features or fixes have been added, a new PATCH version with the latest
 dependencies is released.
```

### Comparing `google-cloud-alloydb-connector-0.1.1/google_cloud_alloydb_connector.egg-info/SOURCES.txt` & `google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.1/setup.py` & `google-cloud-alloydb-connector-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,13 +65,13 @@
         "Programming Language :: Python :: 3.11",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     namespace_packages=namespaces,
     install_requires=core_dependencies,
     extras_require={
-        "pg8000": ["pg8000==1.29.6"],
+        "pg8000": ["pg8000==1.29.8"],
     },
     python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
 )
```

