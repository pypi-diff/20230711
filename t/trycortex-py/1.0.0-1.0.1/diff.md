# Comparing `tmp/trycortex-py-1.0.0.tar.gz` & `tmp/trycortex-py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-py-1.0.0.tar", last modified: Sat Jul  8 00:24:53 2023, max compression
+gzip compressed data, was "trycortex-py-1.0.1.tar", last modified: Mon Jul 10 23:01:18 2023, max compression
```

## Comparing `trycortex-py-1.0.0.tar` & `trycortex-py-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-08 00:24:53.952089 trycortex-py-1.0.0/
--rw-r--r--   0 charlespun   (501) staff       (20)      353 2023-07-08 00:24:53.951909 trycortex-py-1.0.0/PKG-INFO
--rw-r--r--   0 charlespun   (501) staff       (20)       15 2023-07-06 19:03:30.000000 trycortex-py-1.0.0/README.md
-drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-08 00:24:53.950390 trycortex-py-1.0.0/cortex/
--rw-r--r--   0 charlespun   (501) staff       (20)       79 2023-07-07 23:53:07.000000 trycortex-py-1.0.0/cortex/__init__.py
--rw-r--r--   0 charlespun   (501) staff       (20)    12631 2023-07-08 00:15:56.000000 trycortex-py-1.0.0/cortex/api.py
--rw-r--r--   0 charlespun   (501) staff       (20)       38 2023-07-08 00:24:53.952166 trycortex-py-1.0.0/setup.cfg
--rw-r--r--   0 charlespun   (501) staff       (20)      520 2023-07-08 00:24:19.000000 trycortex-py-1.0.0/setup.py
-drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-08 00:24:53.951593 trycortex-py-1.0.0/trycortex_py.egg-info/
--rw-r--r--   0 charlespun   (501) staff       (20)      353 2023-07-08 00:24:53.000000 trycortex-py-1.0.0/trycortex_py.egg-info/PKG-INFO
--rw-r--r--   0 charlespun   (501) staff       (20)      230 2023-07-08 00:24:53.000000 trycortex-py-1.0.0/trycortex_py.egg-info/SOURCES.txt
--rw-r--r--   0 charlespun   (501) staff       (20)        1 2023-07-08 00:24:53.000000 trycortex-py-1.0.0/trycortex_py.egg-info/dependency_links.txt
--rw-r--r--   0 charlespun   (501) staff       (20)        9 2023-07-08 00:24:53.000000 trycortex-py-1.0.0/trycortex_py.egg-info/requires.txt
--rw-r--r--   0 charlespun   (501) staff       (20)        7 2023-07-08 00:24:53.000000 trycortex-py-1.0.0/trycortex_py.egg-info/top_level.txt
+drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-10 23:01:18.683857 trycortex-py-1.0.1/
+-rw-r--r--   0 charlespun   (501) staff       (20)      353 2023-07-10 23:01:18.683654 trycortex-py-1.0.1/PKG-INFO
+-rw-r--r--   0 charlespun   (501) staff       (20)       15 2023-07-06 19:03:30.000000 trycortex-py-1.0.1/README.md
+drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-10 23:01:18.682349 trycortex-py-1.0.1/cortex/
+-rw-r--r--   0 charlespun   (501) staff       (20)       87 2023-07-10 22:39:25.000000 trycortex-py-1.0.1/cortex/__init__.py
+-rw-r--r--   0 charlespun   (501) staff       (20)    12976 2023-07-10 22:57:38.000000 trycortex-py-1.0.1/cortex/api.py
+-rw-r--r--   0 charlespun   (501) staff       (20)       38 2023-07-10 23:01:18.683921 trycortex-py-1.0.1/setup.cfg
+-rw-r--r--   0 charlespun   (501) staff       (20)      536 2023-07-10 23:01:13.000000 trycortex-py-1.0.1/setup.py
+drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-10 23:01:18.682640 trycortex-py-1.0.1/tests/
+-rw-r--r--   0 charlespun   (501) staff       (20)      658 2023-07-10 23:01:08.000000 trycortex-py-1.0.1/tests/test_cortex.py
+drwxr-xr-x   0 charlespun   (501) staff       (20)        0 2023-07-10 23:01:18.683326 trycortex-py-1.0.1/trycortex_py.egg-info/
+-rw-r--r--   0 charlespun   (501) staff       (20)      353 2023-07-10 23:01:18.000000 trycortex-py-1.0.1/trycortex_py.egg-info/PKG-INFO
+-rw-r--r--   0 charlespun   (501) staff       (20)      251 2023-07-10 23:01:18.000000 trycortex-py-1.0.1/trycortex_py.egg-info/SOURCES.txt
+-rw-r--r--   0 charlespun   (501) staff       (20)        1 2023-07-10 23:01:18.000000 trycortex-py-1.0.1/trycortex_py.egg-info/dependency_links.txt
+-rw-r--r--   0 charlespun   (501) staff       (20)       14 2023-07-10 23:01:18.000000 trycortex-py-1.0.1/trycortex_py.egg-info/requires.txt
+-rw-r--r--   0 charlespun   (501) staff       (20)        7 2023-07-10 23:01:18.000000 trycortex-py-1.0.1/trycortex_py.egg-info/top_level.txt
```

### Comparing `trycortex-py-1.0.0/cortex/api.py` & `trycortex-py-1.0.1/cortex/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from enum import Enum
 import requests
 from typing import List, Dict, Union, Any, Tuple
 
 class RetrievedDocument:
     def __init__(
         self,
@@ -259,14 +260,30 @@
         text: Union[str, None] = None,
         source_url: Union[str, None] = None
     ):
         self.timestamp = timestamp
         self.tags = tags
         self.text = text
         self.source_url = source_url
+    def getJson(self):
+        data = {}
+        if self.timestamp is not None:
+            data["timestamp"] = self.timestamp
+
+        if self.tags is not None:
+            data["tags"] = self.tags
+
+        if self.text is not None:
+            data["text"] = self.text
+
+        if self.source_url is not None:
+            data["source_url"] = self.source_url
+        
+        return json.dumps(data)
+
 
 class SharedVisibility:
     PRIVATE = "private"
     PUBLIC = "public"
     UNLISTED = "unlisted"
     DELETED = "deleted"
 
@@ -309,44 +326,45 @@
             },
             'method': 'GET',
         }
         endpoint = 'https://trycortex.ai/api/sdk/q/p'
         res = requests.request(**config, url=endpoint)
         return res.json().get('pID')
 
-    def getDocument(self, knowledgeName: str, documentID: str) -> Dict[str, Document]:
+    def getDocument(self, knowledgeName: str, documentID: str):
         if not self.userId:
             self.userId = self.getIDFromKey()
         config = {
             'headers': {
                 'Authorization': f'Bearer {self.apiKey}',
                 'Content-Type': 'application/json'
             },
             'method': 'GET',
         }
         endpoint = f'/{self.userId}/knowledge/{knowledgeName}/d/{documentID}'
         response = requests.request(**config, url=self.basePath + endpoint)
         return response.json()
 
-    def uploadDocument(self, knowledgeName: str, documentID: str, document: Dict[str, Union[str, None]]) -> Dict[str, Union[Document, Knowledge]]:
+    def uploadDocument(self, knowledgeName: str, documentID: str, document: CreateDocument):
         if not self.userId:
             self.userId = self.getIDFromKey()
+        data = document.getJson()
         config = {
             'headers': {
                 'Authorization': f'Bearer {self.apiKey}',
                 'Content-Type': 'application/json'
             },
             'method': 'POST',
-            'data': document,
+            'data': data,
         }
         endpoint = f'/{self.userId}/knowledge/{knowledgeName}/d/{documentID}'
         response = requests.request(**config, url=self.basePath + endpoint)
         return response.json()
 
-    def deleteDocument(self, knowledgeName: str, documentID: str) -> Dict[str, Document]:
+    def deleteDocument(self, knowledgeName: str, documentID: str):
         if not self.userId:
             self.userId = self.getIDFromKey()
         config = {
             'headers': {
                 'Authorization': f'Bearer {self.apiKey}',
                 'Content-Type': 'application/json'
             },
```

### Comparing `trycortex-py-1.0.0/setup.py` & `trycortex-py-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trycortex-py',
-    version='1.0.0',
+    version='1.0.1',
     description='A short description of your package',
     packages=find_packages(),
     install_requires=[
         'requests',
+        'json',
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     url='https://github.com/kinesysai/cortex-py',
```

