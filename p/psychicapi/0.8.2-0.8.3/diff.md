# Comparing `tmp/psychicapi-0.8.2.tar.gz` & `tmp/psychicapi-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.8.2.tar", last modified: Tue Jul 11 00:20:55 2023, max compression
+gzip compressed data, was "psychicapi-0.8.3.tar", last modified: Tue Jul 11 00:26:04 2023, max compression
```

## Comparing `psychicapi-0.8.2.tar` & `psychicapi-0.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.713343 psychicapi-0.8.2/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-11 00:20:55.713222 psychicapi-0.8.2/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4271 2023-07-10 00:22:36.000000 psychicapi-0.8.2/README.md
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.712410 psychicapi-0.8.2/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-07-07 03:04:36.000000 psychicapi-0.8.2/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)    11229 2023-07-10 23:48:43.000000 psychicapi-0.8.2/psychicapi/psychic.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:20:55.713061 psychicapi-0.8.2/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-07-11 00:20:55.000000 psychicapi-0.8.2/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-07-11 00:20:55.713385 psychicapi-0.8.2/setup.cfg
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-07-10 23:49:15.000000 psychicapi-0.8.2/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:26:04.663705 psychicapi-0.8.3/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     5072 2023-07-11 00:26:04.663602 psychicapi-0.8.3/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4806 2023-07-11 00:24:57.000000 psychicapi-0.8.3/README.md
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:26:04.662911 psychicapi-0.8.3/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-07-07 03:04:36.000000 psychicapi-0.8.3/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)    11229 2023-07-10 23:48:43.000000 psychicapi-0.8.3/psychicapi/psychic.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-11 00:26:04.663452 psychicapi-0.8.3/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     5072 2023-07-11 00:26:04.000000 psychicapi-0.8.3/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-07-11 00:26:04.000000 psychicapi-0.8.3/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-07-11 00:26:04.000000 psychicapi-0.8.3/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-07-11 00:26:04.000000 psychicapi-0.8.3/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-07-11 00:26:04.000000 psychicapi-0.8.3/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-07-11 00:26:04.663736 psychicapi-0.8.3/setup.cfg
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-07-11 00:26:01.000000 psychicapi-0.8.3/setup.py
```

### Comparing `psychicapi-0.8.2/PKG-INFO` & `psychicapi-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.8.2
+Version: 0.8.3
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
@@ -56,24 +56,42 @@
 
 To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
 
 ```
 page_cursor = None
 all_messages = []
 while True:
-    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.gmail, page_cursor=page_cursor)
     if messages_response is None:
         break
     all_messages.extend(messages_response.messages)
     page_cursor = messages_response.next_page_cursor
     if page_cursor is None:
         break
 print(all_messages)
 ```
 
+### Retrieve tickets from a connection
+
+To retrieve messages from connectors like `zendesk`, use the `get_tickets` function.
+
+```
+page_cursor = None
+all_tickets = []
+while True:
+    tickets_response = psychic.get_tickets(account_id="account_id", connector_id=ConnectorId.zendesk, redact_pii=True, page_cursor=page_cursor)
+    if tickets_response is None:
+        break
+    all_tickets.extend(tickets_response.tickets)
+    page_cursor = tickets_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_tickets)
+```
+
 ## Advanced Filtering
 
 ### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
 
 ```
```

### Comparing `psychicapi-0.8.2/README.md` & `psychicapi-0.8.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,24 +48,42 @@
 
 To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
 
 ```
 page_cursor = None
 all_messages = []
 while True:
-    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.gmail, page_cursor=page_cursor)
     if messages_response is None:
         break
     all_messages.extend(messages_response.messages)
     page_cursor = messages_response.next_page_cursor
     if page_cursor is None:
         break
 print(all_messages)
 ```
 
+### Retrieve tickets from a connection
+
+To retrieve messages from connectors like `zendesk`, use the `get_tickets` function.
+
+```
+page_cursor = None
+all_tickets = []
+while True:
+    tickets_response = psychic.get_tickets(account_id="account_id", connector_id=ConnectorId.zendesk, redact_pii=True, page_cursor=page_cursor)
+    if tickets_response is None:
+        break
+    all_tickets.extend(tickets_response.tickets)
+    page_cursor = tickets_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_tickets)
+```
+
 ## Advanced Filtering
 
 ### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
 
 ```
```

### Comparing `psychicapi-0.8.2/psychicapi/psychic.py` & `psychicapi-0.8.3/psychicapi/psychic.py`

 * *Files identical despite different names*

### Comparing `psychicapi-0.8.2/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.8.3/psychicapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.8.2
+Version: 0.8.3
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
@@ -56,24 +56,42 @@
 
 To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
 
 ```
 page_cursor = None
 all_messages = []
 while True:
-    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.gmail, page_cursor=page_cursor)
     if messages_response is None:
         break
     all_messages.extend(messages_response.messages)
     page_cursor = messages_response.next_page_cursor
     if page_cursor is None:
         break
 print(all_messages)
 ```
 
+### Retrieve tickets from a connection
+
+To retrieve messages from connectors like `zendesk`, use the `get_tickets` function.
+
+```
+page_cursor = None
+all_tickets = []
+while True:
+    tickets_response = psychic.get_tickets(account_id="account_id", connector_id=ConnectorId.zendesk, redact_pii=True, page_cursor=page_cursor)
+    if tickets_response is None:
+        break
+    all_tickets.extend(tickets_response.tickets)
+    page_cursor = tickets_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_tickets)
+```
+
 ## Advanced Filtering
 
 ### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
 
 ```
```

### Comparing `psychicapi-0.8.2/setup.py` & `psychicapi-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.8.2',
+    version='0.8.3',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

