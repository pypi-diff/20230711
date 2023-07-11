# Comparing `tmp/actionai-0.0.5.tar.gz` & `tmp/actionai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionai-0.0.5.tar", max compression
+gzip compressed data, was "actionai-0.0.6.tar", max compression
```

## Comparing `actionai-0.0.5.tar` & `actionai-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.5/LICENSE
--rw-r--r--   0        0        0     2152 2023-07-09 15:29:10.860733 actionai-0.0.5/README.md
--rw-r--r--   0        0        0      594 2023-07-09 16:47:48.056335 actionai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3739 2023-07-09 16:47:48.056545 actionai-0.0.5/src/actionai/__init__.py
--rw-r--r--   0        0        0       45 2023-07-09 14:31:10.412650 actionai-0.0.5/src/actionai/exceptions.py
--rw-r--r--   0        0        0     1269 2023-07-09 14:31:10.412909 actionai-0.0.5/src/actionai/json_schema.py
--rw-r--r--   0        0        0     1116 2023-07-09 15:29:10.861426 actionai-0.0.5/src/actionai/types.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 actionai-0.0.5/setup.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 actionai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2155 2023-07-11 06:16:53.623347 actionai-0.0.6/README.md
+-rw-r--r--   0        0        0      593 2023-07-11 06:16:53.623762 actionai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3766 2023-07-11 06:08:01.112385 actionai-0.0.6/src/actionai/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-09 14:31:10.412650 actionai-0.0.6/src/actionai/exceptions.py
+-rw-r--r--   0        0        0     1281 2023-07-11 06:08:01.112568 actionai-0.0.6/src/actionai/json_schema.py
+-rw-r--r--   0        0        0     1144 2023-07-11 06:08:01.112757 actionai-0.0.6/src/actionai/types.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 actionai-0.0.6/setup.py
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 actionai-0.0.6/PKG-INFO
```

### Comparing `actionai-0.0.5/LICENSE` & `actionai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `actionai-0.0.5/README.md` & `actionai-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 ```shell
 pip install actionai
 ```
 
 ## Usage
 
+> **Note**
+> A function must be fully typed and must have a docstring(one liner explanation of the function would be enough)
+
 ```python
 # define a new function
 def get_current_weather(location: str, unit: str = "fahrenheit"):
     """Function to get current weather for the given location"""
     weather_info = {
         "location": location,
         "temperature": "72",
@@ -52,17 +55,14 @@
     return todos[user]
 
 action = actionai.ActionAI(context={"user": "jason"})
 ```
 
 The context keys are skipped when creating json schema. The values are directly passed at the time of function calling.
 
-> **Warning**
-> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)
-
 ### Choosing a model
 
 By default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.
 
 ```python
 import actionai
```

### Comparing `actionai-0.0.5/pyproject.toml` & `actionai-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "actionai"
-version = "0.0.5"
+version = "0.0.6"
 description = "A small library to call local functions using openai function calling"
 authors = ["Amal Shaji <amalshajid@gmail.com>"]
 readme = "README.md"
 packages = [{include = "actionai", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 pydantic = "^2.0.2"
 openai = "^0.27.8"
 
 
 [tool.poetry.group.cq.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
```

### Comparing `actionai-0.0.5/src/actionai/__init__.py` & `actionai-0.0.6/src/actionai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from dataclasses import dataclass
-from typing import Any, Callable, cast
+from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 import openai
 
 from actionai.exceptions import ActionAIException
 from actionai.json_schema import create_json_schema_for_function_input
 from actionai.types import (
     OPENAI_MODELS,
@@ -29,40 +29,40 @@
             "parameters": self.input_schema,
         }
 
 
 class ActionAI:
     def __init__(
         self,
-        openai_api_key: str | None = None,
-        context: dict[str, Any] | None = None,
+        openai_api_key: Optional[str] = None,
+        context: Optional[Dict[str, Any]] = None,
         model: OPENAI_MODELS = "gpt-3.5-turbo-0613",
     ) -> None:
         """
         Args:
-            openai_api_key (str | None, optional): If not set, defaults \
+            openai_api_key (Optional[str]): If not set, defaults \
                 to `OPENAI_API_KEY` environment variable.
 
-            context (dict[str, Any] | None, optional): These keys will be skipped \
+            context (Optional[Dict[str, Any]]): These keys will be skipped \
                 when creating json schema for the function's input. The values \
                     will be directly passed during function call.
 
             model (optional): The chat completion model to use. Defaults to \
                 "gpt-3.5-turbo-0613".
         """
         if openai_api_key is not None:
             openai.api_key = openai_api_key
 
-        self.messages: list[Message | ChatResponseMessage] = []
+        self.messages: List[Union[Message, ChatResponseMessage]] = []
         self.context = context or {}
         self.model = model
 
         # Do not update these attributes directly
-        self._functions: dict[str, ActionAIFunction] = {}
-        self._openai_functions: list[OpenAIFunction] = []
+        self._functions: Dict[str, ActionAIFunction] = {}
+        self._openai_functions: List[OpenAIFunction] = []
 
     def register(self, fn: Callable):
         if fn.__name__ in self._functions:
             raise ActionAIException("function with the same name already registered")
 
         if fn.__doc__ is None:
             raise ActionAIException("function must have a docstring")
```

### Comparing `actionai-0.0.5/src/actionai/json_schema.py` & `actionai-0.0.6/src/actionai/json_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import inspect
-from typing import Any, Callable
+from typing import Any, Callable, Dict, List
 
 from pydantic import create_model
 
 from actionai.exceptions import ActionAIException
 
 
 def create_json_schema_for_function_input(
-    fn: Callable, skip_keys: list[str]
-) -> dict[str, Any]:
+    fn: Callable, skip_keys: List[str]
+) -> Dict[str, Any]:
     """Create json schema for a function's input
 
     Args:
         fn (Callable): The function
-        skip_keys (list[str]): The arguments to skip (context keys)
+        skip_keys (List[str]): The arguments to skip (context keys)
 
     Returns:
-        dict[str, Any]: The json schema
+        Dict[str, Any]: The json schema
     """
     signature = inspect.signature(fn)
     parameters = signature.parameters
 
     model_fields = {}
 
     for param in parameters.values():
```

### Comparing `actionai-0.0.5/src/actionai/types.py` & `actionai-0.0.6/src/actionai/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Any, Literal, TypedDict
+from typing import Any, Dict, List, Literal, Optional, TypedDict
 
 
 class _MessageBase(TypedDict):
     role: str
     content: str
 
 
 class Message(_MessageBase, total=False):
-    name: str | None
+    name: Optional[str]
 
 
 class _BaseChatResponseMessage(TypedDict):
     role: str
-    content: str | None
+    content: Optional[str]
 
 
 class ChatResponseFunctionCall(TypedDict):
     name: str
     arguments: str
 
 
@@ -37,22 +37,22 @@
 
 
 class ChatResponse(TypedDict):
     id: str
     object: str
     created: int
     model: str
-    choices: list[ChatResponseChoices]
+    choices: List[ChatResponseChoices]
     usage: ChatResponseUsage
 
 
 class OpenAIFunction(TypedDict):
     name: str
     description: str
-    parameters: dict[str, Any]
+    parameters: Dict[str, Any]
 
 
 OPENAI_MODELS = Literal[
     "gpt-4",
     "gpt-4-0613",
     "gpt-4-32k",
     "gpt-4-32k-0613",
```

### Comparing `actionai-0.0.5/setup.py` & `actionai-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.8,<0.28.0', 'pydantic>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'actionai',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'A small library to call local functions using openai function calling',
-    'long_description': '# ActionAI\n\nA small library to run local functions using openai function calling\n\n## Install\n\n```shell\npip install actionai\n```\n\n## Usage\n\n```python\n# define a new function\ndef get_current_weather(location: str, unit: str = "fahrenheit"):\n    """Function to get current weather for the given location"""\n    weather_info = {\n        "location": location,\n        "temperature": "72",\n        "unit": unit,\n        "forecast": ["sunny", "windy"],\n    }\n    return weather_info\n\n\nimport actionai\n\naction = actionai.ActionAI()\naction.register(get_current_weather)\n\nresponse = action.prompt("What is the current weather in the north pole?")\n\nprint(response["choices"][0]["message"]["content"])\n# The current weather at the North Pole is 72°F. It is sunny and windy.\n```\n\nThe openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,\n\n```python\nimport actionai\n\naction = actionai.ActionAI(openai_api_key="YOUR_KEY")\n```\n\n### Adding context\n\nSometimes your function will have variables that needs to be set by the program.\n\n```python\ndef list_todos(user: str):\n    """Function to list all todos"""\n    return todos[user]\n\naction = actionai.ActionAI(context={"user": "jason"})\n```\n\nThe context keys are skipped when creating json schema. The values are directly passed at the time of function calling.\n\n> **Warning**\n> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)\n\n### Choosing a model\n\nBy default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.\n\n```python\nimport actionai\n\naction = actionai.ActionAI(model="gpt-4")\n```\n\nYou can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)\n\n## Demo\n\nRunning [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻\n\n![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)\n\nFor more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.\n',
+    'long_description': '# ActionAI\n\nA small library to run local functions using openai function calling\n\n## Install\n\n```shell\npip install actionai\n```\n\n## Usage\n\n> **Note**\n> A function must be fully typed and must have a docstring(one liner explanation of the function would be enough)\n\n```python\n# define a new function\ndef get_current_weather(location: str, unit: str = "fahrenheit"):\n    """Function to get current weather for the given location"""\n    weather_info = {\n        "location": location,\n        "temperature": "72",\n        "unit": unit,\n        "forecast": ["sunny", "windy"],\n    }\n    return weather_info\n\n\nimport actionai\n\naction = actionai.ActionAI()\naction.register(get_current_weather)\n\nresponse = action.prompt("What is the current weather in the north pole?")\n\nprint(response["choices"][0]["message"]["content"])\n# The current weather at the North Pole is 72°F. It is sunny and windy.\n```\n\nThe openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,\n\n```python\nimport actionai\n\naction = actionai.ActionAI(openai_api_key="YOUR_KEY")\n```\n\n### Adding context\n\nSometimes your function will have variables that needs to be set by the program.\n\n```python\ndef list_todos(user: str):\n    """Function to list all todos"""\n    return todos[user]\n\naction = actionai.ActionAI(context={"user": "jason"})\n```\n\nThe context keys are skipped when creating json schema. The values are directly passed at the time of function calling.\n\n### Choosing a model\n\nBy default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.\n\n```python\nimport actionai\n\naction = actionai.ActionAI(model="gpt-4")\n```\n\nYou can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)\n\n## Demo\n\nRunning [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻\n\n![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)\n\nFor more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.\n',
     'author': 'Amal Shaji',
     'author_email': 'amalshajid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `actionai-0.0.5/PKG-INFO` & `actionai-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: actionai
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small library to call local functions using openai function calling
 Author: Amal Shaji
 Author-email: amalshajid@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ActionAI
 
@@ -19,14 +21,17 @@
 
 ```shell
 pip install actionai
 ```
 
 ## Usage
 
+> **Note**
+> A function must be fully typed and must have a docstring(one liner explanation of the function would be enough)
+
 ```python
 # define a new function
 def get_current_weather(location: str, unit: str = "fahrenheit"):
     """Function to get current weather for the given location"""
     weather_info = {
         "location": location,
         "temperature": "72",
@@ -65,17 +70,14 @@
     return todos[user]
 
 action = actionai.ActionAI(context={"user": "jason"})
 ```
 
 The context keys are skipped when creating json schema. The values are directly passed at the time of function calling.
 
-> **Warning**
-> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)
-
 ### Choosing a model
 
 By default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.
 
 ```python
 import actionai
```

