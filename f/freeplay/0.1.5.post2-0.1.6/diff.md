# Comparing `tmp/freeplay-0.1.5.post2.tar.gz` & `tmp/freeplay-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.5.post2.tar", max compression
+gzip compressed data, was "freeplay-0.1.6.tar", max compression
```

## Comparing `freeplay-0.1.5.post2.tar` & `freeplay-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.5.post2/README.md
--rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.5.post2/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.5.post2/freeplay/api_support.py
--rw-r--r--   0        0        0      802 2023-07-05 20:48:51.495916 freeplay-0.1.5.post2/freeplay/completions.py
--rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.5.post2/freeplay/errors.py
--rw-r--r--   0        0        0     8414 2023-07-06 15:31:15.280860 freeplay-0.1.5.post2/freeplay/flavors.py
--rw-r--r--   0        0        0    17926 2023-07-05 20:48:51.496816 freeplay-0.1.5.post2/freeplay/freeplay.py
--rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.5.post2/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      393 2023-07-06 15:59:00.419388 freeplay-0.1.5.post2/pyproject.toml
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 freeplay-0.1.5.post2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.6/README.md
+-rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.6/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.6/freeplay/api_support.py
+-rw-r--r--   0        0        0      802 2023-07-05 20:48:51.495916 freeplay-0.1.6/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.6/freeplay/errors.py
+-rw-r--r--   0        0        0     8833 2023-07-11 19:42:05.561871 freeplay-0.1.6/freeplay/flavors.py
+-rw-r--r--   0        0        0    22477 2023-07-11 19:42:05.562783 freeplay-0.1.6/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.6/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      391 2023-07-11 19:42:28.993845 freeplay-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.6/PKG-INFO
```

### Comparing `freeplay-0.1.5.post2/freeplay/api_support.py` & `freeplay-0.1.6/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post2/freeplay/completions.py` & `freeplay-0.1.6/freeplay/completions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post2/freeplay/flavors.py` & `freeplay-0.1.6/freeplay/flavors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from abc import abstractmethod, ABC
 from copy import copy
-from typing import Optional, Generator
+from typing import Optional, Generator, Any
 
 import anthropic  # type: ignore
 import openai
 
 from .completions import CompletionChunk, PromptTemplateWithMetadata, CompletionResponse, ChatCompletionResponse, \
     ChatMessage
 from .errors import APIKeyMissingError
@@ -31,28 +31,35 @@
         pass
 
     @abstractmethod
     def call_service_stream(self, formatted_prompt: str, llm_parameters: LLMParameters) -> Generator[
         CompletionChunk, None, None]:
         pass
 
-    def _get_model_params(self, llm_parameters: LLMParameters) -> LLMParameters:
+    def get_model_params(self, llm_parameters: LLMParameters) -> LLMParameters:
         return self._model_params_with_defaults.merge_and_override(llm_parameters)
 
 
 class ChatFlavor(Flavor, ABC):
     @abstractmethod
     def continue_chat(
             self,
-            previous_messages: list[ChatMessage],
-            new_messages: Optional[list[ChatMessage]],
+            messages: list[ChatMessage],
             llm_parameters: LLMParameters
     ) -> ChatCompletionResponse:
         pass
 
+    @abstractmethod
+    def continue_chat_stream(
+            self,
+            messages: list[ChatMessage],
+            llm_parameters: LLMParameters
+    ) -> Generator[CompletionChunk, None, None]:
+        pass
+
 
 class OpenAI(Flavor, ABC):
     def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
         super().__init__()
         if openai_api_base:
             openai.api_base = openai_api_base
 
@@ -73,30 +80,30 @@
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         return prompt_template.content.format(**variables)
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         completion = openai.Completion.create(
             prompt=formatted_prompt,
-            **self._get_model_params(llm_parameters)
+            **self.get_model_params(llm_parameters)
         )  # type: ignore
         return CompletionResponse(
             content=completion.choices[0].text,
             is_complete=completion.choices[0].finish_reason == "stop"
         )
 
     def call_service_stream(
             self,
             formatted_prompt: str,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
         completion = openai.Completion.create(
             prompt=formatted_prompt,
             stream=True,
-            **self._get_model_params(llm_parameters)
+            **self.get_model_params(llm_parameters)
         )  # type: ignore
 
         for chunk in completion:
             yield CompletionChunk(
                 text=chunk.choices[0].text,
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
@@ -118,61 +125,63 @@
         formatted_messages = [
             {"content": message['content'].format(**variables), "role": message['role']} for message in
             messages_as_json]
         return json.dumps(formatted_messages)
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         messages = json.loads(formatted_prompt)
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            **self._get_model_params(llm_parameters)
-        )  # type: ignore
+        completion = self.__call_openai(messages, llm_parameters, stream=False)
         return CompletionResponse(
             content=completion.choices[0].message.content,
-            is_complete=completion.choices[0].finish_reason == "stop"
+            is_complete=completion.choices[0].finish_reason == 'stop'
         )
 
-    def continue_chat(
+    def call_service_stream(
             self,
-            previous_messages: list[ChatMessage],
-            new_messages: Optional[list[ChatMessage]],
+            formatted_prompt: str,
             llm_parameters: LLMParameters
-    ) -> ChatCompletionResponse:
-        messages = copy(previous_messages)
-        if new_messages is not None:
-            messages.extend(new_messages)
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            **self._get_model_params(llm_parameters)
-        )  # type: ignore
-        messages.append(completion.choices[0].message.to_dict())
+    ) -> Generator[CompletionChunk, None, None]:
+        messages = json.loads(formatted_prompt)
+        completion_stream = self.__call_openai(messages, llm_parameters, stream=True)
+        for chunk in completion_stream:
+            yield CompletionChunk(
+                text=chunk.choices[0].delta.get('content', ""),
+                is_complete=chunk.choices[0].finish_reason == "stop"
+            )
+
+    def continue_chat(self, messages: list[ChatMessage], llm_parameters: LLMParameters) -> ChatCompletionResponse:
+        completion = self.__call_openai(messages, llm_parameters, stream=False)
+
+        message_history = copy(messages)
+        message_history.append(completion.choices[0].message.to_dict())
         return ChatCompletionResponse(
             content=completion.choices[0].message.content,
-            message_history=messages,
+            message_history=message_history,
             is_complete=completion.choices[0].finish_reason == "stop"
         )
 
-    def call_service_stream(
+    def continue_chat_stream(
             self,
-            formatted_prompt: str,
+            messages: list[ChatMessage],
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
-        messages = json.loads(formatted_prompt)
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            stream=True,
-            **self._get_model_params(llm_parameters)
-        )  # type: ignore
-        for chunk in completion:
-            # Not all chunks have a "content" field -- if they don't, keep chunking.
+        completion_stream = self.__call_openai(messages, llm_parameters, stream=True)
+        for chunk in completion_stream:
             yield CompletionChunk(
-                text=chunk.choices[0].delta.get('content', ""),
+                text=chunk.choices[0].delta.get('content', ''),
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
 
+    def __call_openai(self, messages: list[ChatMessage], llm_parameters: LLMParameters, stream: bool) -> Any:
+        return openai.ChatCompletion.create(
+            messages=messages,
+            **self.get_model_params(llm_parameters),
+            stream=stream
+        )  # type: ignore
+
 
 class AnthropicClaudeText(Flavor):
     record_format_type = "anthropic_text"
     _model_params_with_defaults = LLMParameters({
         "model": "claude-v1",
         "max_tokens_to_sample": 100
     })
@@ -185,29 +194,29 @@
         # Anthropic expects a specific Chat format "Human: $PROMPT_TEXT\n\nAssistant:". We add the wrapping for Text.
         chat_formatted_prompt = f"{anthropic.HUMAN_PROMPT} {interpolated_prompt} {anthropic.AI_PROMPT}"
         return chat_formatted_prompt
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         anthropic_response = self.client.completion(
             prompt=formatted_prompt,
-            **self._get_model_params(llm_parameters)
+            **self.get_model_params(llm_parameters)
         )
         return CompletionResponse(
             content=anthropic_response['completion'],
             is_complete=anthropic_response['stop_reason'] == 'stop_sequence'
         )
 
     def call_service_stream(
             self,
             formatted_prompt: str,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
         anthropic_response = self.client.completion_stream(
             prompt=formatted_prompt,
-            **self._get_model_params(llm_parameters)
+            **self.get_model_params(llm_parameters)
         )
 
         # Yield incremental text completions. Claude returns the full text output in every chunk.
         # We want to predictably return a stream like we do for OpenAI.
         prev_chunk = ''
         for chunk in anthropic_response:
             if len(prev_chunk) != 0:
```

### Comparing `freeplay-0.1.5.post2/freeplay/freeplay.py` & `freeplay-0.1.6/freeplay/freeplay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import copy
 import json
 import logging
 import time
 from dataclasses import dataclass
 from typing import Optional, Generator, Any, cast, Tuple
 
 from . import api_support
@@ -53,53 +54,109 @@
         prompts = api_support.get(
             target_type=PromptTemplates,
             api_key=self.freeplay_api_key,
             url=f'{self.api_base}/projects/{project_id}/templates/all/{tag}'
         )
         return prompts
 
-    def continue_chat(
+    def prepare_and_make_chat_call(
             self,
             session_id: str,
             flavor: ChatFlavor,
             tag: str,
             target_template: PromptTemplateWithMetadata,
             variables: Variables,
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]],
             test_run_id: Optional[str] = None,
             completion_parameters: Optional[LLMParameters] = None) -> ChatCompletionResponse:
         # make call
         start = int(time.time())
         try:
-            params = self.client_params.merge_and_override(completion_parameters)
-            completion_response = flavor.continue_chat(message_history, new_messages=new_messages,
-                                                       llm_parameters=params)
+            params = target_template.get_params() \
+                .merge_and_override(self.client_params) \
+                .merge_and_override(completion_parameters)
+            prompt_messages = copy(message_history)
+            if new_messages is not None:
+                prompt_messages.extend(new_messages)
+            completion_response = flavor.continue_chat(messages=prompt_messages, llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
-        formatted_prompt = json.dumps(completion_response.message_history)
+        model = flavor.get_model_params(params).get('model')
+        formatted_prompt = json.dumps(prompt_messages)
         # record data
         self.__record_call(
             completion_response.content,
             completion_response.is_complete,
             end,
             formatted_prompt,
             session_id,
             start,
             target_template,
             variables,
             flavor.record_format_type,
             tag,
-            test_run_id
+            test_run_id,
+            model
         )
 
         return completion_response
 
+    def prepare_and_make_chat_call_stream(
+            self,
+            session_id: str,
+            flavor: ChatFlavor,
+            tag: str,
+            target_template: PromptTemplateWithMetadata,
+            variables: Variables,
+            message_history: list[ChatMessage],
+            new_messages: Optional[list[ChatMessage]],
+            test_run_id: Optional[str] = None,
+            completion_parameters: Optional[LLMParameters] = None
+    ) -> Generator[CompletionChunk, None, None]:
+        # make call
+        start = int(time.time())
+        try:
+            prompt_messages = copy(message_history)
+            if new_messages is not None:
+                prompt_messages.extend(new_messages)
+            params = target_template.get_params() \
+                .merge_and_override(self.client_params) \
+                .merge_and_override(completion_parameters)
+            completion_response = flavor.continue_chat_stream(prompt_messages, llm_parameters=params)
+        except Exception as e:
+            raise FreeplayError("Error calling service") from e
+        end = int(time.time())
+
+        str_content = ''
+        last_is_complete = False
+        for chunk in completion_response:
+            str_content += chunk.text or ''
+            last_is_complete = chunk.is_complete
+            yield chunk
+
+        model = flavor.get_model_params(params).get('model')
+        formatted_prompt = json.dumps(prompt_messages)
+        self.__record_call(
+            str_content,
+            last_is_complete,
+            end,
+            formatted_prompt,
+            session_id,
+            start,
+            target_template,
+            variables,
+            flavor.record_format_type,
+            tag,
+            test_run_id,
+            model
+        )
+
     def prepare_and_make_call(
             self,
             session_id: str,
             prompts: PromptTemplates,
             template_name: str,
             variables: dict[str, str],
             flavor: Flavor,
@@ -119,27 +176,30 @@
 
             completion_response = flavor.call_service(
                 formatted_prompt=formatted_prompt, llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
+        model = flavor.get_model_params(params).get('model')
+
         # record data
         self.__record_call(
             completion_response.content,
             completion_response.is_complete,
             end,
             formatted_prompt,
             session_id,
             start,
             target_template,
             variables,
             flavor.record_format_type,
             tag,
-            test_run_id
+            test_run_id,
+            model
         )
 
         return completion_response
 
     def prepare_and_make_call_stream(
             self,
             session_id: str,
@@ -164,53 +224,58 @@
         last_is_complete = False
         for chunk in completion_response:
             text_chunks.append(chunk.text)
             last_is_complete = chunk.is_complete
             yield chunk
         end = int(time.time())
 
+        model = flavor.get_model_params(params).get('model')
+
         self.__record_call(''.join(text_chunks),
                            last_is_complete,
                            end,
                            formatted_prompt,
                            session_id,
                            start,
                            target_template,
                            variables,
                            flavor.record_format_type,
                            tag,
-                           test_run_id)
+                           test_run_id,
+                           model)
 
     def __record_call(
             self,
             completion_content: str,
             completion_is_complete: bool,
             end: int,
             formatted_prompt: str,
             session_id: str,
             start: int,
             target_template: PromptTemplateWithMetadata,
             variables: dict[str, str],
             record_format_type: str,
             tag: str,
-            test_run_id: Optional[str]
+            test_run_id: Optional[str],
+            model: Optional[str],
     ) -> None:
 
         record_payload = {
             "session_id": session_id,
             "project_version_id": target_template.project_version_id,
             "prompt_template_id": target_template.prompt_template_id,
             "start_time": start,
             "end_time": end,
             "tag": tag,
             "inputs": variables,
             "prompt_content": formatted_prompt,
             "return_content": completion_content,
             "format_type": record_format_type,
-            "is_complete": completion_is_complete
+            "is_complete": completion_is_complete,
+            "model": model
         }
 
         if test_run_id is not None:
             record_payload['test_run_id'] = test_run_id
 
         try:
             recorded_response = api_support.post_raw(
@@ -291,37 +356,74 @@
             tag: str = default_tag,
             test_run_id: Optional[str] = None
     ) -> None:
         super().__init__(call_support, session_id, prompts, flavor, tag, test_run_id)
         self.flavor = flavor  # Ensures a ChatFlavor is set for this session.
         # A Chat Session tracks the template_name and variables for a set of chat completions.
         # Assumes these will be the same for subsequent chat messages.
-        self.template_name = template_name
         self.variables = variables
+        self.target_template = self.call_support.find_template_by_name(self.prompts, template_name)
+        self.__initial_messages = json.loads(self.session_flavor.format(self.target_template, self.variables))
 
     def start_chat(self, **kwargs: Any) -> ChatCompletionResponse:
-        target_template = self.call_support.find_template_by_name(self.prompts, self.template_name)
-        formatted_prompt = self.session_flavor.format(target_template, self.variables)
-        messages = json.loads(formatted_prompt)
-        return self.continue_chat(message_history=messages, new_messages=None, **kwargs)
+        return self.call_support.prepare_and_make_chat_call(
+            self.session_id,
+            flavor=self.flavor,
+            tag=self.tag,
+            test_run_id=self.test_run_id,
+            target_template=self.target_template,
+            variables=self.variables,
+            message_history=self.__initial_messages,
+            new_messages=None,
+            completion_parameters=LLMParameters(kwargs)
+        )
+
+    def start_chat_stream(self, **kwargs: Any) -> Tuple[Generator[CompletionChunk, None, None], list[ChatMessage]]:
+        return self.call_support.prepare_and_make_chat_call_stream(
+            self.session_id,
+            flavor=self.flavor,
+            tag=self.tag,
+            test_run_id=self.test_run_id,
+            target_template=self.target_template,
+            variables=self.variables,
+            message_history=self.__initial_messages,
+            new_messages=None,
+            completion_parameters=LLMParameters(kwargs)
+        ), self.__initial_messages
 
     def continue_chat(
             self,
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]] = None,
             **kwargs: Any
     ) -> ChatCompletionResponse:
-        target_template = self.call_support.find_template_by_name(self.prompts, self.template_name)
+        return self.call_support.prepare_and_make_chat_call(
+            self.session_id,
+            flavor=self.flavor,
+            tag=self.tag,
+            test_run_id=self.test_run_id,
+            target_template=self.target_template,
+            variables=self.variables,
+            message_history=message_history,
+            new_messages=new_messages,
+            completion_parameters=LLMParameters(kwargs)
+        )
 
-        return self.call_support.continue_chat(
+    def continue_chat_stream(
+            self,
+            message_history: list[ChatMessage],
+            new_messages: Optional[list[ChatMessage]] = None,
+            **kwargs: Any
+    ) -> Generator[CompletionChunk, None, None]:
+        return self.call_support.prepare_and_make_chat_call_stream(
             self.session_id,
             flavor=self.flavor,
             tag=self.tag,
             test_run_id=self.test_run_id,
-            target_template=target_template,
+            target_template=self.target_template,
             variables=self.variables,
             message_history=message_history,
             new_messages=new_messages,
             completion_parameters=LLMParameters(kwargs)
         )
 
 
@@ -430,22 +532,37 @@
             self,
             project_id: str,
             template_name: str,
             variables: Variables,
             tag: str = default_tag,
             **kwargs: Any
     ) -> Tuple[ChatSession, ChatCompletionResponse]:
+        session = self.__create_chat_session(project_id, tag, template_name, variables)
+        completion_response = session.start_chat(**kwargs)
+        return session, completion_response
+
+    def start_chat_stream(
+            self,
+            project_id: str,
+            template_name: str,
+            variables: Variables,
+            tag: str = default_tag,
+            **kwargs: Any
+    ) -> Tuple[ChatSession, list[ChatMessage], Generator[CompletionChunk, None, None]]:
+        """Returns a chat session, the base prompt template messages, and a streamed response from the LLM."""
+        session = self.__create_chat_session(project_id, tag, template_name, variables)
+        completion_response, initial_messages = session.start_chat_stream(**kwargs)
+        return session, initial_messages, completion_response
+
+    def __create_chat_session(self, project_id: str, tag: str, template_name: str, variables: Variables) -> ChatSession:
         if not isinstance(self.client_flavor, ChatFlavor):
             raise FreeplayError('A Chat flavor is required to start a chat session.')
-
         project_session = self.call_support.create_session(project_id, tag)
         prompts = self.call_support.get_prompts(project_id, tag)
-        session = ChatSession(
+        return ChatSession(
             self.call_support,
             project_session['session_id'],
             prompts,
             self.client_flavor,
             template_name,
             variables,
             tag)
-        completion_response = session.start_chat(**kwargs)
-        return session, completion_response
```

### Comparing `freeplay-0.1.5.post2/freeplay/llm_parameters.py` & `freeplay-0.1.6/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post2/PKG-INFO` & `freeplay-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.5.post2
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

