# Comparing `tmp/pteropy-0.1.8.tar.gz` & `tmp/pteropy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pteropy-0.1.8.tar", last modified: Sun May 21 09:12:25 2023, max compression
+gzip compressed data, was "pteropy-0.1.9.tar", last modified: Tue Jul 11 13:26:16 2023, max compression
```

## Comparing `pteropy-0.1.8.tar` & `pteropy-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.121054 pteropy-0.1.8/
--rw-rw-rw-   0        0        0     1083 2023-04-04 14:05:48.000000 pteropy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2778 2023-05-21 09:12:25.114867 pteropy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2308 2023-04-09 13:33:36.000000 pteropy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.086803 pteropy-0.1.8/pteropy/
--rw-rw-rw-   0        0        0     7477 2023-05-21 09:11:42.000000 pteropy-0.1.8/pteropy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.109860 pteropy-0.1.8/pteropy.egg-info/
--rw-rw-rw-   0        0        0     2778 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 09:12:25.122074 pteropy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-21 09:12:14.000000 pteropy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:26:16.349828 pteropy-0.1.9/
+-rw-rw-rw-   0        0        0     1083 2023-05-21 09:17:32.000000 pteropy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2816 2023-07-11 13:26:16.347816 pteropy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2346 2023-07-11 13:23:48.000000 pteropy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 13:26:16.326175 pteropy-0.1.9/pteropy/
+-rw-rw-rw-   0        0        0    10095 2023-07-11 13:21:49.000000 pteropy-0.1.9/pteropy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:26:16.344285 pteropy-0.1.9/pteropy.egg-info/
+-rw-rw-rw-   0        0        0     2816 2023-07-11 13:26:16.000000 pteropy-0.1.9/pteropy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-11 13:26:16.000000 pteropy-0.1.9/pteropy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:26:16.000000 pteropy-0.1.9/pteropy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 13:26:16.000000 pteropy-0.1.9/pteropy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:26:16.349828 pteropy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-07-11 13:25:08.000000 pteropy-0.1.9/setup.py
```

### Comparing `pteropy-0.1.8/LICENSE` & `pteropy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pteropy-0.1.8/PKG-INFO` & `pteropy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.8
+Version: 0.1.9
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
 Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -122,9 +122,11 @@
 ptero.start_server("3fa3d78d")  #啟動伺服器
 
 ptero.restart_server("3fa3d78d")  #重啟伺服器
 
 ptero.stop_server("3fa3d78d")  #關閉伺服器
 
 ptero.kill_server("3fa3d78d")  #強制關閉伺服器
+
+#資料庫已經好了等待更新
 ```
```

### Comparing `pteropy-0.1.8/README.md` & `pteropy-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,8 +106,10 @@
 ptero.start_server("3fa3d78d")  #啟動伺服器
 
 ptero.restart_server("3fa3d78d")  #重啟伺服器
 
 ptero.stop_server("3fa3d78d")  #關閉伺服器
 
 ptero.kill_server("3fa3d78d")  #強制關閉伺服器
+
+#資料庫已經好了等待更新
 ```
```

### Comparing `pteropy-0.1.8/pteropy/__init__.py` & `pteropy-0.1.9/pteropy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import os
 import json
+import urllib.parse
 
 
 class Pterodactyl_Application:
     def __init__(self, base_url, api_key):
         if base_url[-1] == "/":
             base_url = base_url[:-1]
         self.base_url = base_url
@@ -142,25 +143,87 @@
 
     def create_API_key(self, description, allowed_ips: list = None):
         url = f'{self.base_url}/api/client/account/api-keys'
         headers = self.headers
         if allowed_ips == None:
             payload = {"description": description}
         else:
-            payload = {"description": description,"allowed_ips": allowed_ips}
+            payload = {"description": description, "allowed_ips": allowed_ips}
 
-        response = requests.request('POST', url, data=json.dumps(payload), headers=headers)
+        response = requests.request(
+            'POST', url, data=json.dumps(payload), headers=headers)
         return response.json()
 
     def delete_API_key(self, key_identifier):
         url = f'{self.base_url}/api/client/account/api-keys/{key_identifier}'
         headers = self.headers
         response = requests.request('DELETE', url,  headers=headers)
         return response
 
+    def list_databases(self, server):
+        url = f'{self.base_url}/api/client/servers/{server}/databases'
+        headers = self.headers
+        response = requests.request('GET', url,  headers=headers)
+        return response.json()
+
+    def create_databases(self, server, database, remote):
+        url = f'{self.base_url}/api/client/servers/{server}/databases'
+        headers = self.headers
+        payload = {
+            "database": database,
+            "remote": remote
+        }
+        response = requests.request(
+            'POST', url, data=json.dumps(payload), headers=headers)
+        return response.json()
+
+    def rotate_password(self, server, database):
+        url = f'{self.base_url}/api/client/servers/1a7ce997/databases/{database}/rotate-password'
+        headers = self.headers
+        response = requests.request('POST', url, headers=headers)
+        return response.json()
+
+    def delete_database(self, server, database):
+        url = f'{self.base_url}/api/client/servers/{server}/databases/{database}'
+        headers = self.headers
+        response = requests.request('DELETE', url, headers=headers)
+        return response
+
+    def list_files(self, server, directory=None):
+        if directory:
+            url = f'{self.base_url}/api/client/servers/{server}/files/list?directory={urllib.parse.quote_plus(directory)}'
+        else:
+            url = f'{self.base_url}/api/client/servers/{server}/files/list'
+        headers = self.headers
+        response = requests.request('GET', url, headers=headers)
+        return response.json()
+
+    def get_file_contents(self, server, file):
+        url = f'{self.base_url}/api/client/servers/{server}/files/contents?file={urllib.parse.quote_plus(file)}'
+        headers = self.headers
+        response = requests.request('GET', url,  headers=headers)
+        return response.text
+
+    def download_file(self, server, file):
+        url = f'{self.base_url}/api/client/servers/{server}/files/download?file={urllib.parse.quote_plus(file)}'
+        headers = self.headers
+        response = requests.request('GET', url, headers=headers)
+        return response.json()
+
+    def rename_file(self, server,root,files):
+        url = f'{self.base_url}/api/client/servers/{server}/files/rename'
+        headers = self.headers
+        payload = {
+            "root": root,
+            "files":files
+        }
+
+        response = requests.request('PUT', url, data=json.dumps(payload), headers=headers)
+        return response
+
     def get_server(self, server: str):
         self.server = server
         url = f'{self.base_url}/api/client/servers/{self.server}'
         headers = self.headers
 
         response = requests.request('GET', url, headers=headers)
         try:
@@ -203,16 +266,18 @@
         response = requests.request('POST', url, data=payload, headers=headers)
         return response
 
     def rename_server(self, server: str, name: str):
         url = f'{self.base_url}/api/client/servers/{server}/settings/rename'
         headers = self.headers
         payload = {"name": name}
-        response = requests.request('POST', url, data=json.dumps(payload), headers=headers)
+        response = requests.request(
+            'POST', url, data=json.dumps(payload), headers=headers)
         return response
 
     def send_command(self, server: str, command: str):
         url = f'{self.base_url}/api/client/servers/{server}/command'
         headers = self.headers
         payload = {"command": command}
-        response = requests.request('POST', url, data=json.dumps(payload), headers=headers)
+        response = requests.request(
+            'POST', url, data=json.dumps(payload), headers=headers)
         return response
```

### Comparing `pteropy-0.1.8/pteropy.egg-info/PKG-INFO` & `pteropy-0.1.9/pteropy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.8
+Version: 0.1.9
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
 Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -122,9 +122,11 @@
 ptero.start_server("3fa3d78d")  #啟動伺服器
 
 ptero.restart_server("3fa3d78d")  #重啟伺服器
 
 ptero.stop_server("3fa3d78d")  #關閉伺服器
 
 ptero.kill_server("3fa3d78d")  #強制關閉伺服器
+
+#資料庫已經好了等待更新
 ```
```

### Comparing `pteropy-0.1.8/setup.py` & `pteropy-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r",encoding="utf-8") as f:
     long_description = f.read()
     
 setuptools.setup(
     name = "pteropy",
-    version = "0.1.8",
+    version = "0.1.9",
     author = "Hans",
     author_email="ccoccc14@gmail.com",
     description="簡單存取Pterodactyl api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HansHans135/pteropy",                                         
     packages=setuptools.find_packages(),
```

