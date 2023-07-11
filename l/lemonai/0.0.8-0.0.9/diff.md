# Comparing `tmp/lemonai-0.0.8.tar.gz` & `tmp/lemonai-0.0.9.tar.gz`

## Comparing `lemonai-0.0.8.tar` & `lemonai-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.0.8/heatmap-example.gif
--rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.0.8/heatmap-example.png
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 lemonai-0.0.8/test.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 lemonai-0.0.8/.vscode/launch.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.8/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.8/LICENSE
--rw-r--r--   0        0        0    12607 2020-02-02 00:00:00.000000 lemonai-0.0.8/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 lemonai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.0.9/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.0.9/heatmap-example.png
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 lemonai-0.0.9/test.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lemonai-0.0.9/.vscode/launch.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.9/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.9/LICENSE
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 lemonai-0.0.9/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 lemonai-0.0.9/PKG-INFO
```

### Comparing `lemonai-0.0.8/heatmap-example.gif` & `lemonai-0.0.9/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/heatmap-example.png` & `lemonai-0.0.9/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/src/lemonai/api_wrapper.py` & `lemonai-0.0.9/src/lemonai/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/src/lemonai/execute_workflow.py` & `lemonai-0.0.9/src/lemonai/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/src/lemonai/filter_tools.py` & `lemonai-0.0.9/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/src/lemonai/get_integrations.py` & `lemonai-0.0.9/src/lemonai/get_integrations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict, Tuple
 
 def get_apis_from_env() -> Tuple[Dict[str, str], Dict[str, str]]:
 
     api_key_search_strings = ['_API_KEY', '_SECRET_KEY', '_SUBSCRIPTION_KEY', '_ACCESS_KEY']
-    access_token_search_strings = ['_ACCESS_TOKEN', '_SECRET_TOKEN']
+    access_token_search_strings = ['_ACCESS_TOKEN', '_SECRET_TOKEN', '_WEBHOOK_URL']
 
     api_keys = {}
     access_tokens = {}
 
     for key, value in os.environ.items():
         for search_string in api_key_search_strings:
             if search_string in key:
```

### Comparing `lemonai-0.0.8/src/lemonai/tool.py` & `lemonai-0.0.9/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/src/lemonai/toolkit.py` & `lemonai-0.0.9/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/.gitignore` & `lemonai-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/LICENSE` & `lemonai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.8/README.md` & `lemonai-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -261,27 +261,31 @@
 - Update database page: notion-update-database-page
 - Archive page: notion-archive-page
 - Create page: notion-create-page
 - Search page: notion-search-page
 - Get user: notion-get-user
 - Get all users: notion-get-many-user
 
+### Discord
+
+- Send message in channel: discord-message-send
+
 
 ## ❤️‍🔥 Next Up
 
 - [x] Github
 - [x] Notion
+- [x] Discord
 - [ ] Gmail
 - [ ] Google Calendar
 - [ ] Kafka
 - [ ] Pipedrive
 - [ ] Monday.com
 - [ ] Stripe
 - [ ] Medium
-- [ ] Discord
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
 
 
 ## Contributing
 
 Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```

### Comparing `lemonai-0.0.8/pyproject.toml` & `lemonai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.0.8/PKG-INFO` & `lemonai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -277,27 +277,31 @@
 - Update database page: notion-update-database-page
 - Archive page: notion-archive-page
 - Create page: notion-create-page
 - Search page: notion-search-page
 - Get user: notion-get-user
 - Get all users: notion-get-many-user
 
+### Discord
+
+- Send message in channel: discord-message-send
+
 
 ## ❤️‍🔥 Next Up
 
 - [x] Github
 - [x] Notion
+- [x] Discord
 - [ ] Gmail
 - [ ] Google Calendar
 - [ ] Kafka
 - [ ] Pipedrive
 - [ ] Monday.com
 - [ ] Stripe
 - [ ] Medium
-- [ ] Discord
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
 
 
 ## Contributing
 
 Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```

