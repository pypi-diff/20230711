# Comparing `tmp/anthropic-0.3.3.tar.gz` & `tmp/anthropic-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.3.3.tar", max compression
+gzip compressed data, was "anthropic-0.3.4.tar", max compression
```

## Comparing `anthropic-0.3.3.tar` & `anthropic-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.3/LICENSE
--rw-r--r--   0        0        0     9665 2023-07-06 16:11:28.620017 anthropic-0.3.3/README.md
--rw-r--r--   0        0        0     1905 2023-07-11 00:15:56.592396 anthropic-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.3/src/anthropic/__init__.py
--rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.3/src/anthropic/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.3/src/anthropic/_base_exceptions.py
--rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.3/src/anthropic/_client.py
--rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.3/src/anthropic/_constants.py
--rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.3/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.3/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.3/src/anthropic/_qs.py
--rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.3/src/anthropic/_resource.py
--rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.3/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1186 2023-07-06 16:11:28.620372 anthropic-0.3.3/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.3/src/anthropic/_types.py
--rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.3/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.3/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.3/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0      100 2023-07-11 00:15:56.592686 anthropic-0.3.3/src/anthropic/_version.py
--rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.3/src/anthropic/pagination.py
--rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.3/src/anthropic/py.typed
--rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.3/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    33226 2023-07-11 00:15:56.593099 anthropic-0.3.3/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.3/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.3/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.3/src/anthropic/types/completion.py
--rw-r--r--   0        0        0    12185 2023-06-26 21:50:36.641096 anthropic-0.3.3/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0    10606 1970-01-01 00:00:00.000000 anthropic-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.4/LICENSE
+-rw-r--r--   0        0        0     9665 2023-07-11 13:43:09.482168 anthropic-0.3.4/README.md
+-rw-r--r--   0        0        0     1925 2023-07-11 13:43:09.483979 anthropic-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.4/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.4/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.4/src/anthropic/_base_exceptions.py
+-rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.4/src/anthropic/_client.py
+-rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.4/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.4/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.4/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.4/src/anthropic/_qs.py
+-rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.4/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.4/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.4/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.4/src/anthropic/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.4/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.4/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.4/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      128 2023-07-11 13:43:09.485358 anthropic-0.3.4/src/anthropic/_version.py
+-rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.4/src/anthropic/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.4/src/anthropic/py.typed
+-rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.4/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    21486 2023-07-11 13:43:09.485792 anthropic-0.3.4/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.4/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.4/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.4/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0     7015 2023-07-11 13:43:09.486237 anthropic-0.3.4/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0    10618 1970-01-01 00:00:00.000000 anthropic-0.3.4/PKG-INFO
```

### Comparing `anthropic-0.3.3/LICENSE` & `anthropic-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/README.md` & `anthropic-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 anthropic = Anthropic(
     # defaults to os.environ.get("ANTHROPIC_API_KEY")
     api_key="my api key",
 )
 
 completion = anthropic.completions.create(
-    model="claude-1",
+    model="claude-2",
     max_tokens_to_sample=300,
     prompt=f"{HUMAN_PROMPT} how does a court case get to the Supreme Court? {AI_PROMPT}",
 )
 print(completion.completion)
 ```
 
 While you can provide an `api_key` keyword argument, we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
@@ -112,15 +112,15 @@
     # defaults to os.environ.get("ANTHROPIC_API_KEY")
     api_key="my api key",
 )
 
 
 async def main():
     completion = await anthropic.completions.create(
-        model="claude-1",
+        model="claude-2",
         max_tokens_to_sample=300,
         prompt=f"{HUMAN_PROMPT} how does a court case get to the Supreme Court? {AI_PROMPT}",
     )
     print(completion.completion)
 
 
 asyncio.run(main())
@@ -136,15 +136,15 @@
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 anthropic = Anthropic()
 
 stream = anthropic.completions.create(
     prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
     stream=True,
 )
 for completion in stream:
     print(completion.completion)
 ```
 
 The async client uses the exact same interface.
@@ -153,15 +153,15 @@
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 anthropic = AsyncAnthropic()
 
 stream = await anthropic.completions.create(
     prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
     stream=True,
 )
 async for completion in stream:
     print(completion.completion)
 ```
 
 ## Using Types
@@ -184,15 +184,15 @@
 
 anthropic = Anthropic()
 
 try:
     anthropic.completions.create(
         prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
         max_tokens_to_sample=300,
-        model="claude-1",
+        model="claude-2",
     )
 except anthropic.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except anthropic.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except anthropic.APIStatusError as e:
@@ -231,15 +231,15 @@
     max_retries=0,
 )
 
 # Or, configure per-request:
 anthropic.with_options(max_retries=5).completions.create(
     prompt=f"{HUMAN_PROMPT} Can you help me effectively ask for a raise at work? {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
 )
 ```
 
 ### Timeouts
 
 Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
@@ -258,15 +258,15 @@
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 anthropic.with_options(timeout=5 * 1000).completions.create(
     prompt=f"{HUMAN_PROMPT} Where can I get a good coffee in my neighbourhood? {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests which time out will be [retried twice by default](#retries).
```

### Comparing `anthropic-0.3.3/pyproject.toml` & `anthropic-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "anthropic"
-version = "0.3.3"
+version = "0.3.4"
 description = "Client library for the anthropic API"
 readme = "README.md"
 authors = ["Anthropic <support@anthropic.com>"]
 license = "MIT"
 repository = "https://github.com/anthropics/anthropic-sdk-python"
 packages = [
   { include = "anthropic", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-httpx = ">= 0.23.0"
+httpx = ">= 0.23.0, < 1"
 pydantic = "^1.9.0"
-typing-extensions = ">= 4.1.1"
-anyio = ">= 3.5.0"
-distro = ">= 1.7.0"
+typing-extensions = ">= 4.1.1, < 5"
+anyio = ">= 3.5.0, < 4"
+distro = ">= 1.7.0, < 2"
 tokenizers = ">= 0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pyright = "1.1.297"
 mypy = "1.1.1"
 black = "22.10.0"
 respx = "0.19.2"
```

### Comparing `anthropic-0.3.3/src/anthropic/__init__.py` & `anthropic-0.3.4/src/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_base_client.py` & `anthropic-0.3.4/src/anthropic/_base_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_base_exceptions.py` & `anthropic-0.3.4/src/anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_client.py` & `anthropic-0.3.4/src/anthropic/_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_exceptions.py` & `anthropic-0.3.4/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_models.py` & `anthropic-0.3.4/src/anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_qs.py` & `anthropic-0.3.4/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_resource.py` & `anthropic-0.3.4/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_streaming.py` & `anthropic-0.3.4/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_tokenizers.py` & `anthropic-0.3.4/src/anthropic/_tokenizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 
 def sync_get_tokenizer() -> Tokenizer:
     if _tokenizer is not None:
         return _tokenizer
 
     tokenizer_path = _get_tokenizer_cache_path()
-    text = tokenizer_path.read_text(encoding='utf-8')
+    text = tokenizer_path.read_text(encoding="utf-8")
     return _load_tokenizer(text)
 
 
 async def async_get_tokenizer() -> Tokenizer:
     if _tokenizer is not None:
         return _tokenizer
 
     tokenizer_path = AsyncPath(_get_tokenizer_cache_path())
-    text = await tokenizer_path.read_text(encoding='utf-8')
+    text = await tokenizer_path.read_text(encoding="utf-8")
     return _load_tokenizer(text)
```

### Comparing `anthropic-0.3.3/src/anthropic/_types.py` & `anthropic-0.3.4/src/anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_utils/__init__.py` & `anthropic-0.3.4/src/anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_utils/_transform.py` & `anthropic-0.3.4/src/anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/_utils/_utils.py` & `anthropic-0.3.4/src/anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/tokenizer.json` & `anthropic-0.3.4/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/src/anthropic/types/completion.py` & `anthropic-0.3.4/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.3/PKG-INFO` & `anthropic-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.3.3
+Version: 0.3.4
 Summary: Client library for the anthropic API
 Home-page: https://github.com/anthropics/anthropic-sdk-python
 License: MIT
 Author: Anthropic
 Author-email: support@anthropic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anyio (>=3.5.0)
-Requires-Dist: distro (>=1.7.0)
-Requires-Dist: httpx (>=0.23.0)
+Requires-Dist: anyio (>=3.5.0,<4)
+Requires-Dist: distro (>=1.7.0,<2)
+Requires-Dist: httpx (>=0.23.0,<1)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: tokenizers (>=0.13.0)
-Requires-Dist: typing-extensions (>=4.1.1)
+Requires-Dist: typing-extensions (>=4.1.1,<5)
 Project-URL: Repository, https://github.com/anthropics/anthropic-sdk-python
 Description-Content-Type: text/markdown
 
 # Anthropic Python API Library
 
 [![PyPI version](https://img.shields.io/pypi/v/anthropic.svg)](https://pypi.org/project/anthropic/)
 
@@ -112,15 +112,15 @@
 
 anthropic = Anthropic(
     # defaults to os.environ.get("ANTHROPIC_API_KEY")
     api_key="my api key",
 )
 
 completion = anthropic.completions.create(
-    model="claude-1",
+    model="claude-2",
     max_tokens_to_sample=300,
     prompt=f"{HUMAN_PROMPT} how does a court case get to the Supreme Court? {AI_PROMPT}",
 )
 print(completion.completion)
 ```
 
 While you can provide an `api_key` keyword argument, we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
@@ -137,15 +137,15 @@
     # defaults to os.environ.get("ANTHROPIC_API_KEY")
     api_key="my api key",
 )
 
 
 async def main():
     completion = await anthropic.completions.create(
-        model="claude-1",
+        model="claude-2",
         max_tokens_to_sample=300,
         prompt=f"{HUMAN_PROMPT} how does a court case get to the Supreme Court? {AI_PROMPT}",
     )
     print(completion.completion)
 
 
 asyncio.run(main())
@@ -161,15 +161,15 @@
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 anthropic = Anthropic()
 
 stream = anthropic.completions.create(
     prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
     stream=True,
 )
 for completion in stream:
     print(completion.completion)
 ```
 
 The async client uses the exact same interface.
@@ -178,15 +178,15 @@
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 anthropic = AsyncAnthropic()
 
 stream = await anthropic.completions.create(
     prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
     stream=True,
 )
 async for completion in stream:
     print(completion.completion)
 ```
 
 ## Using Types
@@ -209,15 +209,15 @@
 
 anthropic = Anthropic()
 
 try:
     anthropic.completions.create(
         prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
         max_tokens_to_sample=300,
-        model="claude-1",
+        model="claude-2",
     )
 except anthropic.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except anthropic.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except anthropic.APIStatusError as e:
@@ -256,15 +256,15 @@
     max_retries=0,
 )
 
 # Or, configure per-request:
 anthropic.with_options(max_retries=5).completions.create(
     prompt=f"{HUMAN_PROMPT} Can you help me effectively ask for a raise at work? {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
 )
 ```
 
 ### Timeouts
 
 Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
@@ -283,15 +283,15 @@
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 anthropic.with_options(timeout=5 * 1000).completions.create(
     prompt=f"{HUMAN_PROMPT} Where can I get a good coffee in my neighbourhood? {AI_PROMPT}",
     max_tokens_to_sample=300,
-    model="claude-1",
+    model="claude-2",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests which time out will be [retried twice by default](#retries).
```

