# Comparing `tmp/smol_dev-0.0.2.tar.gz` & `tmp/smol_dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_dev-0.0.2.tar", max compression
+gzip compressed data, was "smol_dev-0.0.3.tar", max compression
```

## Comparing `smol_dev-0.0.2.tar` & `smol_dev-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      199 2023-07-02 21:34:41.520460 smol_dev-0.0.2/README.md
--rw-r--r--   0        0        0      519 2023-07-02 21:36:11.244133 smol_dev-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 19:44:11.337011 smol_dev-0.0.2/smol_dev/__init__.py
--rw-r--r--   0        0        0       62 2023-07-02 19:44:11.337510 smol_dev-0.0.2/smol_dev/__main__.py
--rw-r--r--   0        0        0     1498 2023-07-02 21:13:52.150917 smol_dev-0.0.2/smol_dev/main.py
--rw-r--r--   0        0        0     6825 2023-07-02 21:28:13.750660 smol_dev-0.0.2/smol_dev/prompts.py
--rw-r--r--   0        0        0      587 2023-07-02 21:13:58.509196 smol_dev-0.0.2/smol_dev/utils.py
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 smol_dev-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-30 02:52:05.717323 smol_dev-0.0.3/LICENSE
+-rw-r--r--   0        0        0      516 2023-07-11 03:51:18.194194 smol_dev-0.0.3/README.md
+-rw-r--r--   0        0        0      591 2023-07-11 04:01:17.663817 smol_dev-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-11 02:15:42.698639 smol_dev-0.0.3/smol_dev/__init__.py
+-rw-r--r--   0        0        0     3404 2023-07-11 03:35:00.211010 smol_dev-0.0.3/smol_dev/main.py
+-rw-r--r--   0        0        0     6760 2023-07-11 03:34:18.450925 smol_dev-0.0.3/smol_dev/prompts.py
+-rw-r--r--   0        0        0      471 2023-07-11 02:15:42.700303 smol_dev-0.0.3/smol_dev/utils.py
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 smol_dev-0.0.3/PKG-INFO
```

### Comparing `smol_dev-0.0.2/smol_dev/prompts.py` & `smol_dev-0.0.3/smol_dev/prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,180 @@
-import openai
-from typing import List
-from openai_function_call import openai_function
+import asyncio
 import re
+import time
+from typing import List, Optional, Callable, Any
 
-# openaimodel = "gpt-3.5-turbo-0613"
-openaimodel = "gpt-4-0613"
+import openai
+from openai_function_call import openai_function
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 
-smol_dev_system_prompt = """
-You are an AI developer who is trying to write a program that will generate code for the user based on their intent.
-"""
 
+SMOL_DEV_SYSTEM_PROMPT = """
+You are a top tier AI developer who is trying to write a program that will generate code for the user based on their intent.
+Do not leave any todos, fully implement every feature requested.
 
+When writing code, add comments to explain what you intend to do and why it aligns with the program plan and specific instructions from the original prompt.
+"""
 
 
 @openai_function
-def filePaths(filesToEdit: List[str]) -> List[str]:
-    """Takes a list of filepaths relative to the current directory and returns a list of filepaths that need to be edited."""
-    print('filesToEdit', filesToEdit)
-    return filesToEdit
-
-
-def specify_filePaths(prompt: str, sharedDependencyManifest: str):
-  completion = openai.ChatCompletion.create(
-          model=openaimodel,
-          temperature=0.7,
-          functions=[filePaths.openai_schema],
-          function_call={ "name": "filePaths" },
-          messages=[
-              {
-                  "role": "system",
-                  "content": f"""{smol_dev_system_prompt}
+def file_paths(files_to_edit: List[str]) -> List[str]:
+    """
+    Construct a list of strings.
+    """
+    # print("filesToEdit", files_to_edit)
+    return files_to_edit
+
+
+def specify_file_paths(prompt: str, plan: str, model: str = 'gpt-3.5-turbo-0613'):
+    completion = openai.ChatCompletion.create(
+        model=model,
+        temperature=0.7,
+        functions=[file_paths.openai_schema],
+        function_call={"name": "file_paths"},
+        messages=[
+            {
+                "role": "system",
+                "content": f"""{SMOL_DEV_SYSTEM_PROMPT}
           
       When given their intent, create a complete, exhaustive list of filepaths that the user would write to make the program.
       
       only list the filepaths you would write, and return them as a python list of strings. 
       do not add any other explanation, only return a python list of strings.
                   """,
-              },
-              {
-                  "role": "user",
-                  "content": f""" I want a: {prompt} """,
-              },
-              {
-                  "role": "user",
-                  "content": f""" The shared dependencies we have agreed on are: {sharedDependencyManifest} """,
-              },
-          ],
-      )
-  result = filePaths.from_response(completion)
-  return result
-  
-
-def passthrough(prompt: str):
-  print('passthrough', prompt)
-  return prompt
-
-# def plan(prompt: str, filePaths: List[str]):
-def plan(prompt: str):
-  completion = openai.ChatCompletion.create(
-          model=openaimodel,
-          temperature=0.7,
-          messages=[
-              {
-                  "role": "system",
-                  "content": f"""{smol_dev_system_prompt}
+            },
+            {
+                "role": "user",
+                "content": f""" I want a: {prompt} """,
+            },
+            {
+                "role": "user",
+                "content": f""" The plan we have agreed on is: {plan} """,
+            },
+        ],
+    )
+    result = file_paths.from_response(completion)
+    return result
+
+
+def plan(prompt: str, stream_handler: Optional[Callable[[bytes], None]] = None, model: str='gpt-3.5-turbo-0613'):
+    completion = openai.ChatCompletion.create(
+        model=model,
+        temperature=0.7,
+        stream=True,
+        messages=[
+            {
+                "role": "system",
+                "content": f"""{SMOL_DEV_SYSTEM_PROMPT}
       
   In response to the user's prompt, 
   Please name and briefly describe the structure of the app we will generate, including, for each file we are generating, what variables they export, data schemas, id names of every DOM elements that javascript functions will use, message names, and function names.
                   """,
-  # Exclusively focus on the names of the shared dependencies, and do not add any other explanation.
-              },
-              # {
-              #     "role": "user",
-              #     "content": f""" the files we have decided to generate are: {filePaths} """,
-              # },
-              {
-                  "role": "user",
-                  "content": f""" the app prompt is: {prompt} """,
-              },
-          ],
-      )
-  # result = sharedDeps.from_response(completion)
-  # return result
-  return completion.choices[0].message.content
-
-
-#####
-# TODO: explore pydantic models for export to morph/rift
-#####
-# from pydantic import BaseModel, Field # probably doesn't compile
-
-# class CodeFile(BaseModel):
-#     file_name: str = Field("Name of the file")
-#     file_contents: str = Field("Contents of the file. Must compile correctly")
-    
-# class SmolDeveloperManifest(BaseModel):
-#     md_contents = Field("flat md file which specifies the directory tree of the app we are generating")
-
-# # we want to compute this result incrementally through a chain of thought, i.e.
-# # first, synthesize the manifest
-# # then synthesize partial codefiles with filenames and filepaths
-# # then for all codefiles synthesize content
-# class SmolDeveloperResult(BaseModel):
-#     manifest: SmolDeveloperManifest
-#     code_files: List[CodeFile]
-
-@openai_function
-def validCodeFile(codeFile: str) -> str:
-    """Receives a string of valid code and, after checking for code blocks, returns a string of code that is valid."""
-    # pattern = r"```[\w\s]*\n([\s\S]*?)```" # original regex for code blocks anywhere in the string
-    print('----codeFile', codeFile)
-    pattern = r"^\s*```[ws]*\n([sS]*?)```" # codeblocks at start of the string, less eager
-    code_blocks = re.findall(pattern, codeFile, re.MULTILINE)
-    return code_blocks[0] if code_blocks else codeFile
-
-def generate_code(prompt: str, sharedDependencyManifest: str, currentFile: str):
-  completion = openai.ChatCompletion.create(
-          model=openaimodel,
-          temperature=0.7,
-          functions=[validCodeFile.openai_schema],
-          function_call={ "name": "validCodeFile" },
-          messages=[
-              {
-                  "role": "system",
-                  "content": f"""{smol_dev_system_prompt}
+            },
+            {
+                "role": "user",
+                "content": f""" the app prompt is: {prompt} """,
+            },
+        ],
+    )
+
+    collected_messages = []
+    for chunk in completion:
+        chunk_message = chunk["choices"][0]["delta"]  # extract the message
+        collected_messages.append(chunk_message)  # save the message
+        if stream_handler:
+            try:
+                stream_handler(chunk_message["content"].encode("utf-8"))
+            except Exception as err:
+                print("stream_handler error:", err)
+                print(chunk_message)
+    full_reply_content = "".join([m.get("content", "") for m in collected_messages])
+    return full_reply_content
+
+
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6))
+async def generate_code(prompt: str, plan: str, current_file: str, stream_handler: Optional[Callable[Any, Any]] = None,
+                        model: str = 'gpt-3.5-turbo-0613') -> str:
+    first = True
+    chunk_count = 0
+    start_time = time.time()
+    completion = openai.ChatCompletion.acreate(
+        model=model,
+        temperature=0.7,
+        messages=[
+            {
+                "role": "system",
+                "content": f"""{SMOL_DEV_SYSTEM_PROMPT}
       
   In response to the user's prompt, 
   Please name and briefly describe the structure of the app we will generate, including, for each file we are generating, what variables they export, data schemas, id names of every DOM elements that javascript functions will use, message names, and function names.
 
   We have broken up the program into per-file generation. 
-  Now your job is to generate only the code for the file: {currentFile} 
+  Now your job is to generate only the code for the file: {current_file} 
   
   only write valid code for the given filepath and file type, and return only the code.
   do not add any other explanation, only return valid code for that file type.
                   """,
-              },
-              {
-                  "role": "user",
-                  "content": f""" the plan we have agreed on is: {sharedDependencyManifest} """,
-              },
-              {
-                  "role": "user",
-                  "content": f""" the app prompt is: {prompt} """,
-              },
-              {
-                  "role": "user",
-                  "content": f"""
+            },
+            {
+                "role": "user",
+                "content": f""" the plan we have agreed on is: {plan} """,
+            },
+            {
+                "role": "user",
+                "content": f""" the app prompt is: {prompt} """,
+            },
+            {
+                "role": "user",
+                "content": f"""
     Make sure to have consistent filenames if you reference other files we are also generating.
     
     Remember that you must obey 3 things: 
-       - you are generating code for the file {currentFile}
-       - do not stray from the names of the files and the shared dependencies we have decided on
+       - you are generating code for the file {current_file}
+       - do not stray from the names of the files and the plan we have decided on
        - MOST IMPORTANT OF ALL - every line of code you generate must be valid code. Do not include code fences in your response, for example
     
-    Bad response:
+    Bad response (because it contains the code fence):
     ```javascript 
     console.log("hello world")
     ```
     
-    Good response:
+    Good response (because it only contains the code):
     console.log("hello world")
     
     Begin generating the code now.
 
     """,
-              },
-          ],
-      )
-  codeFile = validCodeFile.from_response(completion)
-  return codeFile
-#   print('xxxxxcodeFile', codeFile)
-#   pattern = r"^\s*```[ws]*\n([sS]*?)```" # codeblocks at start of the string, less eager
-#   code_blocks = re.findall(pattern, codeFile, re.MULTILINE)
-#   return code_blocks[0] if code_blocks[0] is not None else codeFile
-# #   return result
-# #   return completion.choices[0].message.content
+            },
+        ],
+        stream=True,
+    )
+
+    collected_messages = []
+    async for chunk in await completion:
+        chunk_message = chunk["choices"][0]["delta"]  # extract the message
+        if stream_handler:
+            try:
+                stream_handler(chunk_message['content'].encode('utf-8'))
+            except Exception as err:
+                pass
+        collected_messages.append(chunk_message)  # save the message
+        if chunk_count < 5:
+            chunk_time = time.time() - start_time  # calculate the time delay of the chunk
+            chunk_count += 1
+
+    code_file = "".join([m.get("content", "") for m in collected_messages])
+
+    pattern = r"```[\w\s]*\n([\s\S]*?)```"  # codeblocks at start of the string, less eager
+    code_blocks = re.findall(pattern, code_file, re.MULTILINE)
+    return code_blocks[0] if code_blocks else code_file
+
+
+def generate_code_sync(prompt: str, plan: str, current_file: str,
+                       stream_handler: Optional[Callable[Any, Any]] = None,
+                       model: str = 'gpt-3.5-turbo-0613') -> str:
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(generate_code(prompt, plan, current_file, stream_handler, model))
```

