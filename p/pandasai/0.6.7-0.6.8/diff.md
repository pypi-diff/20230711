# Comparing `tmp/pandasai-0.6.7.tar.gz` & `tmp/pandasai-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.7.tar", max compression
+gzip compressed data, was "pandasai-0.6.8.tar", max compression
```

## Comparing `pandasai-0.6.7.tar` & `pandasai-0.6.8.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1055 2023-06-29 00:29:00.294691 pandasai-0.6.7/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-29 00:29:00.294691 pandasai-0.6.7/README.md
--rw-r--r--   0        0        0    25266 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3471 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11156 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-29 00:29:00.302691 pandasai-0.6.7/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3176 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-06-29 00:29:00.306691 pandasai-0.6.7/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-06-29 00:29:00.306691 pandasai-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-10 23:04:58.032892 pandasai-0.6.8/LICENSE
+-rw-r--r--   0        0        0     7705 2023-07-10 23:04:58.032892 pandasai-0.6.8/README.md
+-rw-r--r--   0        0        0    25302 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3116 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3507 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11442 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3176 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-07-10 23:04:58.040892 pandasai-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.8/PKG-INFO
```

### Comparing `pandasai-0.6.7/LICENSE` & `pandasai-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/README.md` & `pandasai-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/__init__.py` & `pandasai-0.6.8/pandasai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,15 @@
                 self._check_imports(node)
                 continue
             if self._is_df_overwrite(node):
                 continue
             new_body.append(node)
 
         new_tree = ast.Module(body=new_body)
-        return astor.to_source(new_tree).strip()
+        return astor.to_source(new_tree, pretty_source=lambda x: "".join(x)).strip()
 
     def _get_environment(self) -> dict:
         """
         Returns the environment for the code to be executed.
 
         Returns (dict): A dictionary of environment variables
         """
```

### Comparing `pandasai-0.6.7/pandasai/constants.py` & `pandasai-0.6.8/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/exceptions.py` & `pandasai-0.6.8/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/_optional.py` & `pandasai-0.6.8/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/anonymizer.py` & `pandasai-0.6.8/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/cache.py` & `pandasai-0.6.8/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/from_excel.py` & `pandasai-0.6.8/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/notebook.py` & `pandasai-0.6.8/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/helpers/save_chart.py` & `pandasai-0.6.8/pandasai/helpers/save_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,8 +109,8 @@
 
     chart_save_msg = f"Charts saving to: {chart_save_dir}"
     if print_save_dir:
         print(chart_save_msg)
     logging.info(chart_save_msg)
 
     new_tree = ast.Module(body=new_body)
-    return astor.to_source(new_tree).strip()
+    return astor.to_source(new_tree, pretty_source=lambda x: "".join(x)).strip()
```

### Comparing `pandasai-0.6.7/pandasai/helpers/shortcuts.py` & `pandasai-0.6.8/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/azure_openai.py` & `pandasai-0.6.8/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/base.py` & `pandasai-0.6.8/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 from ..helpers._optional import import_dependency
+from ..helpers.openai_info import openai_callback_var
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
@@ -211,14 +212,18 @@
         params = {**self._default_params, "prompt": prompt}
 
         if self.stop is not None:
             params["stop"] = [self.stop]
 
         response = openai.Completion.create(**params)
 
+        openai_handler = openai_callback_var.get()
+        if openai_handler:
+            openai_handler(response)
+
         return response["choices"][0]["text"]
 
     def chat_completion(self, value: str) -> str:
         """
         Query the chat completion API
 
         Args:
@@ -238,14 +243,18 @@
         }
 
         if self.stop is not None:
             params["stop"] = [self.stop]
 
         response = openai.ChatCompletion.create(**params)
 
+        openai_handler = openai_callback_var.get()
+        if openai_handler:
+            openai_handler(response)
+
         return response["choices"][0]["message"]["content"]
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
 
     LLM base class is extended to be used with HuggingFace LLM Modes APIs
```

### Comparing `pandasai-0.6.7/pandasai/llm/fake.py` & `pandasai-0.6.8/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/falcon.py` & `pandasai-0.6.8/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/google_palm.py` & `pandasai-0.6.8/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/langchain.py` & `pandasai-0.6.8/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/open_assistant.py` & `pandasai-0.6.8/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/llm/openai.py` & `pandasai-0.6.8/pandasai/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 load_dotenv()
 
 
 class OpenAI(BaseOpenAI):
     """OpenAI LLM using BaseOpenAI Class.
 
-    An API call to OpenAi API is sent and response is recorded and returned.
+    An API call to OpenAI API is sent and response is recorded and returned.
     The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only
     supported completion model.
     The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",
      "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].
 
     """
 
@@ -50,15 +50,15 @@
         self,
         api_token: Optional[str] = None,
         **kwargs,
     ):
         """
         __init__ method of OpenAI Class
         Args:
-            api_token (str): API Token fro OpenAI platform.
+            api_token (str): API Token for OpenAI platform.
             **kwargs: Extended Parameters inferred from BaseOpenAI class
 
         Returns: Response generated from OpenAI API
         """
 
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
```

### Comparing `pandasai-0.6.7/pandasai/llm/starcoder.py` & `pandasai-0.6.8/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/middlewares/base.py` & `pandasai-0.6.8/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/middlewares/charts.py` & `pandasai-0.6.8/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/middlewares/streamlit.py` & `pandasai-0.6.8/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/prompts/base.py` & `pandasai-0.6.8/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.8/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.8/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.8/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.8/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.7/pyproject.toml` & `pandasai-0.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.7"
+version = "0.6.8"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.7/PKG-INFO` & `pandasai-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.7
+Version: 0.6.8
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

