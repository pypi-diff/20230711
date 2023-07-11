# Comparing `tmp/pykb-2.4.0.tar.gz` & `tmp/pykb-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykb-2.4.0.tar", last modified: Wed Mar 30 12:14:57 2022, max compression
+gzip compressed data, was "pykb-2.5.0.tar", last modified: Tue Jul 11 12:59:01 2023, max compression
```

## Comparing `pykb-2.4.0.tar` & `pykb-2.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-03-30 12:14:57.109513 pykb-2.4.0/
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      386 2022-03-30 12:14:57.109513 pykb-2.4.0/PKG-INFO
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    20331 2022-03-30 12:05:05.793281 pykb-2.4.0/kb.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      479 2022-03-30 12:12:46.841084 pykb-2.4.0/setup.py
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-11 12:59:01.723548 pykb-2.5.0/
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      386 2023-07-11 12:59:01.723548 pykb-2.5.0/PKG-INFO
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    20435 2023-07-11 12:51:51.312417 pykb-2.5.0/kb.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      479 2023-07-11 12:56:50.462933 pykb-2.5.0/setup.py
```

### Comparing `pykb-2.4.0/kb.py` & `pykb-2.5.0/kb.py`

 * *Files 3% similar despite different names*

```diff
@@ -418,20 +418,22 @@
 
     kb = None
     kb_thread = None
     kb_users = 0
 
     def __init__(self, defaultontology=None):
         try:
-            from minimalkb.kb import MinimalKB
+            from knowledge_core.kb import KnowledgeCore
         except ImportError:
-            raise KbError("Embedded kb required, but MinimalKB can not be imported!")
+            raise KbError(
+                "Embedded kb required, but KnowledgeCore can not be imported! Try 'pip install knowledge_core'"
+            )
 
-        minimalkblogger = logging.getLogger("minimalKB")
-        minimalkblogger.addHandler(NullHandler())
+        knowledgecorelogger = logging.getLogger("KnowledgeCore")
+        knowledgecorelogger.addHandler(NullHandler())
 
         kblogger.warn("Using embedded kb: events are not yet supported!")
 
         if not EmbeddedKBClient.kb:
             kblogger.info("Initializing the embedded knowledge base.")
             self._running = True
             EmbeddedKBClient.kb_thread = threading.Thread(
@@ -468,30 +470,31 @@
         else:
             return value
 
     def sendmsg(self, msg):
         self._incoming_response.put(msg)
 
     def process(self, defaultontology):
-        from minimalkb.kb import MinimalKB
+        from knowledge_core.kb import KnowledgeCore
 
-        EmbeddedKBClient.kb = MinimalKB(defaultontology)
+        EmbeddedKBClient.kb = KnowledgeCore(
+            [defaultontology] if defaultontology else []
+        )
         self._kb = EmbeddedKBClient.kb
         while self._running:
             EmbeddedKBClient.kb.process()
 
     def close(self):
         EmbeddedKBClient.kb_users -= 1
         if EmbeddedKBClient.kb_users == 0:
             kblogger.debug(
                 "Last user of the embedded knowledge base has left. "
                 + "Closing the knowledge base."
             )
             self._running = False
-            EmbeddedKBClient.kb.stop_services()
             EmbeddedKBClient.kb_thread.join()
             EmbeddedKBClient.kb = (
                 None  # reset kb to none so a new fresh thread may be created if needed.
             )
 
 
 class RemoteKBClient(asynchat.async_chat):
```

