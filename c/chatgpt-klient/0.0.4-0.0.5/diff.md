# Comparing `tmp/chatgpt-klient-0.0.4.tar.gz` & `tmp/chatgpt-klient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.4.tar", last modified: Tue Jul 11 09:42:39 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.0.5.tar", last modified: Tue Jul 11 11:28:06 2023, max compression
```

## Comparing `chatgpt-klient-0.0.4.tar` & `chatgpt-klient-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 09:42:39.076945 chatgpt-klient-0.0.4/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 09:42:39.076945 chatgpt-klient-0.0.4/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.4/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-11 09:39:50.000000 chatgpt-klient-0.0.4/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-11 09:42:39.076945 chatgpt-klient-0.0.4/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 09:42:39.072945 chatgpt-klient-0.0.4/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 09:42:39.076945 chatgpt-klient-0.0.4/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-11 09:40:05.000000 chatgpt-klient-0.0.4/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5550 2023-07-11 09:36:27.000000 chatgpt-klient-0.0.4/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.4/src/chatgpt_klient/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 09:42:39.076945 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 09:42:39.000000 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-07-11 09:42:39.000000 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-11 09:42:39.000000 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-11 09:42:39.000000 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-11 09:42:39.000000 chatgpt-klient-0.0.4/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.5/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-11 11:26:47.000000 chatgpt-klient-0.0.5/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.821171 chatgpt-klient-0.0.5/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.825171 chatgpt-klient-0.0.5/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-11 11:26:56.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5640 2023-07-11 11:26:05.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/top_level.txt
```

### Comparing `chatgpt-klient-0.0.4/src/chatgpt_klient/client.py` & `chatgpt-klient-0.0.5/src/chatgpt_klient/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,27 @@
     def clean_history(self):
         self.msg_history = {"messages": [], "tokens": []}
         self.last_prompt_tokens = 0
 
     def get_max_tokens_allowed(self):
         return min(self.max_tokens, MAX_TOKENS[self.engine])
 
-    def send_prompt(self, text=None, max_tokens=None):
+    def send_prompt(self, text=None, max_tokens=None, no_history=False):
         response = "No response"
         if self.engine in ENGINES0:
             r = self.openai.Completion.create(
                 engine=self.engine,
                 prompt=text,
                 max_tokens=max_tokens or self.get_max_tokens_allowed(),
             )
             response = r["choices"][0]["text"]
         elif self.engine in ENGINES1:
             if text:
+                if no_history:
+                    self.clean_history()
                 self.msg_history["messages"].append(
                     {
                         "role": "user",
                         "content": text,
                     }
                 )
                 self.msg_history["tokens"].append(len(self.encoding.encode(text)))
```

### Comparing `chatgpt-klient-0.0.4/src/chatgpt_klient/consts.py` & `chatgpt-klient-0.0.5/src/chatgpt_klient/consts.py`

 * *Files identical despite different names*

