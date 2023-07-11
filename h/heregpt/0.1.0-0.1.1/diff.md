# Comparing `tmp/heregpt-0.1.0.tar.gz` & `tmp/heregpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heregpt-0.1.0.tar", max compression
+gzip compressed data, was "heregpt-0.1.1.tar", max compression
```

## Comparing `heregpt-0.1.0.tar` & `heregpt-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-06 19:18:12.014744 heregpt-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-06 19:18:30.712845 heregpt-0.1.0/heregpt/__init__.py
--rw-r--r--   0        0        0      885 2023-07-10 20:19:31.626465 heregpt-0.1.0/heregpt/main.py
--rw-r--r--   0        0        0      547 2023-07-10 20:18:18.359202 heregpt-0.1.0/heregpt/models.py
--rw-r--r--   0        0        0     1621 2023-07-10 20:18:46.582158 heregpt-0.1.0/heregpt/utils.py
--rw-r--r--   0        0        0      617 2023-07-06 20:34:51.337248 heregpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 heregpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-06 19:18:12.014744 heregpt-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 19:18:30.712845 heregpt-0.1.1/heregpt/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-11 20:29:30.277856 heregpt-0.1.1/heregpt/main.py
+-rw-r--r--   0        0        0      547 2023-07-10 20:18:18.359202 heregpt-0.1.1/heregpt/models.py
+-rw-r--r--   0        0        0     1621 2023-07-10 20:18:46.582158 heregpt-0.1.1/heregpt/utils.py
+-rw-r--r--   0        0        0      617 2023-07-11 20:28:21.503959 heregpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 heregpt-0.1.1/PKG-INFO
```

### Comparing `heregpt-0.1.0/heregpt/main.py` & `heregpt-0.1.1/heregpt/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,40 @@
+import os
+
 import typer
 from rich import print
 from rich.console import Console
+from typing_extensions import Annotated
 
 from heregpt import utils
 from heregpt.models import TaskBase
 
 app = typer.Typer()
 
 console = Console()
 
 
 @app.command()
-def main(tool: str, task: str):
-    if not utils.set_openai_api_key():
-        console.print(
-            "The environment variable OPENAI_API_KEY is not defined. More details here:"
-        )
-        console.print(utils.set_openai_api_key.__doc__)
-        raise typer.Exit(42)
+def main(
+    tool: Annotated[str, typer.Argument(help="Name of the tool you want to use")],
+    task: Annotated[str, typer.Argument(help="Describe the task you want to execute")],
+    openai_key: Annotated[
+        str, typer.Option(help="Manually provided API key for OpenAI")
+    ] = None,
+):
+    if openai_key is not None:
+        os.environ["OPENAI_API_KEY"] = openai_key
+    if openai_key is None:
+        if not utils.set_openai_api_key():
+            console.print(
+                "The environment variable OPENAI_API_KEY is not defined. More details"
+                " here:"
+            )
+            console.print(utils.set_openai_api_key.__doc__)
+            raise typer.Exit(42)
     task = TaskBase(tool=tool, task=task)
     task.build_prompt()
     console.print("About to send the following prompt🚀", style="#5f5fff")
     print(task.prompt)
     console.print("End of prompt", style="#5f5fff")
     abort = typer.confirm("Abort?", default=True)
     if abort:
```

### Comparing `heregpt-0.1.0/heregpt/models.py` & `heregpt-0.1.1/heregpt/models.py`

 * *Files identical despite different names*

### Comparing `heregpt-0.1.0/heregpt/utils.py` & `heregpt-0.1.1/heregpt/utils.py`

 * *Files identical despite different names*

### Comparing `heregpt-0.1.0/pyproject.toml` & `heregpt-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heregpt"
-version = "0.1.0"
+version = "0.1.1"
 description = "Have ChatGPT right_here_ within your shell"
 authors = ["Dror Atariah <drorata@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `heregpt-0.1.0/PKG-INFO` & `heregpt-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heregpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Have ChatGPT right_here_ within your shell
 License: MIT
 Author: Dror Atariah
 Author-email: drorata@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

