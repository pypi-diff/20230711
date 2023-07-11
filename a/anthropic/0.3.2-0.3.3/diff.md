# Comparing `tmp/anthropic-0.3.2.tar.gz` & `tmp/anthropic-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.3.2.tar", max compression
+gzip compressed data, was "anthropic-0.3.3.tar", max compression
```

## Comparing `anthropic-0.3.2.tar` & `anthropic-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.2/LICENSE
--rw-r--r--   0        0        0     9666 2023-06-28 15:42:21.543919 anthropic-0.3.2/README.md
--rw-r--r--   0        0        0     1905 2023-07-01 00:21:15.453002 anthropic-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.2/src/anthropic/__init__.py
--rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.2/src/anthropic/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.2/src/anthropic/_base_exceptions.py
--rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.2/src/anthropic/_client.py
--rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.2/src/anthropic/_constants.py
--rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.2/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.2/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.2/src/anthropic/_qs.py
--rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.2/src/anthropic/_resource.py
--rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.2/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1154 2023-06-29 15:21:58.836551 anthropic-0.3.2/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.2/src/anthropic/_types.py
--rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.2/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.2/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.2/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0      100 2023-06-29 15:21:58.836805 anthropic-0.3.2/src/anthropic/_version.py
--rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.2/src/anthropic/pagination.py
--rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.2/src/anthropic/py.typed
--rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.2/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    33262 2023-06-26 21:50:36.631074 anthropic-0.3.2/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.2/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.2/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.2/src/anthropic/types/completion.py
--rw-r--r--   0        0        0    12185 2023-06-26 21:50:36.641096 anthropic-0.3.2/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0    10607 1970-01-01 00:00:00.000000 anthropic-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.3/LICENSE
+-rw-r--r--   0        0        0     9665 2023-07-06 16:11:28.620017 anthropic-0.3.3/README.md
+-rw-r--r--   0        0        0     1905 2023-07-11 00:15:56.592396 anthropic-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.3/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.3/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.3/src/anthropic/_base_exceptions.py
+-rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.3/src/anthropic/_client.py
+-rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.3/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.3/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.3/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.3/src/anthropic/_qs.py
+-rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.3/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.3/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1186 2023-07-06 16:11:28.620372 anthropic-0.3.3/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.3/src/anthropic/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.3/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.3/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.3/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      100 2023-07-11 00:15:56.592686 anthropic-0.3.3/src/anthropic/_version.py
+-rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.3/src/anthropic/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.3/src/anthropic/py.typed
+-rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.3/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    33226 2023-07-11 00:15:56.593099 anthropic-0.3.3/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.3/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.3/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.3/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0    12185 2023-06-26 21:50:36.641096 anthropic-0.3.3/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0    10606 1970-01-01 00:00:00.000000 anthropic-0.3.3/PKG-INFO
```

### Comparing `anthropic-0.3.2/LICENSE` & `anthropic-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/README.md` & `anthropic-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 **Sync before/after:**
 
 ```diff
 - client = anthropic.Client(os.environ["ANTHROPIC_API_KEY"])
 + client = anthropic.Anthropic(api_key=os.environ["ANTHROPIC_API_KEY"])
   # or, simply provide an ANTHROPIC_API_KEY environment variable:
-+ client = anthropic.Anthropic();
++ client = anthropic.Anthropic()
 
 - rsp = client.completion(**params)
 - rsp["completion"]
 + rsp = client.completions.create(**params)
 + rsp.completion
 ```
```

### Comparing `anthropic-0.3.2/pyproject.toml` & `anthropic-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic"
-version = "0.3.2"
+version = "0.3.3"
 description = "Client library for the anthropic API"
 readme = "README.md"
 authors = ["Anthropic <support@anthropic.com>"]
 license = "MIT"
 repository = "https://github.com/anthropics/anthropic-sdk-python"
 packages = [
   { include = "anthropic", from = "src" }
```

### Comparing `anthropic-0.3.2/src/anthropic/__init__.py` & `anthropic-0.3.3/src/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_base_client.py` & `anthropic-0.3.3/src/anthropic/_base_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_base_exceptions.py` & `anthropic-0.3.3/src/anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_client.py` & `anthropic-0.3.3/src/anthropic/_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_exceptions.py` & `anthropic-0.3.3/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_models.py` & `anthropic-0.3.3/src/anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_qs.py` & `anthropic-0.3.3/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_resource.py` & `anthropic-0.3.3/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_streaming.py` & `anthropic-0.3.3/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_tokenizers.py` & `anthropic-0.3.3/src/anthropic/_tokenizers.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 
 def sync_get_tokenizer() -> Tokenizer:
     if _tokenizer is not None:
         return _tokenizer
 
     tokenizer_path = _get_tokenizer_cache_path()
-    text = tokenizer_path.read_text()
+    text = tokenizer_path.read_text(encoding='utf-8')
     return _load_tokenizer(text)
 
 
 async def async_get_tokenizer() -> Tokenizer:
     if _tokenizer is not None:
         return _tokenizer
 
     tokenizer_path = AsyncPath(_get_tokenizer_cache_path())
-    text = await tokenizer_path.read_text()
+    text = await tokenizer_path.read_text(encoding='utf-8')
     return _load_tokenizer(text)
```

### Comparing `anthropic-0.3.2/src/anthropic/_types.py` & `anthropic-0.3.3/src/anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_utils/__init__.py` & `anthropic-0.3.3/src/anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_utils/_transform.py` & `anthropic-0.3.3/src/anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/_utils/_utils.py` & `anthropic-0.3.3/src/anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/resources/completions.py` & `anthropic-0.3.3/src/anthropic/resources/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> Completion:
         """
         Create a completion
 
         Args:
           max_tokens_to_sample: The maximum number of tokens to generate before stopping.
 
@@ -161,15 +161,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> Stream[Completion]:
         """
         Create a completion
 
         Args:
           max_tokens_to_sample: The maximum number of tokens to generate before stopping.
 
@@ -294,15 +294,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> Completion | Stream[Completion]:
         return self._post(
             "/v1/complete",
             body=maybe_transform(
                 {
                     "max_tokens_to_sample": max_tokens_to_sample,
                     "model": model,
@@ -340,15 +340,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> Completion:
         """
         Create a completion
 
         Args:
           max_tokens_to_sample: The maximum number of tokens to generate before stopping.
 
@@ -471,15 +471,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> AsyncStream[Completion]:
         """
         Create a completion
 
         Args:
           max_tokens_to_sample: The maximum number of tokens to generate before stopping.
 
@@ -604,15 +604,15 @@
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
+        timeout: float | None | NotGiven = 600,
     ) -> Completion | AsyncStream[Completion]:
         return await self._post(
             "/v1/complete",
             body=maybe_transform(
                 {
                     "max_tokens_to_sample": max_tokens_to_sample,
                     "model": model,
```

### Comparing `anthropic-0.3.2/src/anthropic/tokenizer.json` & `anthropic-0.3.3/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/types/completion.py` & `anthropic-0.3.3/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/src/anthropic/types/completion_create_params.py` & `anthropic-0.3.3/src/anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.2/PKG-INFO` & `anthropic-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Client library for the anthropic API
 Home-page: https://github.com/anthropics/anthropic-sdk-python
 License: MIT
 Author: Anthropic
 Author-email: support@anthropic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 
 **Sync before/after:**
 
 ```diff
 - client = anthropic.Client(os.environ["ANTHROPIC_API_KEY"])
 + client = anthropic.Anthropic(api_key=os.environ["ANTHROPIC_API_KEY"])
   # or, simply provide an ANTHROPIC_API_KEY environment variable:
-+ client = anthropic.Anthropic();
++ client = anthropic.Anthropic()
 
 - rsp = client.completion(**params)
 - rsp["completion"]
 + rsp = client.completions.create(**params)
 + rsp.completion
 ```
```

