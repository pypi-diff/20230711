# Comparing `tmp/pqapi-0.0.2.tar.gz` & `tmp/pqapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqapi-0.0.2.tar", last modified: Thu Jun  8 14:42:45 2023, max compression
+gzip compressed data, was "pqapi-0.1.0.tar", last modified: Tue Jul 11 07:23:57 2023, max compression
```

## Comparing `pqapi-0.0.2.tar` & `pqapi-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 14:42:08.000000 pqapi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 14:42:45.628440 pqapi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 14:42:08.000000 pqapi-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/pqapi/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/pqapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 14:42:08.000000 pqapi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:42:45.628440 pqapi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 14:42:08.000000 pqapi-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-08 14:42:08.000000 pqapi-0.0.2/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:23:57.349243 pqapi-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 07:23:30.000000 pqapi-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-11 07:23:57.349243 pqapi-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-11 07:23:30.000000 pqapi-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:23:57.345243 pqapi-0.1.0/pqapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 07:23:30.000000 pqapi-0.1.0/pqapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-11 07:23:30.000000 pqapi-0.1.0/pqapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 07:23:30.000000 pqapi-0.1.0/pqapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-11 07:23:30.000000 pqapi-0.1.0/pqapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 07:23:30.000000 pqapi-0.1.0/pqapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:23:57.349243 pqapi-0.1.0/pqapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-11 07:23:57.000000 pqapi-0.1.0/pqapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 07:23:57.000000 pqapi-0.1.0/pqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:23:57.000000 pqapi-0.1.0/pqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 07:23:57.000000 pqapi-0.1.0/pqapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 07:23:57.000000 pqapi-0.1.0/pqapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 07:23:30.000000 pqapi-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 07:23:57.349243 pqapi-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 07:23:30.000000 pqapi-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:23:57.349243 pqapi-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-11 07:23:30.000000 pqapi-0.1.0/tests/test_api.py
```

### Comparing `pqapi-0.0.2/LICENSE` & `pqapi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqapi-0.0.2/PKG-INFO` & `pqapi-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 0.0.2
+Version: 0.1.0
 Summary: API for interacting with paperqa.app
 Home-page: https://github.com/Future-House/pqapi
 Author: Andrew White
 Author-email: andrew@futurehouse.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,30 +12,41 @@
 License-File: LICENSE
 
 # peperqa-api
 Python UI for interacting with paperqa app
 
 # Usage
 
-Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
+Make sure to set the environment variable `PQA_API_KEY` to your API token.
 
 ```sh
-export PAPERQA_API_TOKEN=pqa-...
+export PQA_API_KEY=pqa-...
 ```
 
 To query agent:
 
 ```py
 import pqapi
 response = pqapi.agent_query(
     "default",
     "Are COVID-19 vaccines effective?"
 )
 ```
 
+to remove bibliography after querying (to avoid memory)
+```py
+import pqapi
+response = pqapi.agent_query(
+    "tmp",
+    "Are COVID-19 vaccines effective?",
+    delete_after=True
+)
+```
+
+
 ## Managing bibliographies
 
 
 To get information about a specific bibliography
 
 ```py
 import pqapi
```

### Comparing `pqapi-0.0.2/README.md` & `pqapi-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 # peperqa-api
 Python UI for interacting with paperqa app
 
 # Usage
 
-Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
+Make sure to set the environment variable `PQA_API_KEY` to your API token.
 
 ```sh
-export PAPERQA_API_TOKEN=pqa-...
+export PQA_API_KEY=pqa-...
 ```
 
 To query agent:
 
 ```py
 import pqapi
 response = pqapi.agent_query(
     "default",
     "Are COVID-19 vaccines effective?"
 )
 ```
 
+to remove bibliography after querying (to avoid memory)
+```py
+import pqapi
+response = pqapi.agent_query(
+    "tmp",
+    "Are COVID-19 vaccines effective?",
+    delete_after=True
+)
+```
+
+
 ## Managing bibliographies
 
 
 To get information about a specific bibliography
 
 ```py
 import pqapi
@@ -51,8 +62,8 @@
 To delete a bibliography:
 
 ```py
 import pqapi
 response = pqapi.delete_bibliography(
     "default"
 )
-```
+```
```

### Comparing `pqapi-0.0.2/pqapi/api.py` & `pqapi-0.1.0/pqapi/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,18 +58,23 @@
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         response.raise_for_status()
         result = DocsStatus(**response.json())
         return result
 
 
-def agent_query(bibliography: str, query: Union[QueryRequest, str]) -> AnswerResponse:
+def agent_query(
+    bibliography: str, query: Union[QueryRequest, str], delete_after: bool = False
+) -> AnswerResponse:
     if isinstance(query, str):
         query = QueryRequest(query=query)
+    print(query.query)
     url = f"https://paperqa.app/api/agent/{bibliography}"
     with requests.Session() as session:
         response = session.post(
             url, json=query.dict(), headers={"Authorization": f"Bearer {get_pqa_key()}"}
         )
         response.raise_for_status()
         result = AnswerResponse(**response.json())
-        return result
+    if delete_after:
+        delete_bibliography(bibliography)
+    return result
```

### Comparing `pqapi-0.0.2/pqapi.egg-info/PKG-INFO` & `pqapi-0.1.0/pqapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 0.0.2
+Version: 0.1.0
 Summary: API for interacting with paperqa.app
 Home-page: https://github.com/Future-House/pqapi
 Author: Andrew White
 Author-email: andrew@futurehouse.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,30 +12,41 @@
 License-File: LICENSE
 
 # peperqa-api
 Python UI for interacting with paperqa app
 
 # Usage
 
-Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
+Make sure to set the environment variable `PQA_API_KEY` to your API token.
 
 ```sh
-export PAPERQA_API_TOKEN=pqa-...
+export PQA_API_KEY=pqa-...
 ```
 
 To query agent:
 
 ```py
 import pqapi
 response = pqapi.agent_query(
     "default",
     "Are COVID-19 vaccines effective?"
 )
 ```
 
+to remove bibliography after querying (to avoid memory)
+```py
+import pqapi
+response = pqapi.agent_query(
+    "tmp",
+    "Are COVID-19 vaccines effective?",
+    delete_after=True
+)
+```
+
+
 ## Managing bibliographies
 
 
 To get information about a specific bibliography
 
 ```py
 import pqapi
```

### Comparing `pqapi-0.0.2/setup.py` & `pqapi-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pqapi-0.0.2/tests/test_api.py` & `pqapi-0.1.0/tests/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,29 @@
     response = agent_query("default", "How are bispecific antibodies engineered?")
     assert isinstance(response, AnswerResponse)
 
 
 def test_query_model():
     response = agent_query(
         "default",
-        QueryRequest(
-            query="How are bispecific antibodies engineered?", llm="gpt-3.5-turbo"
-        ),
+        QueryRequest(query="How are bispecific antibodies engineered?"),
     )
     assert isinstance(response, AnswerResponse)
 
 
+def test_delete_after():
+    response = agent_query(
+        "tmp",
+        QueryRequest(query="How are bispecific antibodies engineered?"),
+        delete_after=True,
+    )
+    assert isinstance(response, AnswerResponse)
+    assert get_bibliography("tmp").doc_count == 0
+
+
 def test_upload_files():
     script_dir = os.path.dirname(__file__)
     file = open(os.path.join(script_dir, "paper.pdf"), "rb")
     response = upload_files(
         "default",
         [file],
         [UploadMetadata(filename="paper.pdf", citation="Test Citation")],
```

