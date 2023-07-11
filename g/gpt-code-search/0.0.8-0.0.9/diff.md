# Comparing `tmp/gpt_code_search-0.0.8.tar.gz` & `tmp/gpt_code_search-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.8.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.9.tar", max compression
```

## Comparing `gpt_code_search-0.0.8.tar` & `gpt_code_search-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.8/LICENSE
--rw-r--r--   0        0        0     8156 2023-06-27 04:09:02.164847 gpt_code_search-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.8/core/__init__.py
--rw-r--r--   0        0        0     6341 2023-06-27 12:16:50.622152 gpt_code_search-0.0.8/core/ai.py
--rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.8/core/analytics.py
--rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.8/core/config.py
--rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.8/core/functions.py
--rw-r--r--   0        0        0     3207 2023-06-26 16:06:16.220339 gpt_code_search-0.0.8/core/main.py
--rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.8/core/tests/__init__.py
--rw-r--r--   0        0        0      968 2023-06-26 14:44:25.615029 gpt_code_search-0.0.8/core/tests/test_truncate_text.py
--rw-r--r--   0        0        0     1292 2023-06-26 16:08:28.094693 gpt_code_search-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9515 1970-01-01 00:00:00.000000 gpt_code_search-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 05:10:24.301708 gpt_code_search-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7401 2023-07-11 05:10:53.940860 gpt_code_search-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 05:10:24.301925 gpt_code_search-0.0.9/core/__init__.py
+-rw-r--r--   0        0        0     6682 2023-07-11 05:10:24.302080 gpt_code_search-0.0.9/core/ai.py
+-rw-r--r--   0        0        0     1104 2023-07-11 05:10:24.302175 gpt_code_search-0.0.9/core/analytics.py
+-rw-r--r--   0        0        0     3154 2023-07-11 05:10:24.302267 gpt_code_search-0.0.9/core/config.py
+-rw-r--r--   0        0        0     7695 2023-07-11 05:12:39.478123 gpt_code_search-0.0.9/core/functions.py
+-rw-r--r--   0        0        0     3421 2023-07-11 05:10:24.302525 gpt_code_search-0.0.9/core/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 05:10:24.302603 gpt_code_search-0.0.9/core/tests/__init__.py
+-rw-r--r--   0        0        0      968 2023-07-11 05:10:24.302711 gpt_code_search-0.0.9/core/tests/test_truncate_text.py
+-rw-r--r--   0        0        0     1266 2023-07-11 05:10:53.939009 gpt_code_search-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8800 1970-01-01 00:00:00.000000 gpt_code_search-0.0.9/PKG-INFO
```

### Comparing `gpt_code_search-0.0.8/LICENSE` & `gpt_code_search-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.8/README.md` & `gpt_code_search-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 <div align="center">
   <h1>gpt-code-search</h1>
   <img
     height="240"
     width="240"
     alt="logo"
-    src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
+    src="https://raw.githubusercontent.com/narenmanoharan/gpt-code-search/main/public/logo.png"
   />
   <p>
-    <b>gpt-code-search</b> is an AI-powered tool enabling you to search your codebase with natural language. It utilizes GPT-4 to retrieve, search and answer queries about your code, boosting productivity and code understanding.
+    <b>gpt-code-search</b> is a tool enabling you to search your codebase with natural language. It utilizes OpenAI's function calling to retrieve, search and answer queries about your code, boosting productivity and code understanding.
   </p>
 </div>
 
-Learn more about the motivation behind this project in our announcement [blog post](https://wolfia.com/blog/announcing-gpt-code-search).
-
 ## Features
 
-- 🧠 **GPT-4**: Code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+- 🧠 **GPT-4**: Code search, retrieval, and answering all done with OpenAI's [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
 - 🔐 **Privacy-first**: Code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
 - 🔥 **Works instantly**: No pre-processing, chunking, or indexing, get started right away.
 - 📦 **File-system backed**: Works with any code on your machine.
 
 ## Getting Started
 
 ### Installation
@@ -56,53 +54,51 @@
 
 #### Select a model to use
 
 ```bash
 gcs select-model
 ```
 
-Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `~/$HOME/.gpt-code-search/config.toml`.
+Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `$HOME/.gpt-code-search/config.toml`.
 
 
 ### Configuration
 
 The tool will prompt you to configure the `OPENAI_API_KEY`, if you haven't already.
 
 ## Problem
 
-You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service.
+You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service (other than OpenAI).
 
-This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
+This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
 - 🛠️ Generate new code based on existing files and conventions
 - 📨 Ask general questions about any part of the codebase
 
 ## How it works
 
-This tool utilizes [OpenAI's function calling](https://platform.openai.com/docs/guides/gpt/function-calling) to allow GPT to call functions in your codebase. This enables us to automatically upload context directly from the file system on-demand, without having to manually copy and paste code snippets. This also means that no code is sent to any third-party service (other than OpenAI), only the question you ask and the code snippets that are requested by the LLM.
+We utilize OpenAI's function calling to let GPT-4 call certain predefined functions in our library. You do not need to implement any of these functions yourself. These functions are designed to interact with your codebase and return enough context for the LLM to perform code searches without pre-indexing it or uploading your repo to a third party other than OpenAI. So, you only need to run the tool from the directory you want to search.
 
 <img src="public/architecture.png" width="650" />
 
 The functions currently available for the LLM to call are:
 
 - `search_codebase` - searches the codebase using a TF-IDF vectorizer
 - `get_file_tree` - provides the file tree of the codebase
 - `get_file_contents` - provides the contents of a file
 
-Combining these three functions, we can ask the LLM to search the codebase for a keyword, and then retrieve the contents of the file that contains the keyword. And it's as simple as that!
+These functions are implemented in `gpt-code-search` and are triggered by chat completions. The LLM is prompted to utilize the search_codebase and get_file_tree function as needed to find the necessary context to answer your query and then loops as needed to collect more context with the get_file_contents until the LLM responds.
 
 ### Privacy
 
-Outside of the LLM, no data is sent or stored.
-
-The only data sent to LLM is the question you ask and the code snippets that it requests related to your question. All code snippets are retrieved from your local machine.
+This tool prioritizes privacy. Outside of the LLM, no code is sent to us and is only used as context for the LLM. We do collect anonymous usage data to improve the tool, but you can opt out of this.
 
 ## Limitations
 
 This does have some limitations, namely:
 
 - The LLM is unable to load context across multiple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
 - Specify the file name and keywords in your question to improve accuracy. For example, if you want to ask a question about `analytics.py`, mention the file name in your question.
@@ -115,20 +111,14 @@
 - [ ] Use vector embeddings to improve search and retrieval
 - [ ] Add support for generating code and saving it to a file
 - [ ] Support for searching across multiple codebases
 - [ ] Allow the model to create new functions that it can then execute
 - [ ] Use [guidance](https://github.com/microsoft/guidance) to improve prompts
 - [ ] Add support for additional models (Claude, Bedrock, etc)
 
-## Wolfia Codex
-
-`gpt-code-search` is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
-
-If you're looking for a more powerful tool which solves the above limitations by using vector embeddings and a more powerful search and retrieval system, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
-
 ## Analytics
 
 We collect anonymous crash and usage data to help us improve the tool. This data aids in understanding usage patterns and improving the tool. You can opt out of analytics by running:
 
 ```bash
 gcs opt-out-of-analytics
 ```
@@ -154,16 +144,16 @@
 
 ## Code of Conduct
 
 We are committed to fostering a welcoming community. To ensure that everyone feels safe and welcome, we have a [Code of Conduct](CODE_OF_CONDUCT.md) that all contributors, maintainers, and users of this project are expected to adhere to.
 
 ## Support
 
-If you're having trouble using `gpt-code-search`, feel free to [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) on our GitHub. You can also reach out to us directly at [support@wolfia.com](mailto:support@wolfia.com). We're always happy to help!
+If you're having trouble using `gpt-code-search`, feel free to [open an issue](https://github.com/narenmanoharan/gpt-code-search/issues) on our GitHub. You can also reach out to us directly at [narenkmanoharan@gmail.com](mailto:narenkmanoharan@gmail.com). We're always happy to help!
 
 ## Feedback
 
-Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) with your suggestions, or you can email [support@wolfia.com](mailto:support@wolfia.com).
+Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/narenmanoharan/gpt-code-search/issues) or reach out to us directly at [narenkmanoharan@gmail](mailto:narenkmanoharan@gmail) with your feedback or thoughts.
 
 ## License
 
-Apache 2.0 © [Wolfia](https://wolfia.com)
+This project is licensed under the terms of the [Apache 2.0](LICENSE).
```

### Comparing `gpt_code_search-0.0.8/core/ai.py` & `gpt_code_search-0.0.9/core/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import json
 import logging
+from typing import List
 
 import openai
 import requests
 from rich.markdown import Markdown
 
-from core.config import load_selected_model
+from core.config import load_selected_model, load_max_tokens
 from core.functions import (
     enabled_functions,
     get_contents_of_file,
     search_codebase,
     truncate_text_to_token_limit,
     get_file_tree,
 )
 
-# Reduced from 16k to 14k to allow for prompt context
-MAX_TOKENS = 14_000
 
 PROMPT = """\
 You're a superpowered coding assistant. Your role is to help users understand and navigate their codebases,
 providing assistance across a range of tasks.
 
 You have access to three primary functions:
 
@@ -54,14 +53,26 @@
 contents of the file and review the contents of at least three files before answering.
 
 Compose responses in markdown with code when necessary. Your objective is to provide the most accurate and detailed
 answer possible, even if it results in a longer response. Let's start assisting with your coding tasks!
 """
 
 
+def get_available_models() -> List:
+    token_mapping = {"16k": 14000, "32k": 30000}
+    return [
+        {
+            "name": model["id"],
+            "max_tokens": next((token_mapping[part] for part in model["id"].split("-") if part in token_mapping), 6000),
+        }
+        for model in openai.Model.list().data
+        if model["id"].startswith("gpt")
+    ]
+
+
 def chat_completion_request(messages, functions=None):
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + openai.api_key,
     }
     json_data = {
         "model": load_selected_model(),
@@ -118,15 +129,15 @@
     elif function_name == "get_file_tree":
         function_call = get_file_tree
         start_path = function_args.get("start_path")
         function_response = function_call(start_path)
     else:
         raise ValueError(f"Function {function_name} not found.")
 
-    truncated_response = truncate_text_to_token_limit(function_response, MAX_TOKENS)
+    truncated_response = truncate_text_to_token_limit(function_response, load_max_tokens())
 
     messages.append(
         {
             "role": "function",
             "name": function_name,
             "content": truncated_response,
         }
```

### Comparing `gpt_code_search-0.0.8/core/analytics.py` & `gpt_code_search-0.0.9/core/analytics.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.8/core/config.py` & `gpt_code_search-0.0.9/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 import uuid
 from datetime import datetime
 from pathlib import Path
 
 import toml
 
+from core import ai
 from core.analytics import send_event, configure_sentry, configure_posthog
 
-CONFIG_FILE_PATH = os.path.join(Path.home(), ".gpt-code-search/config.toml")
 
-models = ["gpt-4-0613", "gpt-3.5-turbo-0613", "gpt-3.5-turbo-16k"]
+CONFIG_FILE_PATH = os.path.join(Path.home(), ".gpt-code-search/config.toml")
 
 
 def create_or_update_with_default_config():
     default_config = {
         "id": str(uuid.uuid4()),
         "model": "gpt-3.5-turbo-16k",
+        "max_tokens": 14_000,
         "usage": {"query_count": 0, "query_at": "", "query_execution_time": ""},
         "analytics": "enabled",
     }
 
     existing_config = {}
     if os.path.exists(CONFIG_FILE_PATH):
         with open(CONFIG_FILE_PATH, "r") as config_file:
@@ -34,21 +35,27 @@
     os.makedirs(os.path.dirname(CONFIG_FILE_PATH), exist_ok=True)
     with open(CONFIG_FILE_PATH, "w") as config_file:
         toml.dump(existing_config, config_file)
 
 
 def load_selected_model():
     config = load_config()
-    model = config.get("model")
-    if model not in models:
+    selected_model = config.get("model")
+    models = [model["name"] for model in ai.get_available_models()]
+    if selected_model not in models:
         raise ValueError(
-            f"Invalid model {model}. Valid models are {models}. "
+            f"Invalid model {selected_model}. Valid models are {models}. "
             f"Please run `gpt-code-search select-model` to select a valid model."
         )
-    return model
+    return selected_model
+
+
+def load_max_tokens():
+    config = load_config()
+    return config.get("max_tokens")
 
 
 def log_usage_info(start_time, end_time):
     config = load_config()
     config["usage"]["query_count"] += 1
     config["usage"]["query_at"] = datetime.utcnow().isoformat()
     execution_time = (end_time - start_time).total_seconds()
@@ -71,16 +78,16 @@
 
 
 def unique_id():
     config = load_config()
     return config["id"]
 
 
-def save_selected_model(selected_model):
-    config = {"model": selected_model}
+def save_selected_model(selected_model, selected_model_max_tokens):
+    config = {"model": selected_model, "max_tokens": selected_model_max_tokens}
     with open(CONFIG_FILE_PATH, "w") as config_file:
         toml.dump(config, config_file)
 
 
 def load_config():
     create_or_update_with_default_config()
     with open(CONFIG_FILE_PATH, "r") as config_file:
```

### Comparing `gpt_code_search-0.0.8/core/functions.py` & `gpt_code_search-0.0.9/core/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import fnmatch
 from typing import List, Union, Tuple
 
 import tiktoken
 from sklearn.feature_extraction.text import TfidfVectorizer
 
 IGNORED_FOLDERS = [
     "__pycache__",
@@ -44,15 +45,15 @@
     :param depth: The current depth of the search.
     :return: The file tree.
     """
     if depth > max_depth:
         return []
     tree = []
     for item in os.listdir(start_path):
-        if item in IGNORED_FOLDERS or item in IGNORED_FILES:
+        if item in IGNORED_FOLDERS or any(fnmatch.fnmatch(item, pattern) for pattern in IGNORED_FILES):
             continue
         item_path = os.path.join(start_path, item)
         if os.path.isfile(item_path):
             tree.append(item_path)
         elif os.path.isdir(item_path):
             tree += get_file_tree(item_path, max_depth, depth + 1)
     return tree
```

### Comparing `gpt_code_search-0.0.8/core/main.py` & `gpt_code_search-0.0.9/core/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import os
 from datetime import datetime
 
 import typer
 from rich.console import Console
 from rich.logging import RichHandler
 
-from core.ai import chat_completions
+from core.ai import chat_completions, get_available_models
 from core.config import (
     save_selected_model,
     log_usage_info,
     CONFIG_FILE_PATH,
     create_or_update_with_default_config,
     save_opt_out_of_analytics,
     configure_deps,
 )
 
+
 logging.basicConfig(
     level=logging.INFO,
     format="%(message)s",
     datefmt="[%X]",
     handlers=[RichHandler(rich_tracebacks=True, markup=True)],
 )
 
@@ -44,24 +45,27 @@
 
 
 @app.command()
 def select_model():
     """
     Select the GPT model to use.
     """
-    models = ["gpt-4-0613", "gpt-3.5-turbo-0613", "gpt-3.5-turbo-16k"]
+    model_name = [model["name"] for model in get_available_models()]
+    model_max_tokens = [model["max_tokens"] for model in get_available_models()]
     console.print("Available Models:")
-    for index, model in enumerate(models, start=1):
+    for index, model in enumerate(model_name, start=1):
         console.print(f"{index}. {model}")
+    console.print("")
 
-    selected_model = typer.prompt("Select a model (enter the number)")
-    if selected_model.isdigit() and int(selected_model) in range(1, len(models) + 1):
-        selected_model_name = models[int(selected_model) - 1]
+    model_index = typer.prompt("Select a model (enter the number)")
+    if model_index.isdigit() and int(model_index) in range(1, len(model_name) + 1):
+        selected_model_name = model_name[int(model_index) - 1]
+        selected_max_tokens = model_max_tokens[int(model_index) - 1]
         console.print(f"Selected model: {selected_model_name}")
-        save_selected_model(selected_model_name)
+        save_selected_model(selected_model_name, selected_max_tokens)
     else:
         console.print("Invalid selection. Please enter a valid number.")
         typer.Exit()
 
 
 @app.command()
 def query(message: str):
```

### Comparing `gpt_code_search-0.0.8/core/tests/test_truncate_text.py` & `gpt_code_search-0.0.9/core/tests/test_truncate_text.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.8/pyproject.toml` & `gpt_code_search-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.8"
+version = "0.0.9"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
-homepage = "https://wolfia.com"
-repository = "https://github.com/wolfia-app/gpt-code-search"
-keywords = ["gpt", "code", "search", "wolfia", "gpt4", "llm"]
+repository = "https://github.com/narenmanoharan/gpt-code-search"
+keywords = ["gpt", "code", "search", "gpt4", "llm"]
 
 [tool.poetry.urls]
-issues = "https://github.com/wolfia-app/gpt-code-search/issues"
-discussions = "https://github.com/wolfia-app/gpt-code-search/discussions"
-wiki = "https://github.com/wolfia-app/gpt-code-search/wiki"
+issues = "https://github.com/narenmanoharan/gpt-code-search/issues"
+discussions = "https://github.com/narenmanoharan/gpt-code-search/discussions"
+wiki = "https://github.com/narenmanoharan/gpt-code-search/wiki"
 
 [tool.poetry.scripts]
 gpt-code-search = "core.main:app"
 gcs = "core.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.17"
```

### Comparing `gpt_code_search-0.0.8/PKG-INFO` & `gpt_code_search-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gpt-code-search
-Version: 0.0.8
+Version: 0.0.9
 Summary: gpt-code-search enables you to search your codebase with natural language.
-Home-page: https://wolfia.com
+Home-page: https://github.com/narenmanoharan/gpt-code-search
 License: Apache-2.0
-Keywords: gpt,code,search,wolfia,gpt4,llm
+Keywords: gpt,code,search,gpt4,llm
 Author: narenmanoharan
 Author-email: narenkmanoharan@gmail.com
 Requires-Python: >=3.8.17,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,38 +19,36 @@
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: sentry-sdk[flask] (>=1.26.0,<2.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
-Project-URL: Repository, https://github.com/wolfia-app/gpt-code-search
-Project-URL: discussions, https://github.com/wolfia-app/gpt-code-search/discussions
-Project-URL: issues, https://github.com/wolfia-app/gpt-code-search/issues
-Project-URL: wiki, https://github.com/wolfia-app/gpt-code-search/wiki
+Project-URL: Repository, https://github.com/narenmanoharan/gpt-code-search
+Project-URL: discussions, https://github.com/narenmanoharan/gpt-code-search/discussions
+Project-URL: issues, https://github.com/narenmanoharan/gpt-code-search/issues
+Project-URL: wiki, https://github.com/narenmanoharan/gpt-code-search/wiki
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>gpt-code-search</h1>
   <img
     height="240"
     width="240"
     alt="logo"
-    src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
+    src="https://raw.githubusercontent.com/narenmanoharan/gpt-code-search/main/public/logo.png"
   />
   <p>
-    <b>gpt-code-search</b> is an AI-powered tool enabling you to search your codebase with natural language. It utilizes GPT-4 to retrieve, search and answer queries about your code, boosting productivity and code understanding.
+    <b>gpt-code-search</b> is a tool enabling you to search your codebase with natural language. It utilizes OpenAI's function calling to retrieve, search and answer queries about your code, boosting productivity and code understanding.
   </p>
 </div>
 
-Learn more about the motivation behind this project in our announcement [blog post](https://wolfia.com/blog/announcing-gpt-code-search).
-
 ## Features
 
-- 🧠 **GPT-4**: Code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+- 🧠 **GPT-4**: Code search, retrieval, and answering all done with OpenAI's [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
 - 🔐 **Privacy-first**: Code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
 - 🔥 **Works instantly**: No pre-processing, chunking, or indexing, get started right away.
 - 📦 **File-system backed**: Works with any code on your machine.
 
 ## Getting Started
 
 ### Installation
@@ -87,53 +85,51 @@
 
 #### Select a model to use
 
 ```bash
 gcs select-model
 ```
 
-Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `~/$HOME/.gpt-code-search/config.toml`.
+Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `$HOME/.gpt-code-search/config.toml`.
 
 
 ### Configuration
 
 The tool will prompt you to configure the `OPENAI_API_KEY`, if you haven't already.
 
 ## Problem
 
-You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service.
+You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service (other than OpenAI).
 
-This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
+This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
 - 🛠️ Generate new code based on existing files and conventions
 - 📨 Ask general questions about any part of the codebase
 
 ## How it works
 
-This tool utilizes [OpenAI's function calling](https://platform.openai.com/docs/guides/gpt/function-calling) to allow GPT to call functions in your codebase. This enables us to automatically upload context directly from the file system on-demand, without having to manually copy and paste code snippets. This also means that no code is sent to any third-party service (other than OpenAI), only the question you ask and the code snippets that are requested by the LLM.
+We utilize OpenAI's function calling to let GPT-4 call certain predefined functions in our library. You do not need to implement any of these functions yourself. These functions are designed to interact with your codebase and return enough context for the LLM to perform code searches without pre-indexing it or uploading your repo to a third party other than OpenAI. So, you only need to run the tool from the directory you want to search.
 
 <img src="public/architecture.png" width="650" />
 
 The functions currently available for the LLM to call are:
 
 - `search_codebase` - searches the codebase using a TF-IDF vectorizer
 - `get_file_tree` - provides the file tree of the codebase
 - `get_file_contents` - provides the contents of a file
 
-Combining these three functions, we can ask the LLM to search the codebase for a keyword, and then retrieve the contents of the file that contains the keyword. And it's as simple as that!
+These functions are implemented in `gpt-code-search` and are triggered by chat completions. The LLM is prompted to utilize the search_codebase and get_file_tree function as needed to find the necessary context to answer your query and then loops as needed to collect more context with the get_file_contents until the LLM responds.
 
 ### Privacy
 
-Outside of the LLM, no data is sent or stored.
-
-The only data sent to LLM is the question you ask and the code snippets that it requests related to your question. All code snippets are retrieved from your local machine.
+This tool prioritizes privacy. Outside of the LLM, no code is sent to us and is only used as context for the LLM. We do collect anonymous usage data to improve the tool, but you can opt out of this.
 
 ## Limitations
 
 This does have some limitations, namely:
 
 - The LLM is unable to load context across multiple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
 - Specify the file name and keywords in your question to improve accuracy. For example, if you want to ask a question about `analytics.py`, mention the file name in your question.
@@ -146,20 +142,14 @@
 - [ ] Use vector embeddings to improve search and retrieval
 - [ ] Add support for generating code and saving it to a file
 - [ ] Support for searching across multiple codebases
 - [ ] Allow the model to create new functions that it can then execute
 - [ ] Use [guidance](https://github.com/microsoft/guidance) to improve prompts
 - [ ] Add support for additional models (Claude, Bedrock, etc)
 
-## Wolfia Codex
-
-`gpt-code-search` is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
-
-If you're looking for a more powerful tool which solves the above limitations by using vector embeddings and a more powerful search and retrieval system, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
-
 ## Analytics
 
 We collect anonymous crash and usage data to help us improve the tool. This data aids in understanding usage patterns and improving the tool. You can opt out of analytics by running:
 
 ```bash
 gcs opt-out-of-analytics
 ```
@@ -185,17 +175,17 @@
 
 ## Code of Conduct
 
 We are committed to fostering a welcoming community. To ensure that everyone feels safe and welcome, we have a [Code of Conduct](CODE_OF_CONDUCT.md) that all contributors, maintainers, and users of this project are expected to adhere to.
 
 ## Support
 
-If you're having trouble using `gpt-code-search`, feel free to [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) on our GitHub. You can also reach out to us directly at [support@wolfia.com](mailto:support@wolfia.com). We're always happy to help!
+If you're having trouble using `gpt-code-search`, feel free to [open an issue](https://github.com/narenmanoharan/gpt-code-search/issues) on our GitHub. You can also reach out to us directly at [narenkmanoharan@gmail.com](mailto:narenkmanoharan@gmail.com). We're always happy to help!
 
 ## Feedback
 
-Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) with your suggestions, or you can email [support@wolfia.com](mailto:support@wolfia.com).
+Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/narenmanoharan/gpt-code-search/issues) or reach out to us directly at [narenkmanoharan@gmail](mailto:narenkmanoharan@gmail) with your feedback or thoughts.
 
 ## License
 
-Apache 2.0 © [Wolfia](https://wolfia.com)
+This project is licensed under the terms of the [Apache 2.0](LICENSE).
```

