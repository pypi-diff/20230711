# Comparing `tmp/rasa_sdk-3.6.1.tar.gz` & `tmp/rasa_sdk-3.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.6.1.tar", max compression
+gzip compressed data, was "rasa_sdk-3.7.0b1.tar", max compression
```

## Comparing `rasa_sdk-3.6.1.tar` & `rasa_sdk-3.7.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11553 2023-07-11 15:17:13.734800 rasa_sdk-3.6.1/LICENSE.txt
--rw-r--r--   0        0        0     5282 2023-07-11 15:17:13.734800 rasa_sdk-3.6.1/README.md
--rw-r--r--   0        0        0     3122 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/pyproject.toml
--rw-r--r--   0        0        0      420 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/__init__.py
--rw-r--r--   0        0        0      947 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1528 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      399 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/constants.py
--rw-r--r--   0        0        0     5727 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6459 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15183 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/forms.py
--rw-r--r--   0        0        0    12929 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0    10413 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     8091 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     7266 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     1035 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/plugin.py
--rw-r--r--   0        0        0     7066 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/slots.py
--rw-r--r--   0        0        0     1683 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/types.py
--rw-r--r--   0        0        0    11308 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/utils.py
--rw-r--r--   0        0        0      116 2023-07-11 15:17:13.738800 rasa_sdk-3.6.1/rasa_sdk/version.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rasa_sdk-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11553 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/LICENSE.txt
+-rw-r--r--   0        0        0     5282 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/README.md
+-rw-r--r--   0        0        0     3124 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1528 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      399 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     5727 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6459 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15183 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    12929 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0    10413 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     8091 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     7266 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     1039 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/plugin.py
+-rw-r--r--   0        0        0     7066 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     1683 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11308 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      118 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rasa_sdk-3.7.0b1/PKG-INFO
```

### Comparing `rasa_sdk-3.6.1/LICENSE.txt` & `rasa_sdk-3.7.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/README.md` & `rasa_sdk-3.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/pyproject.toml` & `rasa_sdk-3.7.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.6.1"
+version = "3.7.0b1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
```

### Comparing `rasa_sdk-3.6.1/rasa_sdk/__main__.py` & `rasa_sdk-3.7.0b1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.7.0b1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/endpoint.py` & `rasa_sdk-3.7.0b1/rasa_sdk/endpoint.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/events.py` & `rasa_sdk-3.7.0b1/rasa_sdk/events.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/exceptions.py` & `rasa_sdk-3.7.0b1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/executor.py` & `rasa_sdk-3.7.0b1/rasa_sdk/executor.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/forms.py` & `rasa_sdk-3.7.0b1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/interfaces.py` & `rasa_sdk-3.7.0b1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/actions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/storage.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/plugin.py` & `rasa_sdk-3.7.0b1/rasa_sdk/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,14 @@
     try:
         # rasa_sdk_plugin is a custom package
         # which extends existing functionality on rasa action server via plugins
         import rasa_sdk_plugins
 
         rasa_sdk_plugins.init_hooks(manager)
     except ModuleNotFoundError as e:
-        logger.debug("No plugins found: %s", e)
+        logger.info("No plugins found", exc_info=e)
         pass
 
 
 @hookspec
 def attach_sanic_app_extensions(app: Sanic) -> None:
     """Hook specification for attaching sanic listeners, routes and middlewares."""
```

### Comparing `rasa_sdk-3.6.1/rasa_sdk/slots.py` & `rasa_sdk-3.7.0b1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/types.py` & `rasa_sdk-3.7.0b1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/rasa_sdk/utils.py` & `rasa_sdk-3.7.0b1/rasa_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.1/PKG-INFO` & `rasa_sdk-3.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-sdk
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
```

