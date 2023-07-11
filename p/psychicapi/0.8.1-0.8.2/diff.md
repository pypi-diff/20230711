# Comparing `tmp/psychicapi-0.8.1.tar.gz` & `tmp/psychicapi-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.8.1.tar", last modified: Mon Jul 10 00:23:53 2023, max compression
+gzip compressed data, was "psychicapi-0.8.2.tar", last modified: Tue Jul 11 00:20:55 2023, max compression
```

## Comparing `psychicapi-0.8.1.tar` & `psychicapi-0.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.478316 psychicapi-0.8.1/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-10 00:23:53.478184 psychicapi-0.8.1/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4271 2023-07-10 00:22:36.000000 psychicapi-0.8.1/README.md
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.477341 psychicapi-0.8.1/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-07-07 03:04:36.000000 psychicapi-0.8.1/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     8870 2023-07-10 00:21:30.000000 psychicapi-0.8.1/psychicapi/psychic.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.478028 psychicapi-0.8.1/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-07-10 00:23:53.478355 psychicapi-0.8.1/setup.cfg
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-07-10 00:23:00.000000 psychicapi-0.8.1/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.713343 psychicapi-0.8.2/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-11 00:20:55.713222 psychicapi-0.8.2/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4271 2023-07-10 00:22:36.000000 psychicapi-0.8.2/README.md
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.712410 psychicapi-0.8.2/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-07-07 03:04:36.000000 psychicapi-0.8.2/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)    11229 2023-07-10 23:48:43.000000 psychicapi-0.8.2/psychicapi/psychic.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.713061 psychicapi-0.8.2/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-07-11 00:20:55.713385 psychicapi-0.8.2/setup.cfg
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-07-10 23:49:15.000000 psychicapi-0.8.2/setup.py
```

### Comparing `psychicapi-0.8.1/PKG-INFO` & `psychicapi-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.8.1
+Version: 0.8.2
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.8.1/README.md` & `psychicapi-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.8.1/psychicapi/psychic.py` & `psychicapi-0.8.2/psychicapi/psychic.py`

 * *Files 18% similar despite different names*

```diff
@@ -103,14 +103,24 @@
 
     def __init__(
         self, documents: List[Dict], next_page_cursor: Optional[str] = None
     ) -> None:
         self.documents = documents
         self.next_page_cursor = next_page_cursor
 
+class GetTicketsResponse:
+    tickets: List[Dict]
+    next_page_cursor: Optional[str] = None
+
+    def __init__(
+        self, tickets: List[Dict], next_page_cursor: Optional[str] = None
+    ) -> None:
+        self.tickets = tickets
+        self.next_page_cursor = next_page_cursor
+
 
 class ChunkingOptions:
     min_chunk_size: Optional[int] = None
     max_chunk_size: Optional[int] = None
 
 
 class Psychic:
@@ -281,7 +291,76 @@
             next_page_cursor = data["next_page_cursor"]
             return GetConversationsResponse(
                 messages=messages, next_page_cursor=next_page_cursor
             )
 
         else:
             self.handle_http_error(response)
+
+    def get_conversations(
+        self,
+        *,
+        account_id: str,
+        connector_id: ConnectorId,
+        page_cursor: Optional[str] = None,
+        oldest_timestamp: Optional[int] = None,
+    ):
+        body = {
+            "connector_id": connector_id.value,
+            "account_id": account_id,
+            "page_cursor": page_cursor,
+        }
+        if oldest_timestamp is not None:
+            body["oldest_timestamp"] = oldest_timestamp
+
+        response = requests.post(
+            self.api_url + "get-conversations",
+            json=body,
+            headers={
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
+        )
+        if response.status_code == 200:
+            data = response.json()
+            messages = data["messages"]
+            next_page_cursor = data["next_page_cursor"]
+            return GetConversationsResponse(
+                messages=messages, next_page_cursor=next_page_cursor
+            )
+
+        else:
+            self.handle_http_error(response)
+
+    def get_tickets(
+        self,
+        *,
+        account_id: str,
+        connector_id: ConnectorId,
+        redact_pii: Optional[bool] = False,
+        page_cursor: Optional[str] = None,
+    ):
+        body = {
+            "connector_id": connector_id.value,
+            "account_id": account_id,
+            "redact_pii": redact_pii,
+            "page_cursor": page_cursor,
+        }
+
+        response = requests.post(
+            self.api_url + "get-tickets",
+            json=body,
+            headers={
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
+        )
+        if response.status_code == 200:
+            data = response.json()
+            tickets = data["tickets"]
+            next_page_cursor = data["next_page_cursor"]
+            return GetTicketsResponse(
+                tickets=tickets, next_page_cursor=next_page_cursor
+            )
+
+        else:
+            self.handle_http_error(response)
```

### Comparing `psychicapi-0.8.1/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.8.2/psychicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.8.1
+Version: 0.8.2
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.8.1/setup.py` & `psychicapi-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.8.1',
+    version='0.8.2',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

