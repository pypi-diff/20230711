# Comparing `tmp/openhab_pythonrule_engine-1.2.6.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.6.tar", last modified: Mon Jul 10 15:32:47 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.7.tar", last modified: Tue Jul 11 04:53:53 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.6.tar` & `openhab_pythonrule_engine-1.2.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.6/PKG-INFO` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab_pythonrule_engine
-Version: 1.2.6
+Name: openhab-pythonrule-engine
+Version: 1.2.7
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.6/README.md` & `openhab_pythonrule_engine-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cron_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import logging
 import time
 import requests
 import json
 import sseclient
+from datetime import datetime
 from threading import Thread
 from typing import Optional
 from dataclasses import dataclass
 
 
-logging = logging.getLogger(__name__)
-
-
-
 
 @dataclass()
 class ItemEvent:
     item_name: str
     operation: str
     payload: str
 
@@ -41,33 +38,38 @@
             openhab_uri = openhab_uri + "/"
         self.event_uri =  openhab_uri + "rest/events"
         self.event_listener = event_listener
         self.is_running = True
         self.thread = None
 
     def start(self):
+        logging.info("opening sse stream " + self.event_uri)
         self.thread = Thread(target=self.__listen, daemon=True)
         self.thread.start()
 
     def __listen(self):
+        previous_error_time = None
         while self.is_running:
             try:
-                logging.info("opening sse stream (" + self.event_uri + ")")
                 response = requests.get(self.event_uri, stream=True)
                 client = sseclient.SSEClient(response)
-
+                if previous_error_time is not None:
+                    logging.info("sse stream " + self.event_uri + " re-opened (after " + str(round((datetime.now() - previous_error_time).total_seconds()/60)) + " min)")
+                previous_error_time = None
                 try:
                     for event in client.events():
                         data = json.loads(event.data)
                         self.event_listener.on_event(data)
                 finally:
                     logging.debug("closing sse stream")
                     client.close()
                     response.close()
             except Exception as e:
-                logging.error("error occurred consuming sse of " + self.event_uri, e)
+                if previous_error_time is None:
+                    logging.warning("sse stream " + self.event_uri + " disconnected: " + str(e))
+                    previous_error_time = datetime.now()
                 time.sleep(5)
 
     def stop(self):
         self.is_running = False
         Thread.join(self.thread)
```

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_change_processor.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_change_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_registry.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/processor.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
             logging.warning("error occurred calling " + self.listener + " " + str(e))
 
     @property
     def triggers(self) -> Set[Trigger]:
         return set().union(*self.trigger_by_module.values())
 
     def add_trigger(self, trigger: Trigger):
-        logging.info(" * " + trigger.name + "(...): trigger '" + trigger.expression + "' has been registered")
+        logging.info(" * register " +  trigger.module + "#" + trigger.name + "(...) - trigger '" + trigger.expression + "'")
         triggers = self.trigger_by_module.get(trigger.module, set())
         triggers.add(trigger)
         self.trigger_by_module[trigger.module] = triggers
         self.on_add_trigger(trigger)
 
     def remove_triggers(self, module: str):
         if module in self.trigger_by_module.keys():
-            logging.info("removing all " + str(len(self.trigger_by_module[module])) + " " + self.name + " trigger of '" + module + "'")
+            logging.info(" * unregister " + module + " (" + self.name + ")")
             del self.trigger_by_module[module]
         self.on_remove_triggers(module)
 
     def process_trigger(self, trigger: Trigger):
         try:
             trigger.invoke(self.item_registry)
             self.last_executed = datetime.now().strftime("%H:%M:%S") + ' - ' + trigger.module + '.py  @when("' + trigger.expression + '")'
```

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 
 class RuleEngine:
 
     def __init__(self, openhab_uri:str, python_rule_directory: str, user: str, pwd: str):
         self.is_running = False
         self.openhab_uri = openhab_uri
-        logging.info("connecting " + openhab_uri)
         self.loaded_modules = dict()
         self.last_executed = ""
         self.last_error = ""
         self.__item_registry = ItemRegistry(openhab_uri, user, pwd)
         self.__processors = [ItemChangeProcessor(openhab_uri, self.__item_registry, self.on_executed),
                              CronProcessor(self.__item_registry, self.on_executed),
                              RuleLoadedProcessor(self.__item_registry, self.on_executed)]
```

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/source_scanner.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/trigger.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab-pythonrule-engine
-Version: 1.2.6
+Name: openhab_pythonrule_engine
+Version: 1.2.7
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.6/setup.py` & `openhab_pythonrule_engine-1.2.7/setup.py`

 * *Files identical despite different names*

