# Comparing `tmp/rudi-node-read-0.1.3.tar.gz` & `tmp/rudi-node-read-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudi-node-read-0.1.3.tar", last modified: Thu Apr 20 14:22:59 2023, max compression
+gzip compressed data, was "rudi-node-read-0.1.4.tar", last modified: Tue Jul 11 13:35:58 2023, max compression
```

## Comparing `rudi-node-read-0.1.3.tar` & `rudi-node-read-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.063051 rudi-node-read-0.1.3/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.3/LICENCE.md
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     2068 2023-04-20 14:22:59.062530 rudi-node-read-0.1.3/PKG-INFO
--rw-r--r--   0 omartine (660741) dept-aac (29120)      924 2023-04-20 08:32:38.000000 rudi-node-read-0.1.3/README.md
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1450 2023-04-20 14:22:49.000000 rudi-node-read-0.1.3/pyproject.toml
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-04-20 14:22:59.063189 rudi-node-read-0.1.3/setup.cfg
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.049723 rudi-node-read-0.1.3/src/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.051912 rudi-node-read-0.1.3/src/rudi_node_read/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.055203 rudi-node-read-0.1.3/src/rudi_node_read/connectors/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     5148 2023-04-19 12:30:07.000000 rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_connector.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     3993 2023-04-19 12:57:38.000000 rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_rudi_api.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)    19661 2023-04-19 12:52:26.000000 rudi-node-read-0.1.3/src/rudi_node_read/rudi_node_reader.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.061018 rudi-node-read-0.1.3/src/rudi_node_read/utils/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     2010 2023-04-20 12:06:46.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/err.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      851 2023-04-20 12:31:59.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/jwt.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-04-20 08:56:10.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/log.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      308 2023-04-20 12:40:43.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/serializable.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     5185 2023-04-20 14:19:11.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/type_dict.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1570 2023-04-20 13:26:33.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/type_string.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      829 2023-04-20 14:20:44.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/types.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.054200 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     2068 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/PKG-INFO
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      654 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/SOURCES.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/dependency_links.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       70 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/requires.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/top_level.txt
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.061724 rudi-node-read-0.1.3/tests/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     3171 2023-04-20 09:46:35.000000 rudi-node-read-0.1.3/tests/test_rudi_node_reader.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.590342 rudi-node-read-0.1.4/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.4/LICENCE.md
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-11 13:35:58.590048 rudi-node-read-0.1.4/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      940 2023-07-07 15:06:14.000000 rudi-node-read-0.1.4/README.md
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     1818 2023-07-11 13:35:29.000000 rudi-node-read-0.1.4/pyproject.toml
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-07-11 13:35:58.590448 rudi-node-read-0.1.4/setup.cfg
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.577826 rudi-node-read-0.1.4/src/
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.580221 rudi-node-read-0.1.4/src/rudi_node_read/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)        0 2023-07-07 13:29:00.000000 rudi-node-read-0.1.4/src/rudi_node_read/__init_.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.583363 rudi-node-read-0.1.4/src/rudi_node_read/connectors/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     5302 2023-07-10 15:15:15.000000 rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_connector.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     4137 2023-07-10 14:57:09.000000 rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_rudi_node_read.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    20460 2023-07-10 14:57:04.000000 rudi-node-read-0.1.4/src/rudi_node_read/rudi_node_reader.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.588631 rudi-node-read-0.1.4/src/rudi_node_read/utils/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2115 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/err.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      864 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/jwt.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/log.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      302 2023-07-07 12:48:49.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/serializable.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     5138 2023-07-10 14:58:48.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_dict.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      784 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_misc.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     1631 2023-07-10 14:58:16.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_string.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.582431 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      694 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/SOURCES.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/dependency_links.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       81 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/requires.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/top_level.txt
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.589284 rudi-node-read-0.1.4/tests/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     3171 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/tests/test_rudi_node_reader.py
```

### Comparing `rudi-node-read-0.1.3/LICENCE.md` & `rudi-node-read-0.1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.3/PKG-INFO` & `rudi-node-read-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
-Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
-Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
-Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
-Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/OlivierMartineau/rudi-node-read
+Project-URL: Documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
+Project-URL: Changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
+Project-URL: Source, https://github.com/OlivierMartineau/rudi-node-read
+Keywords: rudi-node-read,rudi-node-get,RUDI,producer node,RUDI node,rudinode,open-data,Univ. Rennes
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: packaging
 Provides-Extra: tests
 License-File: LICENCE.md
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
 The Jupyter notebook [README.ipynb](https://github.com/OlivierMartineau/rudi-node-read/blob/release/README.ipynb) offers
@@ -46,15 +48,13 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+
 ## Testing
 
 ```bash
-pip install pytest-cov
-
-python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+$ pytest
 ```
-
```

### Comparing `rudi-node-read-0.1.3/README.md` & `rudi-node-read-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
 The Jupyter notebook [README.ipynb](https://github.com/OlivierMartineau/rudi-node-read/blob/release/README.ipynb) offers
@@ -21,15 +23,13 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+
 ## Testing
 
 ```bash
-pip install pytest-cov
-
-python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+$ pytest
 ```
-
```

### Comparing `rudi-node-read-0.1.3/pyproject.toml` & `rudi-node-read-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudi-node-read"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Olivier Martineau", email = "olivier.martineau@irisa.fr" }]
 maintainers = [{ name = "Olivier Martineau", email = "olivier.martineau@irisa.fr" }]
 description = "Use the external API of a RUDI Producer node"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "EUPL-1.2" }
-classifiers = ["Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
+classifiers = ["Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
 ]
-keywords = ["RUDI", "producer node", "RUDI node", "open-data", "Univ. Rennes"]
+keywords = ["rudi-node-read", "rudi-node-get",
+    "RUDI", "producer node",
+    "RUDI node", "rudinode",
+    "open-data", "Univ. Rennes"]
 
 [project.urls]
-repository = "https://github.com/OlivierMartineau/rudi-node-read"
-documentation = "https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER"
-changelog = "https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md"
+Homepage = "https://github.com/OlivierMartineau/rudi-node-read"
+Documentation = "https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER"
+Changelog = "https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md"
+Source = "https://github.com/OlivierMartineau/rudi-node-read"
 
 [project.optional-dependencies]
-packaging = ["build", "twine", "pip-chill", "pip-autoremove"]
+packaging = ["build", "commitizen", "pip-autoremove", "pip-chill", "twine"]
 tests = ["pytest-cov"]
 
+[tool.black]
+line-length = 120
+target-version = ['py311']
+
 [tool.pytest.ini_options]
+pythonpath = ["src"]
 norecursedirs = ["*.egg", ".eggs", "dist", "build"]
+addopts = ["--cov=rudi_node_read", "--cov-report=term-missing", "--cov-report=html"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
+
 include = ["rudi_node_read*"]
 
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "0.1.4"
+version_files = ["pyproject.toml:version"]
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_connector.py` & `rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,119 +4,136 @@
 from urllib.parse import urlsplit
 
 from rudi_node_read.utils.err import HttpError, LiteralUnexpectedValueException
 from rudi_node_read.utils.log import log_d_if, log_e, log_d
 from rudi_node_read.utils.serializable import Serializable
 from rudi_node_read.utils.type_string import slash_join
 
-HttpRequestMethod = Literal['GET', 'PUT', 'DEL', 'POST']
-http_request_methods = get_args(HttpRequestMethod)
+HttpRequestMethod = Literal["GET", "PUT", "DEL", "POST"]
+HTTP_REQUEST_METHODS = get_args(HttpRequestMethod)
 
 
 def https_download(resource_url: str, should_show_debug_line: bool = False):
-    fun = 'https_download'
+    fun = "https_download"
     (scheme, netloc, path, query, fragment) = urlsplit(resource_url)
-    if scheme != 'https':
-        raise NotImplementedError('only HTTPS protocol is supported')
+    if scheme != "https":
+        raise NotImplementedError("only HTTPS protocol is supported")
     connection = HTTPSConnection(netloc)
-    connection.request(method='GET', url=resource_url)
+    connection.request(method="GET", url=resource_url)
     response = connection.getresponse()
     if response.status != 200:
-        log_e(fun, f'ERR {response.status}', resource_url)
+        log_e(fun, f"ERR {response.status}", resource_url)
         return None
     else:
-        log_d_if(should_show_debug_line, fun, f'OK {response.status}', resource_url)
+        log_d_if(should_show_debug_line, fun, f"OK {response.status}", resource_url)
         data = response.read()
         # log_d('https_download', 'data', data)
         connection.close()
         return data
 
 
 class Connector(Serializable):
     _default_connector = None
 
     def __init__(self, server_url: str):
         (scheme, netloc, path, query, fragment) = urlsplit(server_url)
-        if scheme != 'http' and scheme != 'https':
-            raise NotImplementedError('only http and https are supported')
+        if scheme != "http" and scheme != "https":
+            raise NotImplementedError("only http and https are supported")
         self.scheme = scheme
         self.host = netloc
         self.path = path
         self.base_url = slash_join(f"{self.scheme}://{self.host}", self.path)
 
-        log_d('Connector', 'base_url', self.base_url)
+        log_d("Connector", "base_url", self.base_url)
 
-    def full_url(self, url: str = '/'):
+    def full_url(self, url: str = "/"):
         return slash_join(self.base_url, url)
 
-    def full_path(self, url: str = '/'):
-        return slash_join('/', self.path, url)
+    def full_path(self, url: str = "/"):
+        return slash_join("/", self.path, url)
 
-    def request(self, url: str = '/', req_method: HttpRequestMethod = 'GET', body: object = None,
-                headers: object = None, should_log_response: bool = False) -> (str, object):
-        """ Send a http(obj) request
-        """
-        if self.scheme == 'https':
-            connection = HTTPSConnection(self.host)
-        else:
-            connection = HTTPConnection(self.host)
-        if req_method not in http_request_methods:
-            raise LiteralUnexpectedValueException('incorrect type for request method', HttpRequestMethod, req_method)
+    def request(
+        self,
+        url: str = "/",
+        req_method: HttpRequestMethod = "GET",
+        body: dict = None,
+        headers: dict = None,
+        should_log_response: bool = False,
+    ) -> (str, dict):
+        """Send a http(obj) request"""
+
+        connection = HTTPSConnection(self.host) if self.scheme == "https" else HTTPConnection(self.host)
+        if req_method not in HTTP_REQUEST_METHODS:
+            raise LiteralUnexpectedValueException(req_method, HTTP_REQUEST_METHODS, "incorrect type for request method")
 
         if not headers:
-            headers = {'Content-Type': 'text/plain', 'Accept': 'application/json'}
+            headers = {"Content-Type": "text/plain", "Accept": "application/json"}
         if body and type(body) == dict:
-            headers['Content-type'] = 'application/json'
+            headers["Content-type"] = "application/json"
             body = dumps(body)
 
         path_url = self.full_path(url)
-        log_d(f'{self.__class__.__name__}.request', 'to', self.full_url(url))
+        log_d(f"{self.__class__.__name__}.request", "to", self.full_url(url))
         try:
             connection.request(req_method, path_url, body, headers)
         except ConnectionRefusedError as e:
-            log_e(self.__class__.__name__, 'Error on request', req_method, self.full_url(url))
-            log_e(self.__class__.__name__, 'ERR', e)
+            log_e(
+                self.__class__.__name__,
+                "Error on request",
+                req_method,
+                self.full_url(url),
+            )
+            log_e(self.__class__.__name__, "ERR", e)
             raise e
         return self.parse_response(connection, url, req_method, headers, body, should_log_response)
 
-    def parse_response(self, connection: HTTPConnection, url, req_method, headers, body,
-                       should_log_response: bool = True):
-        """ Basic parsing of the result
-        """
-        fun = f'{self.__class__.__name__}.parse_response'
+    def parse_response(
+        self,
+        connection: HTTPConnection,
+        url: str,
+        req_method: HttpRequestMethod,
+        headers: dict,
+        body: dict,
+        should_log_response: bool = True,
+    ):
+        """Basic parsing of the result"""
+        fun = f"{self.__class__.__name__}.parse_response"
         response = connection.getresponse()
-        if response.status not in [200, 500, 501] and not (530 <= response.status < 540) and not (
-                400 <= response.status < 500):
+        if (
+            response.status not in [200, 500, 501]
+            and not (530 <= response.status < 540)
+            and not (400 <= response.status < 500)
+        ):
             return None
 
         rdata = response.read()
         try:
             response_data = loads(rdata)
-            log_d_if(should_log_response, fun, 'Response is a JSON', response_data)
-        except (TypeError, JSONDecodeError) as e:
+            log_d_if(should_log_response, fun, "Response is a JSON", response_data)
+        except (TypeError, JSONDecodeError):
             response_data = repr(rdata)
-            log_d_if(should_log_response, fun, 'Response is not a JSON', response_data)
+            log_d_if(should_log_response, fun, "Response is not a JSON", response_data)
         connection.close()
         if type(response_data) is str:
-            log_d_if(should_log_response, fun, 'Response is a string', response_data)
+            log_d_if(should_log_response, fun, "Response is a string", response_data)
             if response.status == 200:
-                return rdata.decode('utf8')
+                return rdata.decode("utf8")
         if response.status == 200:
             return response_data
         if response.status >= 400:
-            log_e(fun, 'Connection error', response_data)
-            log_e(fun, 'Request in error', req_method, self.full_url(url))
+            log_e(fun, "Connection error", response_data)
+            log_e(fun, "Request in error", req_method, self.full_url(url))
             raise HttpError(response_data, req_method, self.base_url, url)
 
 
-if __name__ == '__main__':
-    if 'GET' in HttpRequestMethod:
-        log_d('Testing Literal', 'GET in HttpRequestMethod', 'OK')
+if __name__ == "__main__":
+    if "GET" in HTTP_REQUEST_METHODS:
+        log_d("Testing Literal", "GET in HttpRequestMethod", "OK")
     else:
-        log_d('Testing Literal', 'GET in HttpRequestMethod', 'KO')
+        log_d("Testing Literal", "GET in HttpRequestMethod", "KO")
 
-    connector = Connector('https://data-rudi.aqmo.org/api/v1')
-    data = connector.request(url='resources?limit=1')
+    connector = Connector("https://data-rudi.aqmo.org/api/v1")
+    data = connector.request(url="resources?limit=1")
     print(data)
 
-    url = 'https://bacasable.fenix.rudi-univ-rennes1.fr/media/download/b086c7b2-bd6d-401f-86f5-f1f207023bae'
-    log_d('https_utils', url, https_download(url))
+    url = "https://bacasable.fenix.rudi-univ-rennes1.fr/media/download/b086c7b2-bd6d-401f-86f5-f1f207023bae"
+    log_d("https_utils", url, https_download(url))
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_rudi_api.py` & `rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_rudi_node_read.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,92 +2,99 @@
 from rudi_node_read.utils.log import log_d, log_e
 from rudi_node_read.utils.type_string import slash_join
 
 REQ_LIMIT = 500
 
 
 class RudiNodeConnector(Connector):
-
-    def __init__(self, server_url: str, headers_user_agent: str = 'RudiNodeConnector'):
+    def __init__(self, server_url: str, headers_user_agent: str = "RudiNodeConnector"):
         """
         Creates a connector to the API/proxy module of a RUDI Node
         :param server_url: the URL of the RUDI Node
         :param headers_user_agent: (optional) identifies the user launching the request (or at least the module)
         in the request headers, for logging purpose.
         """
 
         super().__init__(server_url)
 
-        log_d('RudiNodeConnector', 'attributes', self)
+        log_d("RudiNodeConnector", "attributes", self)
         self.test_rudi_api_connection()
-        self._headers = {'User-Agent': headers_user_agent}
+        self._headers = {
+            "User-Agent": headers_user_agent,
+            "Content-type": "text/plain",
+            "Accept": "application/json",
+        }
 
     def get_api(self, url: str):
         """
         Performs an identified GET request through /api/v1 path
         :param url: part of the URL that comes after /api/admin
         :return: a JSON
         """
-        return self.request(url=slash_join('api/v1', url), req_method='GET',
-                            headers={'Content-type': 'text/plain', 'Accept': 'application/json'})
+        return self.request(url=slash_join("api/v1", url), req_method="GET", headers=self._headers)
 
     def test_rudi_api_connection(self):
-        test = self.request('api/admin/hash')
+        test = self.request("api/admin/hash")
         if test is None:
-            log_e('RudiNodeConnector', f"!! Node '{self.host}'", 'no connection!')
+            log_e("RudiNodeConnector", f"!! Node '{self.host}'", "no connection!")
         else:
-            log_d('RudiNodeConnector', f"Node '{self.host}'", 'connection OK')
+            log_d("RudiNodeConnector", f"Node '{self.host}'", "connection OK")
 
     def get_metadata_with_uuid(self, metadata_uuid: str):
-        return self.get_api(f'resources/{metadata_uuid}')
+        return self.get_api(f"resources/{metadata_uuid}")
 
     def get_metadata_with_filter(self, rudi_fields_filter: dict):
-        filter_str = ''
-        for i, (key, val) in rudi_fields_filter:
+        filter_str = ""
+        for i, (key, val) in enumerate(rudi_fields_filter.items()):
             # TODO: special cases of producer / contact / available_formats
-            filter_str += f'&{key}={val}'
+            filter_str += f"&{key}={val}"
 
-        return self.get_api(f'resources?{filter_str[2:]}')
+        return self.get_api(f"resources?{filter_str[1:]}")
 
     def get_metadata_count(self):
-        return self.get_api(f'resources?limit=1')['total']
+        return self.get_api("resources?limit=1")["total"]
 
     def get_metadata_list(self, max_number: int = 0):
         meta_nb = self.get_metadata_count()
         meta_set = []
         req_offset = 0
         if not max_number:
             max_number = meta_nb
         while req_offset < meta_nb and req_offset < max_number:
             req_limit = REQ_LIMIT if req_offset + REQ_LIMIT < max_number else max_number - req_offset
-            meta_list_partial = self.get_api(f'resources?sort_by=-updatedAt&limit={req_limit}&offset={req_offset}')
-            log_d('get_metadata_list', 'total', meta_list_partial['total'])
-            log_d('get_metadata_list', 'len', len(meta_list_partial['items']))
-            meta_set += meta_list_partial['items']
+            meta_list_partial = self.get_api(f"resources?sort_by=-updatedAt&limit={req_limit}&offset={req_offset}")
+            log_d("get_metadata_list", "total", meta_list_partial["total"])
+            log_d("get_metadata_list", "len", len(meta_list_partial["items"]))
+            meta_set += meta_list_partial["items"]
             req_offset += REQ_LIMIT
         return meta_set
 
     def get_metadata_ids(self):
-        meta_list = self.get_api('resources?fields=global_id,resource_title')
-        return meta_list['items']
+        meta_list = self.get_api("resources?fields=global_id,resource_title")
+        return meta_list["items"]
 
     def get_list_media_for_metadata(self, metadata_uuid):
         meta = self.get_metadata_with_uuid(metadata_uuid)
-        media_list = meta['available_formats']
+        media_list = meta["available_formats"]
         media_list_final = []
         for media in media_list:
             media_list_final.append(
-                {'url': media['connector']['url'], 'type': media['media_type'], 'meta_contact': media['media_id'],
-                 'id': media['media_id']})
+                {
+                    "url": media["connector"]["url"],
+                    "type": media["media_type"],
+                    "meta_contact": media["media_id"],
+                    "id": media["media_id"],
+                }
+            )
         return media_list_final
 
 
-if __name__ == '__main__':
-    rudi_node_connector = RudiNodeConnector('https://bacasable.fenix.rudi-univ-rennes1.fr')
-    log_d('RudiNodeConnector', 'metadata nb', rudi_node_connector.get_metadata_count())
-    log_d('RudiNodeConnector', 'metadata_ids', rudi_node_connector.get_metadata_ids())
+if __name__ == "__main__":
+    rudi_node_connector = RudiNodeConnector("https://bacasable.fenix.rudi-univ-rennes1.fr")
+    log_d("RudiNodeConnector", "metadata nb", rudi_node_connector.get_metadata_count())
+    log_d("RudiNodeConnector", "metadata_ids", rudi_node_connector.get_metadata_ids())
     meta1 = rudi_node_connector.get_metadata_list()[1]
-    meta1_id = meta1['global_id']
+    meta1_id = meta1["global_id"]
     rudi_node_connector.get_metadata_with_uuid(meta1_id)
-    log_d('RudiNodeConnector', 'meta1', meta1_id)
+    log_d("RudiNodeConnector", "meta1", meta1_id)
     meta1_media = rudi_node_connector.get_list_media_for_metadata(meta1_id)
-    log_d('RudiNodeConnector', 'meta1 media', meta1_media)
+    log_d("RudiNodeConnector", "meta1 media", meta1_media)
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/rudi_node_reader.py` & `rudi-node-read-0.1.4/src/rudi_node_read/rudi_node_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from json import dumps
 from os.path import isdir, abspath
-from typing import Union, Optional
+from typing import Union
 
 from rudi_node_read.connectors.io_connector import https_download
-from rudi_node_read.connectors.io_rudi_api import RudiNodeConnector
+from rudi_node_read.connectors.io_rudi_node_read import RudiNodeConnector
 from rudi_node_read.utils.log import log_d
-from rudi_node_read.utils.type_dict import safe_get_key, find_in_dict_list, filter_dict_list, pick_in_dict
+from rudi_node_read.utils.type_dict import (
+    safe_get_key,
+    find_in_dict_list,
+    filter_dict_list,
+    pick_in_dict,
+)
 from rudi_node_read.utils.type_string import slash_join
 
-_STATUS_SKIPPED = 'skipped'
-_STATUS_MISSING = 'missing'
-_STATUS_DOWNLOADED = 'downloaded'
+_STATUS_SKIPPED = "skipped"
+_STATUS_MISSING = "missing"
+_STATUS_DOWNLOADED = "downloaded"
 
 
 class RudiNodeReader:
     _default_getter = None
 
-    def __init__(self, server_url: str, headers_user_agent: str = 'RudiNodeGet'):
+    def __init__(self, server_url: str, headers_user_agent: str = "RudiNodeReader"):
         self._server_url = server_url
         self._headers_user_agent = headers_user_agent
 
         self._connector = None
 
         self._meta_list = None
         self._meta_list_available = None
@@ -58,15 +63,15 @@
         """
         :return: the RudiNodeConnector object used for requesting the RUDI node
         """
         if not self._connector:
             self._connector = RudiNodeConnector(self._server_url, self._headers_user_agent)
         return self._connector
 
-    def connect(self, server_url: str, headers_user_agent: str = 'RudiNodeGet') -> None:
+    def connect(self, server_url: str, headers_user_agent: str = "RudiNodeGet") -> None:
         """
         Reinitialize the connection to a RUDI node
         :param server_url: the URL of the RUDI node
         :param headers_user_agent: (optional) a way to identify the requests made to the node
         """
         self._server_url = server_url
         self._headers_user_agent = headers_user_agent
@@ -97,27 +102,27 @@
         """
         :return: the list of the organizations that appear in the metadata
         (both data producer and metadata publisher)
         """
         if not self._org_list:
             self._org_list = []
             for meta in self.metadata_list:
-                producer_info = safe_get_key(meta, 'producer')
-                publisher_info = safe_get_key(meta, 'metadata_info', 'metadata_provider')
+                producer_info = safe_get_key(meta, "producer")
+                publisher_info = safe_get_key(meta, "metadata_info", "metadata_provider")
 
-                producer_id = safe_get_key(producer_info, 'organization_id')
+                producer_id = safe_get_key(producer_info, "organization_id")
                 was_producer_found = not producer_id
 
-                publisher_id = safe_get_key(publisher_info, 'organization_id')
+                publisher_id = safe_get_key(publisher_info, "organization_id")
                 was_publisher_found = not publisher_id or publisher_id == producer_id
 
                 for org in self._org_list:
                     if was_producer_found and was_publisher_found:
                         break
-                    org_id = safe_get_key(org, 'organization_id')
+                    org_id = safe_get_key(org, "organization_id")
                     if not was_producer_found and org_id == producer_id:
                         was_producer_found = True
                     if not was_publisher_found and org_id == publisher_id:
                         was_publisher_found = True
 
                 if not was_producer_found:
                     self._org_list.append(producer_info)
@@ -131,75 +136,75 @@
         """
         :return: the list of the names of the organizations that appear in the metadata
         (both data producer and metadata publisher)
         """
         if not self._org_names:
             self._org_names = []
             for org in self.organization_list:
-                self._org_names.append(safe_get_key(org, 'organization_name'))
+                self._org_names.append(safe_get_key(org, "organization_name"))
         self._org_names.sort()
         return self._org_names
 
     @property
     def contact_list(self) -> list[dict]:
         """
         :return: the list of the contacts declared in the RUDI node metadata
         """
         if not self._contact_list:
             self._contact_list = []
             for meta in self.metadata_list:
-                meta_contacts = safe_get_key(meta, 'contacts')
-                publ_contacts = safe_get_key(meta, 'metadata_info', 'metadata_contacts')
+                meta_contacts = safe_get_key(meta, "contacts")
+                publ_contacts = safe_get_key(meta, "metadata_info", "metadata_contacts")
                 if publ_contacts:
                     meta_contacts = meta_contacts + publ_contacts
 
                 if meta_contacts:
                     for prod_contact in meta_contacts:
-                        prod_contact_id = safe_get_key(prod_contact, 'contact_id')
+                        prod_contact_id = safe_get_key(prod_contact, "contact_id")
                         if prod_contact_id:
-                            if not find_in_dict_list(self._contact_list, {'contact_id': prod_contact_id}):
+                            if not find_in_dict_list(self._contact_list, {"contact_id": prod_contact_id}):
                                 self._contact_list.append(prod_contact)
 
         return self._contact_list
 
     @property
     def contact_names(self) -> list[str]:
         """
         :return: the list of the names of the contacts declared in the RUDI node metadata
         """
         if not self._contact_names:
             self._contact_names = []
             for contact in self.contact_list:
-                self._contact_names.append(safe_get_key(contact, 'contact_name'))
+                self._contact_names.append(safe_get_key(contact, "contact_name"))
         self._contact_names.sort()
         return self._contact_names
 
     @property
     def themes(self) -> list[str]:
         """
         :return: the list of the themes declared in the RUDI node metadata
         """
-        if not self._themes:
+        if self._themes is None:
             self._themes = []
             for meta in self.metadata_list:
-                theme = safe_get_key(meta, 'theme')
+                theme = safe_get_key(meta, "theme")
                 if theme and theme not in self._themes:
                     self._themes.append(theme)
         self._themes.sort()
         return self._themes
 
     @property
     def keywords(self) -> list[str]:
         """
         :return: the list of the keywords declared in the RUDI node metadata
         """
-        if not self._keywords:
+        if self._keywords is None:
             self._keywords = []
             for meta in self.metadata_list:
-                keywords = safe_get_key(meta, 'keywords')
+                keywords = safe_get_key(meta, "keywords")
                 if keywords:
                     for kword in keywords:
                         if kword not in self._keywords:
                             self._keywords.append(kword)
         self._keywords.sort()
         return self._keywords
 
@@ -208,241 +213,318 @@
         Returns an object with the following attributes:
         - total: the number of metadata that match the filter
         - items: the list of the metadata that match the filter
         :param matching_filter: JSON-like object whose attributes are all matched in the resulting
         metadata list
         :return: list of the metadata that match the filter
         """
-        '''
-        items = filter_dict_list(self.metadata_list, matching_filter)    
-        total = len(items)   
+        """
+        items = filter_dict_list(self.metadata_list, matching_filter)
+        total = len(items)
         return {'total': total, 'items': items}
-        '''
+        """
         return filter_dict_list(self.metadata_list, matching_filter)
 
     @property
     def metadata_with_available_media(self) -> list[dict]:
         """
         :return: list of the metadata whose `available_data` attribute contains at least one media for which
         `file_storage_status`attribute is set to `available`
         """
-        if not self._meta_list_available:
+        if self._meta_list_available is None:
             self._meta_list_available = self.filter_metadata(
-                {'available_formats': [{'file_storage_status': 'available'}]})
+                {"available_formats": [{"file_storage_status": "available"}]}
+            )
         return self._meta_list_available
 
     def get_metadata_with_producer(self, producer_name: str) -> list[dict]:
         """
         :param producer_name: the meta_contact of the organization declared in the metadata
         :return: list of the metadata whose `producer.organization_name` attribute matches the `producer_name` input
         parameter
         """
-        return self.filter_metadata({'producer': {'organization_name': producer_name}})
+        return self.filter_metadata({"producer": {"organization_name": producer_name}})
 
     def get_metadata_with_contact(self, contact_name: str) -> list[dict]:
         """
         :param contact_name: the meta_contact of the contact declared in the metadata
         :return: list of the metadata whose `contacts` attribute contains a contact object whose `contact_name`
         attribute matches the `contact_name` input parameter
         """
-        return self.filter_metadata({'contacts': [{'contact_name': contact_name}]})
+        return self.filter_metadata({"contacts": [{"contact_name": contact_name}]})
 
     def get_metadata_with_theme(self, theme: str) -> list[dict]:
         """
         :param theme: a string used to filter the metadata by theme
         :return: list of the metadata whose `theme` attribute matches the `theme` input parameter
         """
-        return self.filter_metadata({'theme': theme})
+        return self.filter_metadata({"theme": theme})
 
     def get_metadata_with_keywords(self, keywords: Union[str, list]) -> list[dict]:
         """
         :param keywords: a string or a list of strings used to filter the metadata by keywords
         :return: list of the metadata whose `keywords` attribute contains every `keywords` input parameter
         """
-        return self.filter_metadata({'keywords': keywords})
+        return self.filter_metadata({"keywords": keywords})
 
-    def find_metadata_with_uuid(self, metadata_id: str) -> Optional[dict]:
+    def find_metadata_with_uuid(self, metadata_id: str) -> dict | None:
         """
         :param metadata_id: a UUIDv4 string
         :return: metadata whose `global_id` attribute matches the `metadata_id` input parameter
         """
-        return find_in_dict_list(self.metadata_list, {'global_id': metadata_id})
+        return find_in_dict_list(self.metadata_list, {"global_id": metadata_id})
 
-    def find_metadata_with_source_id(self, source_id: str) -> Optional[dict]:
+    def find_metadata_with_source_id(self, source_id: str) -> dict | None:
         """
         :param source_id: a string that was used in the producer data source to identify the dataset
         :return: metadata whose `local_id` attribute matches the `media_name` input parameter
         """
-        return find_in_dict_list(self.metadata_list, {'local_id': source_id})
+        return find_in_dict_list(self.metadata_list, {"local_id": source_id})
 
-    def find_metadata_with_title(self, title: str) -> Optional[dict]:
+    def find_metadata_with_title(self, title: str) -> dict | None:
         """
         :param title: media_name of the metadata
         :return: metadata whose `resource_title` attribute matches the `media_name` input parameter
         """
-        return find_in_dict_list(self.metadata_list, {'resource_title': title})
+        return find_in_dict_list(self.metadata_list, {"resource_title": title})
 
-    def find_metadata_with_media_name(self, media_name: str) -> Optional[dict]:
+    def find_metadata_with_media_name(self, media_name: str) -> dict | None:
         """
         :param media_name: meta_contact of the media
         :return: metadata whose `resource_title` attribute matches the `title` input parameter
         """
-        return find_in_dict_list(self.metadata_list, {'available_formats': [{'media_name': media_name}]})
+        return find_in_dict_list(self.metadata_list, {"available_formats": [{"media_name": media_name}]})
 
-    def find_metadata_with_media_uuid(self, media_uuid: str) -> Optional[dict]:
+    def find_metadata_with_media_uuid(self, media_uuid: str) -> dict | None:
         """
         :param media_uuid: UUIDv4 of the media
         :return: metadata whose `resource_title` attribute matches the `title` input parameter
         """
-        return find_in_dict_list(self.metadata_list, {'available_formats': [{'media_id': media_uuid}]})
+        return find_in_dict_list(self.metadata_list, {"available_formats": [{"media_id": media_uuid}]})
 
     @staticmethod
     def _download_media_from_info(media: dict, local_download_dir: str) -> dict:
         """
         Download a file from its media metadata
         :param media: the file metadata (as found in the RUDI metadata `available_formats` attribute
         :param local_download_dir: the path to a local folder
         :return: an object that states if the file was downloaded, skipped or found missing
         """
         # fun = '_download_media_from_info'
 
-        media_type = safe_get_key(media, 'media_type')
+        media_type = safe_get_key(media, "media_type")
 
         # Most likely for media_type == 'SERVICE'
-        if media_type != 'FILE':
-            return {'status': _STATUS_SKIPPED,
-                    'media': pick_in_dict(media, ['media_name', 'media_id', 'media_url', 'media_type']), }
+        if media_type != "FILE":
+            return {
+                "status": _STATUS_SKIPPED,
+                "media": pick_in_dict(media, ["media_name", "media_id", "media_url", "media_type"]),
+            }
 
         # If the file is not available on storage, we won't try to download it.
-        if safe_get_key(media, 'file_storage_status') != 'available':
-            return {'status': _STATUS_MISSING, 'media': pick_in_dict(media, ['media_name', 'media_id', 'media_url',
-                                                                             'file_type', 'file_storage_status'])}
+        if safe_get_key(media, "file_storage_status") != "available":
+            return {
+                "status": _STATUS_MISSING,
+                "media": pick_in_dict(
+                    media,
+                    [
+                        "media_name",
+                        "media_id",
+                        "media_url",
+                        "file_type",
+                        "file_storage_status",
+                    ],
+                ),
+            }
 
         # The metadata says the file is available, let's download it
         if not isdir(local_download_dir):
             raise FileNotFoundError(f"The following folder does not exist: '{local_download_dir}'")
 
-        media_name = safe_get_key(media, 'media_name')
-        media_url = safe_get_key(media, 'connector', 'url')
+        media_name = safe_get_key(media, "media_name")
+        media_url = safe_get_key(media, "connector", "url")
 
         destination_path = abspath(slash_join(local_download_dir, media_name))
         content = https_download(media_url)
-        open(destination_path, 'wb').write(content)
-        log_d('media_download', 'content saved to file', destination_path)
+        open(destination_path, "wb").write(content)
+        log_d("media_download", "content saved to file", destination_path)
 
-        file_info = {'media_name': media_name, 'media_id': safe_get_key(media, 'media_id'), 'media_url': media_url,
-                     'file_type': safe_get_key(media, 'file_type'),
-                     'created': safe_get_key(media, 'media_dates', 'created'),
-                     'updated': safe_get_key(media, 'media_dates', 'updated'), 'file_path': destination_path}
-        return {'status': _STATUS_DOWNLOADED, 'media': file_info}
+        file_info = {
+            "media_name": media_name,
+            "media_id": safe_get_key(media, "media_id"),
+            "media_url": media_url,
+            "file_type": safe_get_key(media, "file_type"),
+            "created": safe_get_key(media, "media_dates", "created"),
+            "updated": safe_get_key(media, "media_dates", "updated"),
+            "file_path": destination_path,
+        }
+        return {"status": _STATUS_DOWNLOADED, "media": file_info}
 
-    def download_file_with_uuid(self, media_uuid: str, local_download_dir: str) -> dict:
+    def download_file_with_uuid(self, media_uuid: str, local_download_dir: str) -> dict | None:
         """
         Download a file identified with the input UUID
         :param media_uuid: a UUIDv4 that identifies the media on the RUDI node
         :param local_download_dir: the path to a local folder
         :return: an object that states if the file was downloaded, skipped or found missing
         """
         # fun = 'download_media_with_uuid'
         meta = self.find_metadata_with_media_uuid(media_uuid)
-        media_list = safe_get_key(meta, 'available_formats')
+        media_list = safe_get_key(meta, "available_formats")
         if not media_list:
             return None
 
-        media = find_in_dict_list(media_list, {'media_id': media_uuid})
+        media = find_in_dict_list(media_list, {"media_id": media_uuid})
         return self._download_media_from_info(media, local_download_dir)
 
-    def download_file_with_name(self, media_name: str, local_download_dir: str) -> dict:
+    def download_file_with_name(self, media_name: str, local_download_dir: str) -> dict | None:
         """
         Find a file from its name and download it if it is available
         :param media_name: the name of the file we want to download
         :param local_download_dir: the path to a local folder
         :return: an object that states if the file was downloaded, skipped or found missing
         """
         # fun = 'download_media_with_name'
         meta = self.find_metadata_with_media_name(media_name)
-        media_list = safe_get_key(meta, 'available_formats')
+        media_list = safe_get_key(meta, "available_formats")
         if not media_list:
             return None
-        media = find_in_dict_list(media_list, {'media_name': media_name})
+        media = find_in_dict_list(media_list, {"media_name": media_name})
         return self._download_media_from_info(media, local_download_dir)
 
-    def download_files_for_metadata(self, metadata_id, local_download_dir) -> dict:
+    def download_files_for_metadata(self, metadata_id, local_download_dir) -> dict | None:
         """
         Download all the available files for a metadata
         :param metadata_id: the UUIDv4 of the metadata
         :param local_download_dir: the path to a local folder
         :return: an object that lists the files that were downloaded, skipped or found missing
         """
         # fun = 'download_all_media_for_metadata'
         if not isdir(local_download_dir):
             raise FileNotFoundError(f"The following folder does not exist: '{local_download_dir}'")
 
         meta = self.find_metadata_with_uuid(metadata_id)
-        media_list = safe_get_key(meta, 'available_formats')
+        media_list = safe_get_key(meta, "available_formats")
         if not media_list:
             return None
-        files_dwnld_info = {_STATUS_DOWNLOADED: [], _STATUS_MISSING: [], _STATUS_SKIPPED: []}
+        files_dwnld_info: dict = {
+            _STATUS_DOWNLOADED: [],
+            _STATUS_MISSING: [],
+            _STATUS_SKIPPED: [],
+        }
         for media in media_list:
             dwnld_info = self._download_media_from_info(media, local_download_dir)
-            status = dwnld_info['status']
-            files_dwnld_info[status].append(dwnld_info['media'])
+            status = dwnld_info["status"]
+            files_dwnld_info[status].append(dwnld_info["media"])
         return files_dwnld_info
 
-    def save_metadata_to_file(self, local_download_dir: str, file_name: str = 'rudi_node_metadata.json') -> None:
+    def save_metadata_to_file(self, local_download_dir: str, file_name: str = "rudi_node_metadata.json") -> None:
         """
         Dumps the metadata list to a local file
         :param local_download_dir: the path to a local folder
         :param file_name: the name of the file in which the JSON representation of the list of metadata will be saved
         """
         file_path = abspath(slash_join(local_download_dir, file_name))
-        json_str = dumps(obj=self.metadata_list, ensure_ascii=False, indent=2).encode('utf-8')
-        open(file_path, 'wb').write(json_str)
-
-
-if __name__ == '__main__':
-    rudi_node_info = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
-    info_tag = 'RudiNode info'
-    log_d(info_tag, 'metadata nb', rudi_node_info.metadata_count)
-    log_d(info_tag, 'metadata list nb', len(rudi_node_info.metadata_list))
-    log_d(info_tag, 'organizations', rudi_node_info.organization_list)
-    log_d(info_tag, 'organization names', rudi_node_info.organization_names)
-
-    log_d(info_tag, 'contact names', rudi_node_info.contact_names)
-    log_d(info_tag, 'themes', rudi_node_info.themes)
-    log_d(info_tag, 'keywords', rudi_node_info.keywords)
-
-    filter_tag = 'Filtering metadata'
-    log_d(filter_tag, 'filter_metadata', rudi_node_info.filter_metadata(
-        {'producer': {'organization_id': '1d6bc543-07ed-46f6-a813-958edb73d5f0', 'organization_name': 'SIB (Test)'}}))
-
-    meta_producer = 'SIB (Test)'
-    log_d(filter_tag, f"with producer '{meta_producer}'", rudi_node_info.get_metadata_with_producer(meta_producer))
-
-    meta_contact = 'Bacasable'
-    log_d(filter_tag, f"with contact '{meta_contact}'", rudi_node_info.get_metadata_with_contact(meta_contact))
-
-    meta_theme = 'citizenship'
-    log_d(filter_tag, f"with theme '{meta_theme}'", rudi_node_info.get_metadata_with_theme(meta_theme))
-
-    meta_keywords = ['python']
-    log_d(filter_tag, f"with keywords '{meta_keywords}'", rudi_node_info.get_metadata_with_keywords(meta_keywords))
-
-    log_d(filter_tag, f"with available media", rudi_node_info.metadata_with_available_media)
-
-    find_tag = 'Finding metadata'
-    meta_id = 'f48b4bcd-bba3-47ba-86e6-c0754b748728'
-    log_d(find_tag, f"with uuid '{meta_id}'", rudi_node_info.find_metadata_with_uuid(meta_id))
-
-    f_name = 'toucan.jpg'
-    log_d(find_tag, f"with media name '{f_name}'", rudi_node_info.find_metadata_with_media_name(f_name))
+        json_str = dumps(obj=self.metadata_list, ensure_ascii=False, indent=2).encode("utf-8")
+        open(file_path, "wb").write(json_str)
 
-    f_uuid = '782bab2d-7ee8-4633-9c0a-173649b4d879'
-    log_d(find_tag, f"with media uuid '{f_uuid}'", rudi_node_info.find_metadata_with_media_uuid(f_uuid))
 
-    dwnld_tag = 'Downloading'
-    dwnld_dir = '../../dwnld'
-    log_d(dwnld_tag, f"media for metadata '{meta_id}'", rudi_node_info.download_files_for_metadata(meta_id, dwnld_dir))
-    log_d(dwnld_tag, f"media with uuid '{f_uuid}'", rudi_node_info.download_file_with_uuid(f_uuid, dwnld_dir))
-    log_d(dwnld_tag, f"media with name '{f_name}'", rudi_node_info.download_file_with_name(f_name, dwnld_dir))
+if __name__ == "__main__":
+    rudi_node_info = RudiNodeReader("https://bacasable.fenix.rudi-univ-rennes1.fr")
+    info_tag = "RudiNode info"
+    log_d(info_tag, "metadata nb", rudi_node_info.metadata_count)
+    log_d(info_tag, "metadata list nb", len(rudi_node_info.metadata_list))
+    log_d(info_tag, "organizations", rudi_node_info.organization_list)
+    log_d(info_tag, "organization names", rudi_node_info.organization_names)
+
+    log_d(info_tag, "contact names", rudi_node_info.contact_names)
+    log_d(info_tag, "themes", rudi_node_info.themes)
+    log_d(info_tag, "keywords", rudi_node_info.keywords)
+
+    filter_tag = "Filtering metadata"
+    log_d(
+        filter_tag,
+        "filter_metadata",
+        rudi_node_info.filter_metadata(
+            {
+                "producer": {
+                    "organization_id": "1d6bc543-07ed-46f6-a813-958edb73d5f0",
+                    "organization_name": "SIB (Test)",
+                }
+            }
+        ),
+    )
+
+    meta_producer = "SIB (Test)"
+    log_d(
+        filter_tag,
+        f"with producer '{meta_producer}'",
+        rudi_node_info.get_metadata_with_producer(meta_producer),
+    )
+
+    meta_contact = "Bacasable"
+    log_d(
+        filter_tag,
+        f"with contact '{meta_contact}'",
+        rudi_node_info.get_metadata_with_contact(meta_contact),
+    )
+
+    meta_theme = "citizenship"
+    log_d(
+        filter_tag,
+        f"with theme '{meta_theme}'",
+        rudi_node_info.get_metadata_with_theme(meta_theme),
+    )
+
+    meta_keywords = ["python"]
+    log_d(
+        filter_tag,
+        f"with keywords '{meta_keywords}'",
+        rudi_node_info.get_metadata_with_keywords(meta_keywords),
+    )
+
+    log_d(
+        filter_tag,
+        "with available media",
+        rudi_node_info.metadata_with_available_media,
+    )
+
+    find_tag = "Finding metadata"
+    meta_id = "f48b4bcd-bba3-47ba-86e6-c0754b748728"
+    log_d(
+        find_tag,
+        f"with uuid '{meta_id}'",
+        rudi_node_info.find_metadata_with_uuid(meta_id),
+    )
+
+    f_name = "toucan.jpg"
+    log_d(
+        find_tag,
+        f"with media name '{f_name}'",
+        rudi_node_info.find_metadata_with_media_name(f_name),
+    )
+
+    f_uuid = "782bab2d-7ee8-4633-9c0a-173649b4d879"
+    log_d(
+        find_tag,
+        f"with media uuid '{f_uuid}'",
+        rudi_node_info.find_metadata_with_media_uuid(f_uuid),
+    )
+
+    dwnld_tag = "Downloading"
+    dwnld_dir = "../../dwnld"
+    log_d(
+        dwnld_tag,
+        f"media for metadata '{meta_id}'",
+        rudi_node_info.download_files_for_metadata(meta_id, dwnld_dir),
+    )
+    log_d(
+        dwnld_tag,
+        f"media with uuid '{f_uuid}'",
+        rudi_node_info.download_file_with_uuid(f_uuid, dwnld_dir),
+    )
+    log_d(
+        dwnld_tag,
+        f"media with name '{f_name}'",
+        rudi_node_info.download_file_with_name(f_name, dwnld_dir),
+    )
 
     rudi_node_info.save_metadata_to_file(dwnld_dir)
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/err.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/err.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-from typing import get_args
-
 from rudi_node_read.utils.type_string import slash_join
 
 
 class MissingEnvironmentVariableException(Exception):
-    def __init__(self, var_name: str, var_use: str = ''):
-        super().__init__(f'an environment variable should be defined {var_use}: {var_name}')
+    def __init__(self, var_name: str, var_use: str = ""):
+        super().__init__(f"an environment variable should be defined {var_use}: {var_name}")
 
 
 class IniMissingValueException(Exception):
     def __init__(self, ini_section: str, ini_subsection: str, err_msg: str):
-        super().__init__(f'Missing value in INI config file for parameter {ini_section}.{ini_subsection}: {err_msg}')
+        super().__init__(f"Missing value in INI config file for parameter {ini_section}.{ini_subsection}: {err_msg}")
 
 
 class IniUnexpectedValueException(Exception):
     def __init__(self, ini_section: str, ini_subsection: str, err_msg: str):
-        super().__init__(f'Unexpected value in INI config file for parameter {ini_section}.{ini_subsection}: {err_msg}')
+        super().__init__(f"Unexpected value in INI config file for parameter {ini_section}.{ini_subsection}: {err_msg}")
 
 
 class UnexpectedValueException(Exception):
     def __init__(self, param_name: str, expected_val, received_val):
         super().__init__(
-            f"Unexpected value for parameter '{param_name}': expected '{expected_val}', got '{received_val}'")
+            f"Unexpected value for parameter '{param_name}': expected '{expected_val}', got '{received_val}'"
+        )
 
 
 class LiteralUnexpectedValueException(Exception):
-    def __init__(self, err_msg, expected_literal, received_val):
-        super().__init__(f"{err_msg}. Expected {get_args(expected_literal)}, got '{received_val}'")
+    def __init__(
+        self,
+        received_val,
+        expected_literal: tuple,
+        err_msg: str = "Unexpected value error",
+    ):
+        super().__init__(f"{err_msg}. Expected {expected_literal}, got '{received_val}'")
 
 
 def rudi_api_http_error_to_string(status, err_type, err_msg):
     return f"ERR {status} {err_type}: {err_msg}"
 
 
 class HttpError(Exception):
-    def __init__(self, err, req_method=None, base_url=None, url=None):
-        err_msg = f"{err}"
-        if type(err) is dict and 'error' in err and 'message' in err:
-            if 'status' in err:
-                err_msg = rudi_api_http_error_to_string(err['status'], err['error'], err['message'])
-            elif 'statusCode' in err:
-                err_msg = rudi_api_http_error_to_string(err['statusCode'], err['error'], err['message'])
+    def __init__(self, err_msg: str, req_method=None, base_url=None, url=None):
+        err_msg = f"{err_msg}"
+        if type(err_msg) is dict and "error" in err_msg and "message" in err_msg:
+            if "status" in err_msg:
+                err_msg = rudi_api_http_error_to_string(err_msg["status"], err_msg["error"], err_msg["message"])
+            elif "statusCode" in err_msg:
+                err_msg = rudi_api_http_error_to_string(err_msg["statusCode"], err_msg["error"], err_msg["message"])
         if req_method and base_url:
             err_msg = f"for request '{req_method} {slash_join(base_url, url)}' -> {err_msg}"
-        super().__init__(f'HTTP ERR {err_msg}')
+        super().__init__(f"HTTP ERR {err_msg}")
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/jwt.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/jwt.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from math import ceil
 from time import time
 
 
 def pad_b64_str(jwt_base64url: str):
     jwt_str_length = len(jwt_base64url)
     div, mod = divmod(jwt_str_length, 4)
-    return jwt_base64url if mod == 0 else jwt_base64url.ljust(jwt_str_length + 4 - mod, '=')
+    return jwt_base64url if mod == 0 else jwt_base64url.ljust(jwt_str_length + 4 - mod, "=")
 
 
 def get_jwt_basic_auth(usr: str, pwd: str):
-    token = urlsafe_b64encode(bytes(f'{usr}:{pwd}', 'utf-8')).decode('ascii').replace('=', '')
-    return f'Basic {token}'
+    token = urlsafe_b64encode(bytes(f"{usr}:{pwd}", "utf-8")).decode("ascii").replace("=", "")
+    return f"Basic {pad_b64_str(token)}"
 
 
 def is_jwt_expired(jwt_b64: str) -> bool:
-    jwt_head_b64, jwt_body_b64, jwt_sign_b64 = jwt_b64.split('.')
+    jwt_head_b64, jwt_body_b64, jwt_sign_b64 = jwt_b64.split(".")
     jwt_body_b64_pad = pad_b64_str(jwt_body_b64)
-    jwt_str = urlsafe_b64decode(jwt_body_b64_pad).decode('utf-8')
+    jwt_str = urlsafe_b64decode(jwt_body_b64_pad).decode("utf-8")
     jwt_json = loads(jwt_str)
-    exp = int(jwt_json['exp'])
+    exp = int(jwt_json["exp"])
     now_epoch_s = ceil(time())
     return exp < now_epoch_s
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/log.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 SHOULD_LOG = False
 
 
 def log(*args):
     if SHOULD_LOG:
         if len(args) < 2:
-            print(f'D {now()}')
+            print(f"D {now()}")
         elif len(args) == 2:
-            print(f'{args[0]} {now()} [{args[1]}] <')
+            print(f"{args[0]} {now()} [{args[1]}] <")
         elif len(args) == 3:
-            print(f'{args[0]} {now()} [{args[1]}] {args[2]}')
+            print(f"{args[0]} {now()} [{args[1]}] {args[2]}")
         else:
             try:
-                print(f'{args[0]} {now()} [{args[1]}] {args[2]}:', *args[3:])
+                print(f"{args[0]} {now()} [{args[1]}] {args[2]}:", *args[3:])
             except UnicodeDecodeError:
-                print(f'{args[0]} {now()} [{args[1]}] {args[2]}:', str(*args[3:]))
+                print(f"{args[0]} {now()} [{args[1]}] {args[2]}:", str(*args[3:]))
 
 
 def log_e(*args):
-    log('E', *args)
+    log("E", *args)
 
 
 def log_d(*args):
-    log('D', *args)
+    log("D", *args)
 
 
 def log_d_if(should_print: bool, *args):
     if should_print:
         log_d(*args)
 
 
@@ -44,16 +44,16 @@
             result = some_function(*args, **kwargs)
         duration = (time() - begin) / multiplier
         return result, duration
 
     return _wrap
 
 
-def log_assert(cond: bool, ok_tag: str = 'OK', ko_tag: str = '!! KO !!'):
+def log_assert(cond: bool, ok_tag: str = "OK", ko_tag: str = "!! KO !!"):
     return ok_tag if cond else ko_tag
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     log_d()
-    log_d('Test log')
-    log_d('Log', 'Test')
-    log_d('Log', 'Main', 'test')
+    log_d("Test log")
+    log_d("Log", "Test")
+    log_d("Log", "Main", "test")
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/type_dict.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Union
 
-from rudi_node_read.utils.log import log_d, log_assert
-from rudi_node_read.utils.types import is_type, is_list, get_type_name, is_list_or_dict
+from rudi_node_read.utils.type_misc import is_type, is_list, is_list_or_dict
 
 
 def is_dict(obj) -> bool:
     """
     :return: True of input obj is an object, False otherwise
     """
-    return is_type(obj, 'dict')
+    return is_type(obj, "dict")
 
 
 def is_object(obj) -> bool:
     """
     :return: True of input obj is an object, False otherwise
     """
     return is_dict(obj)
@@ -28,14 +27,15 @@
         return False
     return key_name in obj.keys() and obj[key_name] is not None
 
 
 def check_has_key(obj: dict, key_name: str):
     if not has_key(obj, key_name):
         raise AttributeError(f"Property '{key_name}' missing in obj {obj}")
+    return obj[key_name]
 
 
 def safe_get_key(obj: dict, *args):
     """
     Offers a way to access an object attribute hierarchy without raising an error if the attribute doesn't exist
     :param obj: an object
     :param args: hierarchy of attributes we need to access.
@@ -61,30 +61,30 @@
     :param obj: an object
     :param props: the attributes to keep from the input object
     :return:
     """
     return dict((k, obj[k]) for k in props if k in obj)
 
 
-def is_element_matching_filter(element, match_filter):
+def is_element_matching_filter(element, match_filter) -> bool:
     """
     An element is considered to be matching a filter if all the key/value pairs in the filter are found in the element
     :param element: element that is tested
     :param match_filter: object whose key/value pairs must be found in the tested element
     :return: True if the element is matching the filter object
     """
-    fun = 'match_filter'
+    # fun = "match_filter"
     if element == match_filter:
         return True
     if not is_list_or_dict(element):
         return False
     if is_dict(element):
         if not is_dict(match_filter):
             return False
-        for i, (key, val) in enumerate(match_filter.items()):
+        for key, val in match_filter.items():
             if not has_key(element, key) or not is_element_matching_filter(element[key], val):
                 return False
         return True
     # elif is_list(element):
     if is_dict(match_filter):
         for e in element:
             if is_element_matching_filter(e, match_filter):
@@ -123,15 +123,15 @@
     :return:
     """
     found_elements = []
     for element in searched_list:
         if is_dict(search_filter):
             if is_element_matching_filter(element, search_filter):
                 found_elements.append(element)
-        elif is_type(search_filter, 'list'):
+        elif is_type(search_filter, "list"):
             if is_element_matching_one_of_filters(element, search_filter):
                 found_elements.append(element)
     return found_elements
 
 
 def find_in_dict_list(searched_list: list, search_filter: dict):
     """
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/type_string.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_string.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 from re import compile
 from uuid import UUID
 
-from rudi_node_read.utils.log import log_d
-from rudi_node_read.utils.types import is_type
+from rudi_node_read.utils.type_misc import is_type
 
 
-def is_string(s):
-    return is_type(s, 'str')
+def is_string(s) -> bool:
+    return is_type(s, "str")
 
 
 ISO_FULL_DATE_REGEX = compile(
-    r'^([+-]?[1-9]\d{3})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12]\d)T(2[0-3]|[01]\d):([0-5]\d):([0-5]\d)(?:\.(\d{3}))?('
-    r'?:Z|[+-](?:1[0-2]|0\d):[03]0)$')
+    r"^([+-]?[1-9]\d{3})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12]\d)T(2[0-3]|[01]\d):([0-5]\d):([0-5]\d)(?:\.(\d{3}))?("
+    r"?:Z|[+-](?:1[0-2]|0\d):[03]0)$"
+)
 
 
-def is_iso_full_date(date_str):
+def is_iso_full_date(date_str) -> bool:
     return bool(ISO_FULL_DATE_REGEX.match(date_str))
 
 
 # REGEX_UUID = re.compile(r'^[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$')
 
 
-def is_uuid_v4(uuid: str):
+def is_uuid_v4(uuid: str) -> bool:
     if uuid is None:
         return False
     try:
         uuid_v4 = UUID(str(uuid))
         if uuid_v4.version == 4:
-            return uuid_v4
+            return True
         else:
             return False
-    except ValueError as e:
+    except ValueError:
         return False
 
 
-def validate_uuid_v4(uuid: str):
+def check_is_uuid4(uuid: str | UUID) -> str:
+    if uuid is None:
+        raise ValueError("Input parameter should not be null")
     try:
-        if uuid is not None:
-            uuid_v4 = UUID(str(uuid))
-            if uuid_v4.version == 4:
-                return str(uuid_v4)
+        uuid_v4 = UUID(str(uuid))
+        if uuid_v4.version == 4:
+            return str(uuid_v4)
     except ValueError:
         pass
-    raise ValueError('System ID should be a UUIDv4')
+    raise ValueError(f"Input parameter is not a valid UUID v4: '{uuid}'")
 
 
-def slash_join(*args):
+def slash_join(*args) -> str:
     """
     Joins a set of strings with a slash (/) between them (useful for merging URLs or paths fragments)
     """
     non_null_args = []
     for frag in args:
-        if frag is None or frag == '':
+        if frag is None or frag == "":
             pass
         elif not is_string(frag):
-            raise AttributeError('input parameters must be strings')
+            raise AttributeError("input parameters must be strings")
         else:
-            non_null_args.append(frag.strip('/'))
-    joined_str = '/'.join(non_null_args)
+            non_null_args.append(frag.strip("/"))
+    joined_str = "/".join(non_null_args)
     return joined_str
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read/utils/types.py` & `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-from rudi_node_read.utils.log import log_d, log_e
-
-
 def get_type_name(obj):
     return type(obj).__name__
 
 
 def is_type(obj, type_name: str):
     return get_type_name(obj) == type_name
 
 
 def is_list(obj):
-    return get_type_name(obj) == 'list'
+    return get_type_name(obj) == "list"
 
 
 def is_array(obj):
     return is_list(obj)
 
 
 def is_list_or_dict(obj):
-    return get_type_name(obj) in ['dict', 'list']
+    return get_type_name(obj) in ["dict", "list"]
 
 
-def check_type(obj, type_name: str, param_name: str = None):
-    param_str = 'Parameter' if param_name is None else f"Parameter '{param_name}'"
+def check_type(obj, type_name: str, param_name: str | None = None):
+    param_str = "Parameter" if param_name is None else f"Parameter '{param_name}'"
     if not is_type(obj, type_name):
         raise TypeError(f"{param_str} should be a '{type_name}', got '{get_type_name(obj)}'")
 
 
 def to_float(val):
     try:
         f_val = float(val)
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read.egg-info/PKG-INFO` & `rudi-node-read-0.1.4/src/rudi_node_read.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
-Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
-Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
-Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
-Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/OlivierMartineau/rudi-node-read
+Project-URL: Documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
+Project-URL: Changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
+Project-URL: Source, https://github.com/OlivierMartineau/rudi-node-read
+Keywords: rudi-node-read,rudi-node-get,RUDI,producer node,RUDI node,rudinode,open-data,Univ. Rennes
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: packaging
 Provides-Extra: tests
 License-File: LICENCE.md
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
 The Jupyter notebook [README.ipynb](https://github.com/OlivierMartineau/rudi-node-read/blob/release/README.ipynb) offers
@@ -46,15 +48,13 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+
 ## Testing
 
 ```bash
-pip install pytest-cov
-
-python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+$ pytest
 ```
-
```

### Comparing `rudi-node-read-0.1.3/src/rudi_node_read.egg-info/SOURCES.txt` & `rudi-node-read-0.1.4/src/rudi_node_read.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 LICENCE.md
 README.md
 pyproject.toml
+src/rudi_node_read/__init_.py
 src/rudi_node_read/rudi_node_reader.py
 src/rudi_node_read.egg-info/PKG-INFO
 src/rudi_node_read.egg-info/SOURCES.txt
 src/rudi_node_read.egg-info/dependency_links.txt
 src/rudi_node_read.egg-info/requires.txt
 src/rudi_node_read.egg-info/top_level.txt
 src/rudi_node_read/connectors/io_connector.py
-src/rudi_node_read/connectors/io_rudi_api.py
+src/rudi_node_read/connectors/io_rudi_node_read.py
 src/rudi_node_read/utils/err.py
 src/rudi_node_read/utils/jwt.py
 src/rudi_node_read/utils/log.py
 src/rudi_node_read/utils/serializable.py
 src/rudi_node_read/utils/type_dict.py
+src/rudi_node_read/utils/type_misc.py
 src/rudi_node_read/utils/type_string.py
-src/rudi_node_read/utils/types.py
 tests/test_rudi_node_reader.py
```

### Comparing `rudi-node-read-0.1.3/tests/test_rudi_node_reader.py` & `rudi-node-read-0.1.4/tests/test_rudi_node_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from rudi_node_read.rudi_node_reader import RudiNodeReader
 
-rudi_node_info = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
+rudi_node_info = RudiNodeReader("https://bacasable.fenix.rudi-univ-rennes1.fr")
 
 
 @pytest.fixture
 def rudi_node():
     assert rudi_node_info is not None
     return rudi_node_info
 
@@ -40,63 +40,63 @@
 
 
 def test_keywords(rudi_node):
     assert len(rudi_node.keywords) > 0
 
 
 def test_filter_metadata(rudi_node):
-    meta1_id = rudi_node.metadata_list[0]['global_id']
-    assert len(rudi_node.filter_metadata({'global_id': meta1_id})) == 1
+    meta1_id = rudi_node.metadata_list[0]["global_id"]
+    assert len(rudi_node.filter_metadata({"global_id": meta1_id})) == 1
 
 
 def test_get_metadata_with_producer(rudi_node):
-    producer_name = rudi_node.metadata_list[0]['producer']['organization_name']
+    producer_name = rudi_node.metadata_list[0]["producer"]["organization_name"]
     assert len(rudi_node.get_metadata_with_producer(producer_name)) > 0
 
 
 def test_get_metadata_with_contact(rudi_node):
-    contact_name = rudi_node.metadata_list[0]['contacts'][0]['contact_name']
+    contact_name = rudi_node.metadata_list[0]["contacts"][0]["contact_name"]
     assert len(rudi_node.get_metadata_with_contact(contact_name)) > 0
 
 
 def test_get_metadata_with_theme(rudi_node):
-    theme = rudi_node.metadata_list[0]['theme']
+    theme = rudi_node.metadata_list[0]["theme"]
     assert len(rudi_node.get_metadata_with_theme(theme)) > 0
 
 
 def test_get_metadata_with_keywords(rudi_node):
-    keywords = rudi_node.metadata_list[0]['keywords']
+    keywords = rudi_node.metadata_list[0]["keywords"]
     assert len(rudi_node.get_metadata_with_keywords([keywords])) > 0
 
 
 def test_find_metadata_with_uuid(rudi_node):
-    meta1_id = rudi_node.metadata_list[0]['global_id']
-    assert rudi_node.find_metadata_with_uuid(meta1_id)['global_id'] == meta1_id
+    meta1_id = rudi_node.metadata_list[0]["global_id"]
+    assert rudi_node.find_metadata_with_uuid(meta1_id)["global_id"] == meta1_id
 
 
 def test_find_metadata_with_title(rudi_node):
-    meta1_title = rudi_node.metadata_list[0]['resource_title']
+    meta1_title = rudi_node.metadata_list[0]["resource_title"]
     assert bool(meta1_title)
     meta1 = rudi_node.find_metadata_with_title(meta1_title)
     assert bool(meta1)
-    assert meta1['resource_title'] == meta1_title
+    assert meta1["resource_title"] == meta1_title
 
 
 def test_metadata_with_available_media(rudi_node):
     meta_list = rudi_node.metadata_with_available_media
     assert len(meta_list) > 0
-    media_list = meta_list[0]['available_formats']
+    media_list = meta_list[0]["available_formats"]
     an_available_media_was_found = False
     for media in media_list:
-        if media['media_type'] == 'FILE' and media['file_storage_status'] == 'available':
+        if media["media_type"] == "FILE" and media["file_storage_status"] == "available":
             an_available_media_was_found = True
     assert an_available_media_was_found
 
 
 def test_find_metadata_with_media_name(rudi_node):
-    media_name = rudi_node.metadata_list[0]['available_formats'][0]['media_name']
+    media_name = rudi_node.metadata_list[0]["available_formats"][0]["media_name"]
     assert len(rudi_node.find_metadata_with_media_name(media_name)) > 0
 
 
 def test_find_metadata_with_media_name(rudi_node):
-    media_uuid = rudi_node.metadata_list[0]['available_formats'][0]['media_id']
+    media_uuid = rudi_node.metadata_list[0]["available_formats"][0]["media_id"]
     assert len(rudi_node.find_metadata_with_media_uuid(media_uuid)) > 0
```

