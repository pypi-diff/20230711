# Comparing `tmp/gpt4-api-0.2.3.tar.gz` & `tmp/gpt4-api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.2.3.tar", last modified: Tue Jul 11 07:15:50 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.2.4.tar", last modified: Tue Jul 11 07:42:45 2023, max compression
```

## Comparing `gpt4-api-0.2.3.tar` & `gpt4-api-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.3/api/Logger.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.3/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    10260 2023-07-11 07:15:22.000000 gpt4-api-0.2.3/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.3/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.4/api/Logger.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.4/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10302 2023-07-11 07:42:32.000000 gpt4-api-0.2.4/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-07-11 07:42:45.000000 gpt4-api-0.2.4/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.4/setup.py
```

### Comparing `gpt4-api-0.2.3/api/Logger.py` & `gpt4-api-0.2.4/api/Logger.py`

 * *Files identical despite different names*

### Comparing `gpt4-api-0.2.3/api/gpt.py` & `gpt4-api-0.2.4/api/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
         self.completion_tokens = 0
         self.call_back = call_back
         self.threads = []
         self.__worker_flag = True
 
     def __worker(self, run_func):
         while True:
+            task = self.task_queue.get(timeout=1)
             try:
-                task = self.task_queue.get(timeout=1)
                 if task:
                     content = task.get("ask")
                     messages = task.get("messages")
                     run_func(task, content, messages)
                     self.task_queue.task_done()
             except Empty:
                 break
             except Exception as e:
-                logging.error(e)
-                break
+                logging.error("__worker error", e)
+                self.task_queue.put(task)
 
     def __run_tasks(self, tasks, run_func):
         logging.info("total tasks: %s" % len(tasks))
         for task in tasks:
             task["retry"] = False
             self.task_queue.put(task)
         if len(tasks) * 2 < self.num_threads:
@@ -113,15 +113,14 @@
                 open_ai_key = token
                 break
             else:
                 logging.info("token: %s limit: %s" % (token, token_limit))
         return open_ai_key
 
     def __release_token(self, open_ai_key):
-        time.sleep(0.5)
         self.usable_openai_keys[open_ai_key] = 0
 
     @staticmethod
     def get_active_thread_count():
         return threading.active_count() - 1
 
     def task_is_empty(self):
@@ -167,14 +166,15 @@
                 if call_back_func and self.call_back:
                     call_back_func = self.call_back.get(call_back_func, None)
                     if call_back_func:
                         call_back_func(call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name))
             except openai.error.RateLimitError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
                 self.__release_token(open_ai_key)
+                time.sleep(0.5)
                 self.__retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.Timeout as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request timed out: {e} ")
                 self.__retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.APIConnectionError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request timed out, OpenAI API request failed to connect: {e}")
                 self.__retry_on_error(task, ask_content, messages, retries=retries)
```

### Comparing `gpt4-api-0.2.3/setup.py` & `gpt4-api-0.2.4/setup.py`

 * *Files identical despite different names*

