# Comparing `tmp/BlitzChain-0.5.1.tar.gz` & `tmp/BlitzChain-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.5.1.tar", last modified: Sun Jul  9 13:27:45 2023, max compression
+gzip compressed data, was "BlitzChain-0.6.0.tar", last modified: Tue Jul 11 11:33:20 2023, max compression
```

## Comparing `BlitzChain-0.5.1.tar` & `BlitzChain-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.887178 BlitzChain-0.5.1/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.882551 BlitzChain-0.5.1/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.5.1/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 13:27:45.886882 BlitzChain-0.5.1/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.5.1/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.883931 BlitzChain-0.5.1/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-09 13:27:33.000000 BlitzChain-0.5.1/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     6471 2023-07-09 13:27:28.000000 BlitzChain-0.5.1/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.5.1/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.5.1/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.884631 BlitzChain-0.5.1/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.5.1/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.5.1/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-09 13:27:45.887283 BlitzChain-0.5.1/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.5.1/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.886296 BlitzChain-0.5.1/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.5.1/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.5.1/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.5.1/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-11 11:33:20.166841 BlitzChain-0.6.0/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-11 11:33:20.161909 BlitzChain-0.6.0/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      398 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       40 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/entry_points.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-11 11:33:20.000000 BlitzChain-0.6.0/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.6.0/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-11 11:33:20.166561 BlitzChain-0.6.0/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3436 2023-07-09 13:29:34.000000 BlitzChain-0.6.0/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-11 11:33:20.163557 BlitzChain-0.6.0/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-11 11:33:08.000000 BlitzChain-0.6.0/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     7421 2023-07-11 11:33:10.000000 BlitzChain-0.6.0/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.6.0/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.6.0/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-11 11:33:20.164465 BlitzChain-0.6.0/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-07-09 14:53:24.000000 BlitzChain-0.6.0/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      432 2023-07-09 14:53:44.000000 BlitzChain-0.6.0/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-11 11:33:20.166930 BlitzChain-0.6.0/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      475 2023-07-10 01:54:16.000000 BlitzChain-0.6.0/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-11 11:33:20.166038 BlitzChain-0.6.0/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.6.0/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.6.0/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.6.0/tests/test_qa.py
```

### Comparing `BlitzChain-0.5.1/LICENSE` & `BlitzChain-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.1/README.md` & `BlitzChain-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 Retrieval-Augmented Generation For Powerful Results
 
 ## Installation
 
 ```
-pip install -e git+https://github.com/mr-gpt/blitzchain.git#egg=blitzchain
+pip install blitzchain
 ```
 
 Once you install, you can get your API key from https://app.twilix.io/
 
 If you would like to then use this for your solutions, we recommend the following: 
 
 ## QuickStart
```

### Comparing `BlitzChain-0.5.1/blitzchain/api.py` & `BlitzChain-0.6.0/blitzchain/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,196 +1,240 @@
 """The API behind BlitzChain
 """
+import json
+import base64
 import requests
 from typing import List
 from .splitter import WordSplitter
 
+
 def get_json_response(response):
     try:
         return response.json()
     except Exception as e:
         return response.content
 
+
 class Client:
     def __init__(self, api_key: str):
         self.api_key = api_key
         self.base_url = "https://app.twilix.io/api/v1/"
-    
+
     def Collection(self, collection_name: str):
         return Collection(api_key=self.api_key, collection_name=collection_name)
-    
+
     def list_collections(self):
         response = requests.get(
             url=self.base_url + "collection/list",
             headers={
-                "Content-Type": "application/json", 
-                "Authorization": "Bearer " + self.api_key
-            }
+                "Content-Type": "application/json",
+                "Authorization": "Bearer " + self.api_key,
+            },
         )
         return get_json_response(response)
 
+
 class Collection:
     def __init__(self, api_key: str, collection_name: str):
         self.collection_name = collection_name
         self.api_key = api_key
         self.base_url = "https://app.twilix.io/api/v1/"
-    
+
     def insert_objects(
         self,
         objects: list,
-        fields_for_vectorization: list=None,
+        fields_for_vectorization: list = None,
         split_on_field: str = None,
-        wait_to_finish=True
+        wait_to_finish=True,
     ):
         if wait_to_finish:
             url = self.base_url + "collection/bulk-insert"
         else:
             raise NotImplementedError
             # url = self.base_url + "collection/async-bulk-insert"
-        
+
         response = requests.post(
             url,
             headers={
-                "Content-Type": "application/json", 
-                "Authorization": "Bearer " + self.api_key
+                "Content-Type": "application/json",
+                "Authorization": "Bearer " + self.api_key,
             },
             json={
                 "collection": self.collection_name,
                 "objects": objects,
                 "fieldsForVectorization": fields_for_vectorization,
-                "splitOnField": split_on_field
-            }
+                "splitOnField": split_on_field,
+            },
         )
         if not wait_to_finish:
-            return response.status_code == 200, "Request failed - please make sure parameters are correct."
+            return (
+                response.status_code == 200,
+                "Request failed - please make sure parameters are correct.",
+            )
         return get_json_response(response)
-    
+
     def insert_pdf(self, url: str):
         api_url = self.base_url + "collection/insert-pdf"
         print(api_url)
         response = requests.post(
             api_url,
             headers={
                 # "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer "
+                + self.api_key
             },
-            json={
-                "collection": self.collection_name,
-                "url": url
-            }
+            json={"collection": self.collection_name, "url": url},
         )
         return get_json_response(response)
 
-    def insert_html(self, html: str, metadata: dict=None):
+    def insert_html(self, html: str, metadata: dict = None):
         api_url = self.base_url + "collection/insert-html"
         response = requests.post(
             api_url,
             headers={
                 "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer " + self.api_key,
             },
             json={
                 "collection": self.collection_name,
                 "html": html,
-                "metadata": metadata
-            }
+                "metadata": metadata,
+            },
         )
         return get_json_response(response)
-    
-    def generative_qa(self, user_input: str, prompt_fields: list,
-        conversation_id: str=None, limit: int=5, fields: list=None,
-        include_rerank: bool=False, minimum_rerank_score: float=0.7,
-        include_moderation: bool=False
+
+    def generative_qa(
+        self,
+        user_input: str,
+        prompt_fields: list,
+        conversation_id: str = None,
+        limit: int = 5,
+        fields: list = None,
+        include_rerank: bool = False,
+        minimum_rerank_score: float = 0.7,
+        include_moderation: bool = False,
     ):
-        """Get an answer based on a question that you ask.
-        """
-        url =  self.base_url + "collection/generative-qa"
+        """Get an answer based on a question that you ask."""
+        url = self.base_url + "collection/generative-qa"
         print(url)
-        data={
+        data = {
             "collection": self.collection_name,
             "userInput": user_input,
             "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
-            "include_moderation": include_moderation
+            "include_moderation": include_moderation,
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
             headers={
                 "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer " + self.api_key,
             },
-            json=data
+            json=data,
         )
         return get_json_response(response)
 
-    def copilot(self, user_input: str, prompt_fields: list,
-        conversation_id: str=None, limit: int=5, fields: list=None,
-        include_rerank: bool=False, minimum_rerank_score: float=0.7,
-        include_moderation: bool=False
+    def copilot(
+        self,
+        user_input: str,
+        prompt_fields: list,
+        conversation_id: str = None,
+        limit: int = 5,
+        fields: list = None,
+        include_rerank: bool = False,
+        minimum_rerank_score: float = 0.7,
+        include_moderation: bool = False,
     ):
-        """Get an answer based on a question that you ask.
-        """
-        url =  self.base_url + "collection/generative-code-qa"
+        """Get an answer based on a question that you ask."""
+        url = self.base_url + "collection/generative-code-qa"
         print(url)
-        data={
+        data = {
             "collection": self.collection_name,
             "userInput": user_input,
             "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
-            "includeModeration": include_moderation
+            "includeModeration": include_moderation,
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
             headers={
                 "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer " + self.api_key,
             },
-            json=data
+            json=data,
         )
         return get_json_response(response)
 
-    def list_objects(self, limit: int=5, offset: int=0, 
-            fields: list=None, where=None, sort:list=None):
+    def list_objects(
+        self,
+        limit: int = 5,
+        offset: int = 0,
+        fields: list = None,
+        where=None,
+        sort: list = None,
+    ):
         api_url = self.base_url + "object/list"
         print(api_url)
         response = requests.post(
             api_url,
             headers={
                 "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer " + self.api_key,
             },
             json={
                 "collection": self.collection_name,
                 "limit": limit,
                 "offset": offset,
                 "fields": fields,
                 "where": where,
-                "sort": sort
-            }
+                "sort": sort,
+            },
         )
         return get_json_response(response)
-    
+
     def count(self):
         api_url = self.base_url + "object/count"
         response = requests.get(
             api_url,
             headers={
                 "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.api_key
+                "Authorization": "Bearer " + self.api_key,
             },
             params={
                 "collection": self.collection_name,
-            }
+            },
         )
         return get_json_response(response)
+
+    def launch_dashboard(
+        self, name: str, description: str, prompt_fields: List[str] = None
+    ):
+        """Launch Dashboard"""
+        if prompt_fields is None:
+            prompt_fields = ["autoGen_content"]
+        encoding = base64.urlsafe_b64encode(
+            json.dumps(
+                {
+                    "path": "graph-weaver",
+                    "name": name,
+                    "collection": self.collection_name,
+                    "promptFields": prompt_fields,
+                    "apiKey": self.api_key,
+                    "description": description,
+                }
+            ).encode()
+        )
+        token = encoding.decode()
+        link = "https://ask.twilix.io/custom?token=" + token
+        print(link)
```

### Comparing `BlitzChain-0.5.1/blitzchain/splitter.py` & `BlitzChain-0.6.0/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.1/blitzchain/utils.py` & `BlitzChain-0.6.0/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.1/tests/test_pdf.py` & `BlitzChain-0.6.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.1/tests/test_qa.py` & `BlitzChain-0.6.0/tests/test_qa.py`

 * *Files identical despite different names*

