# Comparing `tmp/rubberduck-ai-0.5.8.tar.gz` & `tmp/rubberduck-ai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubberduck-ai-0.5.8.tar", last modified: Sat Mar 25 07:54:42 2023, max compression
+gzip compressed data, was "rubberduck-ai-0.6.0.tar", last modified: Tue Jul 11 21:53:54 2023, max compression
```

## Comparing `rubberduck-ai-0.5.8.tar` & `rubberduck-ai-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-25 07:54:42.264000 rubberduck-ai-0.5.8/
--rw-r--r--   0 david      (501) staff       (20)    35148 2023-03-22 04:14:30.000000 rubberduck-ai-0.5.8/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     1376 2023-03-25 07:54:42.263908 rubberduck-ai-0.5.8/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1099 2023-03-22 04:13:56.000000 rubberduck-ai-0.5.8/README.md
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-25 07:54:42.262562 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     1376 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      608 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       56 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/entry_points.txt
--rw-r--r--   0 david      (501) staff       (20)      147 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       16 2023-03-25 07:54:42.000000 rubberduck-ai-0.5.8/rubberduck_ai.egg-info/top_level.txt
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-25 07:54:42.263267 rubberduck-ai-0.5.8/rubberduck_chat/
--rw-r--r--   0 david      (501) staff       (20)       22 2023-03-25 07:54:24.000000 rubberduck-ai-0.5.8/rubberduck_chat/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-25 07:54:42.263764 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/
--rw-r--r--   0 david      (501) staff       (20)       90 2023-03-18 03:49:08.000000 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     7648 2023-03-25 07:53:26.000000 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/chat.py
--rw-r--r--   0 david      (501) staff       (20)     3282 2023-03-19 03:08:33.000000 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/credentials.py
--rw-r--r--   0 david      (501) staff       (20)     8616 2023-03-19 23:28:03.000000 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/session_store.py
--rw-r--r--   0 david      (501) staff       (20)     2709 2023-03-19 23:27:28.000000 rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/setup_gpt.py
--rw-r--r--   0 david      (501) staff       (20)     6719 2023-03-19 23:30:30.000000 rubberduck-ai-0.5.8/rubberduck_chat/configs.py
--rw-r--r--   0 david      (501) staff       (20)     5252 2023-03-19 23:31:37.000000 rubberduck-ai-0.5.8/rubberduck_chat/input_handler.py
--rw-r--r--   0 david      (501) staff       (20)     1375 2023-03-19 05:48:07.000000 rubberduck-ai-0.5.8/rubberduck_chat/rubberduck.py
--rw-r--r--   0 david      (501) staff       (20)      169 2023-03-19 05:41:55.000000 rubberduck-ai-0.5.8/rubberduck_chat/store.py
--rw-r--r--   0 david      (501) staff       (20)      181 2023-03-18 03:49:08.000000 rubberduck-ai-0.5.8/rubberduck_chat/utils.py
--rw-r--r--   0 david      (501) staff       (20)       38 2023-03-25 07:54:42.264033 rubberduck-ai-0.5.8/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      903 2023-03-22 04:14:41.000000 rubberduck-ai-0.5.8/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-11 21:53:54.935021 rubberduck-ai-0.6.0/
+-rw-r--r--   0 david      (501) staff       (20)    35148 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)     1376 2023-07-11 21:53:54.934878 rubberduck-ai-0.6.0/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1099 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/README.md
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-11 21:53:54.933021 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     1376 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      608 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)       56 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/entry_points.txt
+-rw-r--r--   0 david      (501) staff       (20)      147 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       16 2023-07-11 21:53:54.000000 rubberduck-ai-0.6.0/rubberduck_ai.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-11 21:53:54.934144 rubberduck-ai-0.6.0/rubberduck_chat/
+-rw-r--r--   0 david      (501) staff       (20)       22 2023-07-11 21:48:28.000000 rubberduck-ai-0.6.0/rubberduck_chat/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-11 21:53:54.934689 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/
+-rw-r--r--   0 david      (501) staff       (20)       90 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     7723 2023-07-11 21:40:20.000000 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/chat.py
+-rw-r--r--   0 david      (501) staff       (20)     3282 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/credentials.py
+-rw-r--r--   0 david      (501) staff       (20)     8616 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/session_store.py
+-rw-r--r--   0 david      (501) staff       (20)     2786 2023-07-11 21:35:49.000000 rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/setup_gpt.py
+-rw-r--r--   0 david      (501) staff       (20)     6887 2023-07-11 21:42:46.000000 rubberduck-ai-0.6.0/rubberduck_chat/configs.py
+-rw-r--r--   0 david      (501) staff       (20)     5252 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/input_handler.py
+-rw-r--r--   0 david      (501) staff       (20)     1375 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/rubberduck.py
+-rw-r--r--   0 david      (501) staff       (20)      169 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/store.py
+-rw-r--r--   0 david      (501) staff       (20)      181 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/rubberduck_chat/utils.py
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-11 21:53:54.935058 rubberduck-ai-0.6.0/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      903 2023-05-06 17:45:26.000000 rubberduck-ai-0.6.0/setup.py
```

### Comparing `rubberduck-ai-0.5.8/LICENSE` & `rubberduck-ai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/PKG-INFO` & `rubberduck-ai-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubberduck-ai
-Version: 0.5.8
+Version: 0.6.0
 Summary: A CLI tool for ChatGPT.
 Home-page: https://github.com/hansololz/rubberduck-ai
 License: GPL
 Keywords: rda,openai,ChatGPT,chat
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rubberduck-ai-0.5.8/README.md` & `rubberduck-ai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/rubberduck_ai.egg-info/PKG-INFO` & `rubberduck-ai-0.6.0/rubberduck_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubberduck-ai
-Version: 0.5.8
+Version: 0.6.0
 Summary: A CLI tool for ChatGPT.
 Home-page: https://github.com/hansololz/rubberduck-ai
 License: GPL
 Keywords: rda,openai,ChatGPT,chat
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rubberduck-ai-0.5.8/rubberduck_ai.egg-info/SOURCES.txt` & `rubberduck-ai-0.6.0/rubberduck_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/chat.py` & `rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from rubberduck_chat.chat_gpt.session_store import *
 from rubberduck_chat.utils import get_datetime
 from dataclasses import dataclass
 
 
 @dataclass
 class GptChatSessionConfigs:
+  chat_gpt_model: str
   max_messages_per_request: int
   snippet_header_background_color: str
   snippet_theme: str
 
 
 class GptChatSession:
   snippet_end_pattern = r'\s*```'
@@ -72,15 +73,15 @@
         create_time = ''
 
       print(f'>>>{create_time}{turn.user_prompt}')
       assistant_response = turn.get_assistant_response()
       if assistant_response:
         self.print_assistant_response(assistant_response)
 
-  def process_prompt(self, prompt: str):
+  def process_prompt(self, prompt: str, configs: GptChatSessionConfigs):
     current_turn = GptChatTurn.from_user_prompt(prompt)
     self.store_chat_turn(current_turn)
     self.turns.append(current_turn)
     messages: List[dict] = [self.system_message.get_chat_gpt_request_message()]
 
     for turn in self.turns[-(self.configs.max_messages_per_request + 1):]:
       messages.append(turn.get_user_prompt_message())
@@ -89,15 +90,15 @@
         messages.append(assistant_response_message)
 
     response = None
     error_message = None
 
     with Halo(text='Fetching', spinner='dots'):
       try:
-        response = openai.ChatCompletion.create(model='gpt-3.5-turbo', messages=messages)
+        response = openai.ChatCompletion.create(model=configs.chat_gpt_model, messages=messages)
       except Exception as error:
         error_message = str(error)
 
     if error_message:
       print(error_message)
       return
 
@@ -188,15 +189,15 @@
 class GptChat:
 
   def __init__(self, session: GptChatSession, configs: GptChatSessionConfigs):
     self.session = session
     self.configs = configs
 
   def process_prompt(self, prompt: str):
-    self.session.process_prompt(prompt)
+    self.session.process_prompt(prompt, self.configs)
 
   def create_new_session(self):
     self.session = GptChatSession.create_new(self.configs)
     set_active_session_id(self.session.session_id)
     print('Started new session')
 
   def update_configs(self, configs: GptChatSessionConfigs):
```

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/credentials.py` & `rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/credentials.py`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/session_store.py` & `rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/session_store.py`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/chat_gpt/setup_gpt.py` & `rubberduck-ai-0.6.0/rubberduck_chat/chat_gpt/setup_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
   if previous_session:
     return GptChat(previous_session, chat_session_configs)
   else:
     return GptChat(get_new_session(chat_session_configs), chat_session_configs)
 
 
 def get_gpt_chat_configs() -> GptChatSessionConfigs:
-  return GptChatSessionConfigs(config_collection.max_messages_per_request.get_int_value(),
+  return GptChatSessionConfigs(config_collection.chat_gpt_model.get_value(),
+                               config_collection.max_messages_per_request.get_int_value(),
                                config_collection.snippet_header_background_color.get_value(),
                                config_collection.snippet_theme.get_value())
 
 
 def restore_previous_session(configs: GptChatSessionConfigs) -> Optional[GptChatSession]:
   always_continue_last_session = config_collection.always_continue_last_session.get_bool_value()
   active_session = get_active_session()
```

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/configs.py` & `rubberduck-ai-0.6.0/rubberduck_chat/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,20 @@
   )
   inactive_session_cutoff_time_in_seconds = ConfigEntry(
     'inactive_session_cutoff_time_in_seconds',
     str(172800),
     'Creat new session if previous session is inactive for this many seconds',
     is_valid_int
   )
+  chat_gpt_model = ConfigEntry(
+    'chat_gpt_model',
+    'gpt-3.5-turbo',
+    'ChatGPT model; [gpt-3.5-turbo/gpt-4]',
+    None
+  )
   max_messages_per_request = ConfigEntry(
     'max_messages_per_request',
     str(10),
     'Maximum number of previous chat user prompts used to generating new responses',
     is_valid_int
   )
   snippet_header_background_color = ConfigEntry(
@@ -150,14 +156,15 @@
 
 
 config_collection = ConfigSet()
 config_collection_list: List[ConfigEntry] = [
   config_collection.max_saved_session_count,
   config_collection.always_continue_last_session,
   config_collection.inactive_session_cutoff_time_in_seconds,
+  config_collection.chat_gpt_model,
   config_collection.max_messages_per_request,
   config_collection.snippet_header_background_color,
   config_collection.snippet_theme,
   config_collection.exit_command_trigger,
   config_collection.help_command_trigger,
   config_collection.change_session_command_trigger,
   config_collection.print_session_command_trigger,
```

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/input_handler.py` & `rubberduck-ai-0.6.0/rubberduck_chat/input_handler.py`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/rubberduck_chat/rubberduck.py` & `rubberduck-ai-0.6.0/rubberduck_chat/rubberduck.py`

 * *Files identical despite different names*

### Comparing `rubberduck-ai-0.5.8/setup.py` & `rubberduck-ai-0.6.0/setup.py`

 * *Files identical despite different names*

