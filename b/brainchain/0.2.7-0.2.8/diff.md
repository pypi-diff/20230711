# Comparing `tmp/brainchain-0.2.7.tar.gz` & `tmp/brainchain-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.2.7.tar", max compression
+gzip compressed data, was "brainchain-0.2.8.tar", max compression
```

## Comparing `brainchain-0.2.7.tar` & `brainchain-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.2.7/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.2.7/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.2.7/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.2.7/brainchain/__init__.py
--rw-r--r--   0        0        0     4900 2023-07-11 17:40:06.191841 brainchain-0.2.7/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.2.7/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.2.7/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.2.7/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.2.7/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.2.7/brainchain/sales_intel.py
--rw-r--r--   0        0        0      531 2023-07-11 17:40:19.169209 brainchain-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.2.8/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.2.8/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.2.8/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.2.8/brainchain/__init__.py
+-rw-r--r--   0        0        0     4960 2023-07-11 17:43:37.939287 brainchain-0.2.8/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.2.8/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.2.8/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.2.8/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.2.8/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.2.8/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      531 2023-07-11 17:43:42.083604 brainchain-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.2.8/PKG-INFO
```

### Comparing `brainchain-0.2.7/brainchain/.aider.chat.history.md` & `brainchain-0.2.8/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/.aider.input.history` & `brainchain-0.2.8/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/README.md` & `brainchain-0.2.8/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/brainchain.py` & `brainchain-0.2.8/brainchain/brainchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,30 +60,32 @@
             params["document_text"] = text_first_page
 
         if url_link:
             params["url_link"] = url_link
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, params=params)
-        return json.loads(json.dumps(response.content))
+        content = response.content.decode('utf-8')
+        return json.loads(content)
 
     # Only use text_first_page - MUCH faster! url_link provided for testing across link types
     def obtain_authors(self, text_first_page: str = None, url_link: str = None):
         endpoint = self.services["pdf_authors"][self.env]
         params = {}
 
         if text_first_page:
             params["document_text"] = text_first_page
 
         if url_link:
             params["url_link"] = url_link
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, params=params)
-        return json.loads(json.dumps(response.content))
+        content = response.content.decode('utf-8')
+        return json.loads(content)
 
     def summon(self, prompt, agent_type="CCR", model="gpt-4-0613", max_tokens=2048, temperature=0.18, top_p=0.15, top_k=0.0, presence_penalty=1.0, frequency_penalty=1.0):
         endpoint = self.services["agent"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
             "env": self.env,
```

### Comparing `brainchain-0.2.7/brainchain/carnivore.py` & `brainchain-0.2.8/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/coredata.py` & `brainchain-0.2.8/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/factcheck.py` & `brainchain-0.2.8/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/requirements.txt` & `brainchain-0.2.8/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/brainchain/sales_intel.py` & `brainchain-0.2.8/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.2.7/pyproject.toml` & `brainchain-0.2.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.2.7"
+version = "0.2.8"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.90"
```

### Comparing `brainchain-0.2.7/PKG-INFO` & `brainchain-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.2.7
+Version: 0.2.8
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

