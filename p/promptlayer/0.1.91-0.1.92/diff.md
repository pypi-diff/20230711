# Comparing `tmp/promptlayer-0.1.91.tar.gz` & `tmp/promptlayer-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.91.tar", last modified: Thu Jul  6 14:58:36 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.92.tar", last modified: Tue Jul 11 20:33:18 2023, max compression
```

## Comparing `promptlayer-0.1.91.tar` & `promptlayer-0.1.92.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.996017 promptlayer-0.1.91/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.91/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-06 14:58:36.995681 promptlayer-0.1.91/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3855 2023-07-06 14:55:00.000000 promptlayer-0.1.91/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.986876 promptlayer-0.1.91/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-22 17:22:46.000000 promptlayer-0.1.91/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.989372 promptlayer-0.1.91/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.91/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.990711 promptlayer-0.1.91/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.91/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.91/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.91/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.993464 promptlayer-0.1.91/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.91/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.91/promptlayer/prompts/chat.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.91/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.994809 promptlayer-0.1.91/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.91/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.91/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    12463 2023-07-06 14:55:00.000000 promptlayer-0.1.91/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.988941 promptlayer-0.1.91/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-07-06 14:58:36.996116 promptlayer-0.1.91/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-07-06 14:55:35.000000 promptlayer-0.1.91/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.393675 promptlayer-0.1.92/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.92/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-11 20:33:18.393347 promptlayer-0.1.92/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3855 2023-07-06 14:55:00.000000 promptlayer-0.1.92/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.383868 promptlayer-0.1.92/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-22 17:22:46.000000 promptlayer-0.1.92/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.386405 promptlayer-0.1.92/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.92/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.387308 promptlayer-0.1.92/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.92/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.92/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3085 2023-07-11 20:32:57.000000 promptlayer-0.1.92/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.390574 promptlayer-0.1.92/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.92/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.92/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.92/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.392202 promptlayer-0.1.92/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.92/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.92/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13309 2023-07-11 20:32:57.000000 promptlayer-0.1.92/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-11 20:33:18.386014 promptlayer-0.1.92/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-11 20:33:18.000000 promptlayer-0.1.92/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-07-11 20:33:18.000000 promptlayer-0.1.92/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-07-11 20:33:18.000000 promptlayer-0.1.92/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-07-11 20:33:18.000000 promptlayer-0.1.92/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-07-11 20:33:18.000000 promptlayer-0.1.92/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-07-11 20:33:18.393811 promptlayer-0.1.92/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-07-11 20:32:57.000000 promptlayer-0.1.92/setup.py
```

### Comparing `promptlayer-0.1.91/LICENSE` & `promptlayer-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/PKG-INFO` & `promptlayer-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.91
+Version: 0.1.92
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.91 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.92 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.91/README.md` & `promptlayer-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/__init__.py` & `promptlayer-0.1.92/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.92/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/promptlayer.py` & `promptlayer-0.1.92/promptlayer/promptlayer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import datetime
 import inspect
 
 from promptlayer.utils import (
     get_api_key,
     promptlayer_api_handler,
-    promptlayer_api_handler_async,
+    async_wrapper,
 )
 
 
 class PromptLayerBase(object):
     __slots__ = ["_obj", "__weakref__", "_function_name", "_provider_type"]
 
     def __init__(self, obj, function_name="", provider_type="openai"):
         object.__setattr__(self, "_obj", obj)
         object.__setattr__(self, "_function_name", function_name)
         object.__setattr__(self, "_provider_type", provider_type)
 
     def __getattr__(self, name):
         attr = getattr(object.__getattribute__(self, "_obj"), name)
-        if inspect.isclass(attr) or inspect.isfunction(attr) or inspect.ismethod(attr):
+        if (
+            inspect.isclass(attr)
+            or inspect.isfunction(attr)
+            or inspect.ismethod(attr)
+            or str(type(attr))
+            == "<class 'anthropic.resources.completions.Completions'>"
+            or str(type(attr))
+            == "<class 'anthropic.resources.completions.AsyncCompletions'>"
+        ):
             return PromptLayerBase(
                 attr,
                 function_name=f'{object.__getattribute__(self, "_function_name")}.{name}',
                 provider_type=object.__getattribute__(self, "_provider_type"),
             )
         return attr
 
@@ -41,40 +49,34 @@
         function_object = object.__getattribute__(self, "_obj")
         if inspect.isclass(function_object):
             return PromptLayerBase(
                 function_object(*args, **kwargs),
                 function_name=object.__getattribute__(self, "_function_name"),
                 provider_type=object.__getattribute__(self, "_provider_type"),
             )
-        if inspect.iscoroutinefunction(function_object):
-
-            async def async_wrapper(*args, **kwargs):
-                response = await function_object(*args, **kwargs)
-                request_end_time = datetime.datetime.now().timestamp()
-                return await promptlayer_api_handler_async(
-                    object.__getattribute__(self, "_function_name"),
-                    object.__getattribute__(self, "_provider_type"),
-                    args,
-                    kwargs,
-                    tags,
-                    response,
-                    request_start_time,
-                    request_end_time,
-                    get_api_key(),
-                    return_pl_id=return_pl_id,
-                )
-
-            return async_wrapper(*args, **kwargs)
-        response = function_object(*args, **kwargs)
+        function_response = function_object(*args, **kwargs)
+        if inspect.iscoroutinefunction(function_object) or inspect.iscoroutine(
+            function_response
+        ):
+            return async_wrapper(
+                function_response,
+                return_pl_id,
+                request_start_time,
+                object.__getattribute__(self, "_function_name"),
+                object.__getattribute__(self, "_provider_type"),
+                tags,
+                *args,
+                **kwargs,
+            )
         request_end_time = datetime.datetime.now().timestamp()
         return promptlayer_api_handler(
             object.__getattribute__(self, "_function_name"),
             object.__getattribute__(self, "_provider_type"),
             args,
             kwargs,
             tags,
-            response,
+            function_response,
             request_start_time,
             request_end_time,
             get_api_key(),
             return_pl_id=return_pl_id,
         )
```

### Comparing `promptlayer-0.1.91/promptlayer/prompts/chat.py` & `promptlayer-0.1.92/promptlayer/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/prompts/prompts.py` & `promptlayer-0.1.92/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/track/track.py` & `promptlayer-0.1.92/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/promptlayer/utils.py` & `promptlayer-0.1.92/promptlayer/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import contextvars
+import datetime
 import functools
 import os
 import sys
 import types
 from copy import deepcopy
 from json import JSONDecodeError
 
@@ -112,14 +113,18 @@
     api_key,
     return_pl_id=False,
     metadata=None,
 ):
     if type(response) != dict and hasattr(response, "to_dict_recursive"):
         response = response.to_dict_recursive()
     request_response = None
+    if hasattr(
+        response, "dict"
+    ):  # added this for anthropic 3.0 changes, they return a completion object
+        response = response.dict()
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/track-request",
             json={
                 "function_name": function_name,
                 "provider_type": provider_type,
                 "args": args,
@@ -129,15 +134,18 @@
                 "request_start_time": request_start_time,
                 "request_end_time": request_end_time,
                 "metadata": metadata,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            warn_on_bad_response(request_response, "WARNING: While logging your request PromptLayer had the following error")
+            warn_on_bad_response(
+                request_response,
+                "WARNING: While logging your request PromptLayer had the following error",
+            )
     except Exception as e:
         print(
             f"WARNING: While logging your request PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
     if request_response is not None and return_pl_id:
         return request_response.json().get("request_id")
@@ -183,15 +191,18 @@
             params={"prompt_name": prompt_name, "version": version},
         )
     except Exception as e:
         raise Exception(
             f"PromptLayer had the following error while getting your prompt: {e}"
         )
     if request_response.status_code != 200:
-        raise_on_bad_response(request_response, "PromptLayer had the following error while getting your prompt")
+        raise_on_bad_response(
+            request_response,
+            "PromptLayer had the following error while getting your prompt",
+        )
 
     return request_response.json()
 
 
 def promptlayer_publish_prompt(prompt_name, prompt_template, tags, api_key):
     try:
         request_response = requests.post(
@@ -204,15 +215,18 @@
             },
         )
     except Exception as e:
         raise Exception(
             f"PromptLayer had the following error while publishing your prompt: {e}"
         )
     if request_response.status_code != 200:
-        raise_on_bad_response(request_response, "PromptLayer had the following error while publishing your prompt")
+        raise_on_bad_response(
+            request_response,
+            "PromptLayer had the following error while publishing your prompt",
+        )
     return True
 
 
 def promptlayer_track_prompt(
     request_id, prompt_name, input_variables, api_key, version
 ):
     try:
@@ -223,15 +237,18 @@
                 "prompt_name": prompt_name,
                 "prompt_input_variables": input_variables,
                 "api_key": api_key,
                 "version": version,
             },
         )
         if request_response.status_code != 200:
-            warn_on_bad_response(request_response, "WARNING: While tracking your prompt PromptLayer had the following error")
+            warn_on_bad_response(
+                request_response,
+                "WARNING: While tracking your prompt PromptLayer had the following error",
+            )
             return False
     except Exception as e:
         print(
             f"WARNING: While tracking your prompt PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
@@ -245,15 +262,18 @@
             json={
                 "request_id": request_id,
                 "metadata": metadata,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            warn_on_bad_response(request_response, "WARNING: While tracking your metadata PromptLayer had the following error")
+            warn_on_bad_response(
+                request_response,
+                "WARNING: While tracking your metadata PromptLayer had the following error",
+            )
             return False
     except Exception as e:
         print(
             f"WARNING: While tracking your metadata PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
@@ -267,15 +287,18 @@
             json={
                 "request_id": request_id,
                 "score": score,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            warn_on_bad_response(request_response, "WARNING: While tracking your score PromptLayer had the following error")
+            warn_on_bad_response(
+                request_response,
+                "WARNING: While tracking your score PromptLayer had the following error",
+            )
             return False
     except Exception as e:
         print(
             f"WARNING: While tracking your score PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
@@ -368,36 +391,52 @@
 
 
 def warn_on_bad_response(request_response, main_message):
     if hasattr(request_response, "json"):
         try:
             print(
                 f"{main_message}: {request_response.json().get('message')}",
-                file=sys.stderr
+                file=sys.stderr,
             )
         except JSONDecodeError:
             print(
                 f"{main_message}: {request_response}",
                 file=sys.stderr,
             )
     else:
-        print(
-            f"{main_message}: {request_response}",
-            file=sys.stderr
-        )
+        print(f"{main_message}: {request_response}", file=sys.stderr)
 
 
 def raise_on_bad_response(request_response, main_message):
     if hasattr(request_response, "json"):
         try:
-            raise Exception(
-                f"{main_message}: {request_response.json().get('message')}"
-            )
+            raise Exception(f"{main_message}: {request_response.json().get('message')}")
         except JSONDecodeError:
-            raise Exception(
-                f"{main_message}: {request_response}"
-            )
+            raise Exception(f"{main_message}: {request_response}")
     else:
-        raise Exception(
-            f"{main_message}: {request_response}"
-        )
+        raise Exception(f"{main_message}: {request_response}")
+
 
+async def async_wrapper(
+    coroutine_obj,
+    return_pl_id,
+    request_start_time,
+    function_name,
+    provider_type,
+    tags,
+    *args,
+    **kwargs,
+):
+    response = await coroutine_obj
+    request_end_time = datetime.datetime.now().timestamp()
+    return await promptlayer_api_handler_async(
+        function_name,
+        provider_type,
+        args,
+        kwargs,
+        tags,
+        response,
+        request_start_time,
+        request_end_time,
+        get_api_key(),
+        return_pl_id=return_pl_id,
+    )
```

### Comparing `promptlayer-0.1.91/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.92/promptlayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.91
+Version: 0.1.92
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.91 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.92 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.91/promptlayer.egg-info/SOURCES.txt` & `promptlayer-0.1.92/promptlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.91/setup.py` & `promptlayer-0.1.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.91",
+    version="0.1.92",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

