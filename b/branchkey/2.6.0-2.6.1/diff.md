# Comparing `tmp/branchkey-2.6.0.tar.gz` & `tmp/branchkey-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branchkey-2.6.0.tar", last modified: Mon Jul  3 11:25:41 2023, max compression
+gzip compressed data, was "branchkey-2.6.1.tar", last modified: Tue Jul 11 08:39:58 2023, max compression
```

## Comparing `branchkey-2.6.0.tar` & `branchkey-2.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.704577 branchkey-2.6.0/
--rw-r--r--   0 root         (0) root         (0)     5243 2023-07-03 11:25:41.704577 branchkey-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-07-03 11:25:26.000000 branchkey-2.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-25 09:44:56.000000 branchkey-2.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 11:25:41.704577 branchkey-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-03 11:25:40.000000 branchkey-2.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.692577 branchkey-2.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.692577 branchkey-2.6.0/src/branchkey/
--rw-rw-rw-   0 root         (0) root         (0)     5125 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/__consumer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10466 2023-07-03 11:25:26.000000 branchkey-2.6.0/src/branchkey/client.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.704577 branchkey-2.6.0/src/branchkey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5243 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:39:58.016447 branchkey-2.6.1/
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-07-11 08:39:58.016447 branchkey-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-07-11 08:39:46.000000 branchkey-2.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-30 06:54:10.000000 branchkey-2.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 08:39:58.016447 branchkey-2.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-11 08:39:57.000000 branchkey-2.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:39:57.992448 branchkey-2.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:39:58.016447 branchkey-2.6.1/src/branchkey/
+-rw-rw-rw-   0 root         (0) root         (0)     5125 2023-05-30 06:54:10.000000 branchkey-2.6.1/src/branchkey/__consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 06:54:10.000000 branchkey-2.6.1/src/branchkey/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10712 2023-07-11 08:39:46.000000 branchkey-2.6.1/src/branchkey/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-30 06:54:10.000000 branchkey-2.6.1/src/branchkey/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:39:58.016447 branchkey-2.6.1/src/branchkey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-07-11 08:39:57.000000 branchkey-2.6.1/src/branchkey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-07-11 08:39:57.000000 branchkey-2.6.1/src/branchkey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 08:39:57.000000 branchkey-2.6.1/src/branchkey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-11 08:39:57.000000 branchkey-2.6.1/src/branchkey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 08:39:57.000000 branchkey-2.6.1/src/branchkey.egg-info/top_level.txt
```

### Comparing `branchkey-2.6.0/PKG-INFO` & `branchkey-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.6.0
+Version: 2.6.1
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,20 @@
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "response_host":"response.branchkey.com"}
 
-  host = "http://api.branchkey.com"
+  host = "https://api.branchkey.com"
+
+  proxy_servers = {
+        'http': 'http://user:password@proxyserver.com:8080',
+        'https': 'http://user:password@proxyserver.com:8080',
+        }
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
   ssl: Whether to verify the SSL certificates of the
   remote host or not. Default it True
@@ -62,15 +67,15 @@
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
   parameter decides the sleeping interval of the
   program until the run status is checked again.
   Default is 30 seconds
   '''
-  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+  c = Client(credentials,host, ssl=True, wait_for_run=True, run_check_interval_s=15, proxies=proxy_servers)
 
   '''
   upload the file to the system
   '''
   c.file_upload("./file/path.npy")
 
   '''Download a file with the file_id value
```

### Comparing `branchkey-2.6.0/README.md` & `branchkey-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,20 @@
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "response_host":"response.branchkey.com"}
 
-  host = "http://api.branchkey.com"
+  host = "https://api.branchkey.com"
+
+  proxy_servers = {
+        'http': 'http://user:password@proxyserver.com:8080',
+        'https': 'http://user:password@proxyserver.com:8080',
+        }
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
   ssl: Whether to verify the SSL certificates of the
   remote host or not. Default it True
@@ -47,15 +52,15 @@
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
   parameter decides the sleeping interval of the
   program until the run status is checked again.
   Default is 30 seconds
   '''
-  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+  c = Client(credentials,host, ssl=True, wait_for_run=True, run_check_interval_s=15, proxies=proxy_servers)
 
   '''
   upload the file to the system
   '''
   c.file_upload("./file/path.npy")
 
   '''Download a file with the file_id value
```

### Comparing `branchkey-2.6.0/setup.py` & `branchkey-2.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(os.path.join(current_directory, "README.md"), encoding="utf-8") as f:
         long_description = f.read()
 except Exception:
     long_description = ""
 
 setuptools.setup(
     name="branchkey",
-    version="2.6.0",
+    version="2.6.1",
     author="BranchKey",
     author_email="info@branchkey.com",
     description="Client application to interface with the BranchKey system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://branchkey.com",
     project_urls={
```

### Comparing `branchkey-2.6.0/src/branchkey/__consumer.py` & `branchkey-2.6.1/src/branchkey/__consumer.py`

 * *Files identical despite different names*

### Comparing `branchkey-2.6.0/src/branchkey/client.py` & `branchkey-2.6.1/src/branchkey/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 
 from .__consumer import Consumer
 from .utils import AGGREGATED_OUTPUT_DIR, FILE_METADATA
 
 
 class Client:
     def __init__(self,
-                 credentials: dict = None,
+                 credentials: dict,
                  host: str = "https://api.branchkey.com",
-                 ssl: bool = True, wait_for_run: bool = False, run_check_interval_s: int = 30):
+                 ssl: bool = True, 
+                 wait_for_run: bool = False, 
+                 run_check_interval_s: int = 30,
+                 proxies : dict = None):
 
         if credentials is None:
             credentials = dict(leaf_name="guest", leaf_id="guest", leaf_session_token="guest",
                                response_host="response.branchkey.com", port=5672)
 
         self.__leaf_name = credentials["leaf_name"]
         self.__leaf_id = credentials["leaf_id"]
         self.__leaf_session_token = credentials["leaf_session_token"]
         self.__status = "unauthenticated"
         self.__tree_id = None
         self.__branch_id = None
 
         self.__api_host = host
+        self.__proxies = proxies
         # Verify SSL certs
         self.__verify = ssl
 
         self.queue = Queue()
         self.__run_status = None
         self.__run_number = None
         self.__wait_for_run = wait_for_run
@@ -50,15 +54,15 @@
 
     def __authenticate(self):
         try:
             url = self.__api_host + "/v1/leaf/authenticate"
             headers = {"accept": "application/json"}
 
             resp = requests.get(url, headers=headers,
-                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
+                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify, proxies=self.__proxies)
 
             print(f"received resp code form auth: {resp.status_code}")
             if resp.status_code != HTTPStatus.OK:
                 raise Exception(resp.json())
 
             authenticate_data = resp.json()["data"]
             try:
@@ -82,15 +86,15 @@
 
     def get_run_details(self):
         try:
             url = self.__api_host + "/v1/branch/" + self.__branch_id + "/run"
             headers = {"accept": "application/json", "leaf": "true"}
 
             resp = requests.get(url, headers=headers,
-                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
+                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify, proxies=self.__proxies)
 
             print(
                 f"received resp code from api-gateway for get_run_details: {resp.status_code}")
             if resp.status_code != HTTPStatus.OK:
                 raise Exception(resp.json())
 
             run_details = resp.json()["data"]
@@ -167,15 +171,15 @@
                 headers = {"accept": "application/json"}
                 data = {"data": json.dumps({"leaf_name": self.__leaf_name,
                                             "metadata": FILE_METADATA})}
                 file = {"file": f}
 
                 resp = requests.post(
                     url, files=file, data=data, headers=headers,
-                    auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
+                    auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify, proxies=self.__proxies)
                 f.close()
 
                 if resp.status_code != HTTPStatus.CREATED:
                     raise Exception(resp.json()["error"])
                 else:
                     return resp.json()["data"]["file_id"]
 
@@ -188,26 +192,26 @@
         try:
             if not os.path.exists(AGGREGATED_OUTPUT_DIR):
                 os.makedirs(AGGREGATED_OUTPUT_DIR)
 
             url = self.__api_host + "/v1/file/download/" + file_id
             headers = {"accept": "*/*S"}
             resp = requests.get(url, headers=headers,
-                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
+                                auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify, proxies=self.__proxies)
 
             if resp.status_code != HTTPStatus.OK:
                 raise Exception(resp.json()["error"])
 
             try:
                 download_url = resp.json()["data"]["download_url"]
             except Exception as e:
                 raise Exception(
                     f"Failed to parse response from download API: {resp.json()}")
 
-            resp = requests.get(download_url, verify=self.__verify)
+            resp = requests.get(download_url, verify=self.__verify, proxies=self.__proxies)
             if len(resp.content) == 0:
                 raise Exception("file not received")
 
             f = open(AGGREGATED_OUTPUT_DIR +
                      '/' + file_id + ".npy", 'wb')
             f.write(resp.content)
             f.close()
@@ -227,15 +231,15 @@
                                "aggregation_id": aggregation_id,
                                "leaf_id": self.__leaf_id,
                                "branch_id": self.__branch_id,
                                "tree_id": self.__tree_id,
                                "data": data})
 
             resp = requests.post(url, headers=headers, data=data,
-                                 auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
+                                 auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify, proxies=self.__proxies)
 
             print(
                 f"received resp code form performance_analyser: {resp.status_code}")
             if resp.status_code != HTTPStatus.CREATED:
                 raise Exception(resp.json())
             else:
                 return True
```

### Comparing `branchkey-2.6.0/src/branchkey.egg-info/PKG-INFO` & `branchkey-2.6.1/src/branchkey.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.6.0
+Version: 2.6.1
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,20 @@
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "response_host":"response.branchkey.com"}
 
-  host = "http://api.branchkey.com"
+  host = "https://api.branchkey.com"
+
+  proxy_servers = {
+        'http': 'http://user:password@proxyserver.com:8080',
+        'https': 'http://user:password@proxyserver.com:8080',
+        }
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
   ssl: Whether to verify the SSL certificates of the
   remote host or not. Default it True
@@ -62,15 +67,15 @@
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
   parameter decides the sleeping interval of the
   program until the run status is checked again.
   Default is 30 seconds
   '''
-  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+  c = Client(credentials,host, ssl=True, wait_for_run=True, run_check_interval_s=15, proxies=proxy_servers)
 
   '''
   upload the file to the system
   '''
   c.file_upload("./file/path.npy")
 
   '''Download a file with the file_id value
```

