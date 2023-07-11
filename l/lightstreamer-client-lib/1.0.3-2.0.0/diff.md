# Comparing `tmp/lightstreamer-client-lib-1.0.3.tar.gz` & `tmp/lightstreamer-client-lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightstreamer-client-lib-1.0.3.tar", last modified: Thu Jun 22 07:33:49 2023, max compression
+gzip compressed data, was "lightstreamer-client-lib-2.0.0.tar", last modified: Tue Jul 11 08:52:57 2023, max compression
```

## Comparing `lightstreamer-client-lib-1.0.3.tar` & `lightstreamer-client-lib-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.156802 lightstreamer-client-lib-1.0.3/
--rw-r--r--   0 acarioni   (501) staff       (20)    11357 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/LICENSE
--rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-06-22 07:33:49.156004 lightstreamer-client-lib-1.0.3/PKG-INFO
--rw-r--r--   0 acarioni   (501) staff       (20)     4517 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/README.md
--rw-r--r--   0 acarioni   (501) staff       (20)      783 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/pyproject.toml
--rw-r--r--   0 acarioni   (501) staff       (20)       38 2023-06-22 07:33:49.157016 lightstreamer-client-lib-1.0.3/setup.cfg
--rw-r--r--   0 acarioni   (501) staff       (20)       37 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/setup.py
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.115185 lightstreamer-client-lib-1.0.3/src/
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.114869 lightstreamer-client-lib-1.0.3/src/lightstreamer/
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.137976 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/
--rw-r--r--   0 acarioni   (501) staff       (20)       75 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/__init__.py
--rw-r--r--   0 acarioni   (501) staff       (20)     5499 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/com_lightstreamer_net.py
--rw-r--r--   0 acarioni   (501) staff       (20)    43272 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_api.py
--rw-r--r--   0 acarioni   (501) staff       (20)   749421 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_haxe.py
--rw-r--r--   0 acarioni   (501) staff       (20)   107900 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_wrapper.py
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.155097 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/
--rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/PKG-INFO
--rw-r--r--   0 acarioni   (501) staff       (20)      539 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/SOURCES.txt
--rw-r--r--   0 acarioni   (501) staff       (20)        1 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/dependency_links.txt
--rw-r--r--   0 acarioni   (501) staff       (20)       31 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/requires.txt
--rw-r--r--   0 acarioni   (501) staff       (20)       14 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/top_level.txt
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-07-11 08:52:57.826043 lightstreamer-client-lib-2.0.0/
+-rw-r--r--   0 acarioni   (501) staff       (20)    11357 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/LICENSE
+-rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-07-11 08:52:57.825597 lightstreamer-client-lib-2.0.0/PKG-INFO
+-rw-r--r--   0 acarioni   (501) staff       (20)     4517 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/README.md
+-rw-r--r--   0 acarioni   (501) staff       (20)      783 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/pyproject.toml
+-rw-r--r--   0 acarioni   (501) staff       (20)       38 2023-07-11 08:52:57.826159 lightstreamer-client-lib-2.0.0/setup.cfg
+-rw-r--r--   0 acarioni   (501) staff       (20)       37 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/setup.py
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-07-11 08:52:57.808130 lightstreamer-client-lib-2.0.0/src/
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-07-11 08:52:57.807930 lightstreamer-client-lib-2.0.0/src/lightstreamer/
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-07-11 08:52:57.819336 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/
+-rw-r--r--   0 acarioni   (501) staff       (20)       75 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/__init__.py
+-rw-r--r--   0 acarioni   (501) staff       (20)     5499 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/com_lightstreamer_net.py
+-rw-r--r--   0 acarioni   (501) staff       (20)    43417 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_api.py
+-rw-r--r--   0 acarioni   (501) staff       (20)   752536 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_haxe.py
+-rw-r--r--   0 acarioni   (501) staff       (20)   107900 2023-07-11 08:06:31.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_wrapper.py
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-07-11 08:52:57.825096 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/
+-rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-07-11 08:52:57.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/PKG-INFO
+-rw-r--r--   0 acarioni   (501) staff       (20)      539 2023-07-11 08:52:57.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)        1 2023-07-11 08:52:57.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)       31 2023-07-11 08:52:57.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/requires.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)       14 2023-07-11 08:52:57.000000 lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/top_level.txt
```

### Comparing `lightstreamer-client-lib-1.0.3/LICENSE` & `lightstreamer-client-lib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.3/PKG-INFO` & `lightstreamer-client-lib-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightstreamer-client-lib
-Version: 1.0.3
+Version: 2.0.0
 Summary: Lightstreamer Client SDK
 Author-email: Lightstreamer Srl <support@lightstreamer.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Lightstreamer/Lightstreamer-lib-client-haxe
 Keywords: lightstreamer,push,realtime,real-time
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -28,35 +28,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -82,34 +82,34 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
 LightstreamerClient.setLoggerProvider(loggerProvider)
 ```
 
 ## Compatibility ##
 
-Compatible with Lightstreamer Server since version 7.3.2.
+Compatible with Lightstreamer Server since version 7.4.0.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/2.0.0/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.3/README.md` & `lightstreamer-client-lib-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -66,34 +66,34 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
 LightstreamerClient.setLoggerProvider(loggerProvider)
 ```
 
 ## Compatibility ##
 
-Compatible with Lightstreamer Server since version 7.3.2.
+Compatible with Lightstreamer Server since version 7.4.0.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/2.0.0/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.3/pyproject.toml` & `lightstreamer-client-lib-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightstreamer-client-lib"
-version = "1.0.3"
+version = "2.0.0"
 description = "Lightstreamer Client SDK"
 readme = "README.md"
 authors = [{ name = "Lightstreamer Srl", email = "support@lightstreamer.com" }]
 license = { text = "Apache-2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/com_lightstreamer_net.py` & `lightstreamer-client-lib-2.0.0/src/lightstreamer/client/com_lightstreamer_net.py`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_api.py` & `lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,18 +151,19 @@
  Events for these listeners are dispatched by a different thread than the one that generates them.
  All the notifications for a single LightstreamerClient, including notifications to
  :class:`ClientListener`, :class:`SubscriptionListener` and :class:`ClientMessageListener` will be dispatched by the 
  same thread.
  Only one event per message is fired on this listener.
  """
 
-  def onProcessed(self,msg):
+  def onProcessed(self,msg,response):
     """Event handler that is called by Lightstreamer when the related message has been processed by the Server with success.
 
    :param originalMessage: the message to which this notification is related.
+   :param response: the response from the Metadata Adapter. If not supplied (i.e. supplied as null), an empty message is received here.
    """
     pass
 
   def onDeny(self,msg,code,error):
     """Event handler that is called by Lightstreamer when the related message has been processed by the Server but the 
    expected processing outcome could not be achieved for any reason.
```

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_haxe.py` & `lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_haxe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1547,15 +1547,15 @@
 
 
 class LSSubscription:
     _hx_class_name = "LSSubscription"
     _hx_is_interface = "False"
     __slots__ = ("eventDispatcher", "mode", "items", "fields", "group", "schema", "dataAdapter", "bufferSize", "snapshot", "requestedMaxFrequency", "selector", "dataAdapter2", "fields2", "schema2", "state", "subId", "cmdIdx", "keyIdx", "nItems", "nFields", "m_internal", "manager", "wrapper", "lock")
     _hx_fields = ["eventDispatcher", "mode", "items", "fields", "group", "schema", "dataAdapter", "bufferSize", "snapshot", "requestedMaxFrequency", "selector", "dataAdapter2", "fields2", "schema2", "state", "subId", "cmdIdx", "keyIdx", "nItems", "nFields", "m_internal", "manager", "wrapper", "lock"]
-    _hx_methods = ["initSnapshot", "initItemsAndFields", "addListener", "removeListener", "getListeners", "isActive", "isSubscribed", "getDataAdapter", "setDataAdapter", "getMode", "getItems", "setItems", "getItemGroup", "setItemGroup", "getFields", "setFields", "getFieldSchema", "setFieldSchema", "getRequestedBufferSize", "setRequestedBufferSize", "getRequestedSnapshot", "setRequestedSnapshot", "getRequestedMaxFrequency", "setRequestedMaxFrequency", "getSelector", "setSelector", "getCommandPosition", "getKeyPosition", "getCommandSecondLevelDataAdapter", "setCommandSecondLevelDataAdapter", "getCommandSecondLevelFields", "setCommandSecondLevelFields", "getCommandSecondLevelFieldSchema", "setCommandSecondLevelFieldSchema", "getValue", "getCommandValue", "getValuePosPos", "getValuePosName", "getValueNamePos", "getValueNameName", "getCommandValuePosPos", "getCommandValuePosName", "getCommandValueNamePos", "getCommandValueNameName", "getItemPos", "getFieldPos", "checkActive", "checkCommand", "fetch_mode", "fetch_requestedBufferSize", "fetch_requestedSnapshot", "fetch_requestedMaxFrequency", "fetch_nItems", "fetch_subManager", "setActive", "setInactive", "setSubscribed", "setSubscribedCMD", "fetch_nFields", "isInternal", "setInternal", "getItemName", "relate", "unrelate", "hasSnapshot", "getItemNameOrPos", "fireOnSubscription", "fireOnUnsubscription", "fireOnSubscriptionError", "fireOnEndOfSnapshot", "fireOnClearSnapshot", "fireOnLostUpdates", "fireOnItemUpdate", "fireOnRealMaxFrequency", "fireOnSubscriptionError2Level", "fireOnLostUpdates2Level", "toString"]
+    _hx_methods = ["initSnapshot", "initItemsAndFields", "addListener", "removeListener", "getListeners", "isActive", "isSubscribed", "getDataAdapter", "setDataAdapter", "getMode", "getItems", "setItems", "getItemGroup", "setItemGroup", "getFields", "setFields", "getFieldSchema", "setFieldSchema", "getRequestedBufferSize", "setRequestedBufferSize", "getRequestedSnapshot", "setRequestedSnapshot", "getRequestedMaxFrequency", "setRequestedMaxFrequency", "getSelector", "setSelector", "getCommandPosition", "getKeyPosition", "getCommandSecondLevelDataAdapter", "setCommandSecondLevelDataAdapter", "getCommandSecondLevelFields", "setCommandSecondLevelFields", "getCommandSecondLevelFieldSchema", "setCommandSecondLevelFieldSchema", "getValue", "getCommandValue", "getValuePosPos", "getValuePosName", "getValueNamePos", "getValueNameName", "getCommandValuePosPos", "getCommandValuePosName", "getCommandValueNamePos", "getCommandValueNameName", "getItemPos", "getFieldPos", "checkActive", "checkCommand", "fetch_items", "fetch_fields", "fetch_fields2", "fetch_mode", "fetch_requestedBufferSize", "fetch_requestedSnapshot", "fetch_requestedMaxFrequency", "fetch_nItems", "fetch_subManager", "setActive", "setInactive", "setSubscribed", "setSubscribedCMD", "fetch_nFields", "isInternal", "setInternal", "getItemName", "relate", "unrelate", "hasSnapshot", "getItemNameOrPos", "fireOnSubscription", "fireOnUnsubscription", "fireOnSubscriptionError", "fireOnEndOfSnapshot", "fireOnClearSnapshot", "fireOnLostUpdates", "fireOnItemUpdate", "fireOnRealMaxFrequency", "fireOnSubscriptionError2Level", "fireOnLostUpdates2Level", "toString"]
 
     def __init__(self,mode,items,fields,wrapper = None):
         self.manager = None
         self.nFields = None
         self.nItems = None
         self.keyIdx = None
         self.cmdIdx = None
@@ -2105,14 +2105,38 @@
         if self.isActive():
             raise com_lightstreamer_internal_IllegalStateException("Cannot modify an active Subscription. Please unsubscribe before applying any change")
 
     def checkCommand(self):
         if (self.mode != "COMMAND"):
             raise com_lightstreamer_internal_IllegalStateException("This method can only be used on COMMAND subscriptions")
 
+    def fetch_items(self):
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                return _gthis.items
+            return com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
+        return _hx_local_1()
+
+    def fetch_fields(self):
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                return _gthis.fields
+            return com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
+        return _hx_local_1()
+
+    def fetch_fields2(self):
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                return _gthis.fields2
+            return com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
+        return _hx_local_1()
+
     def fetch_mode(self):
         _gthis = self
         def _hx_local_1():
             def _hx_local_0():
                 return _gthis.mode
             return com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
         return _hx_local_1()
@@ -2811,15 +2835,17 @@
             else:
                 self.evtCONS(com_lightstreamer_internal_RealMaxBandwidth.BWLimited(com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.parseFloat(bw)))
         elif line.startswith("MSGDONE"):
             args = line.split(",")
             seq = (args[1] if 1 < len(args) else None)
             if (seq == "*"):
                 seq = "UNORDERED_MESSAGES"
-            self.evtMSGDONE(seq,com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.parseInt((args[2] if 2 < len(args) else None)))
+            prog = com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.parseInt((args[2] if 2 < len(args) else None))
+            rawResp = (args[3] if 3 < len(args) else None)
+            self.evtMSGDONE(seq,prog,("" if ((rawResp == "")) else com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.unquote(rawResp)))
         elif line.startswith("MSGFAIL"):
             args = line.split(",")
             seq = (args[1] if 1 < len(args) else None)
             if (seq == "*"):
                 seq = "UNORDERED_MESSAGES"
             self.evtMSGFAIL(seq,com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.parseInt((args[2] if 2 < len(args) else None)),com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.parseInt((args[3] if 3 < len(args) else None)),com_lightstreamer_client_internal__ParseTools_ParseTools_Fields_.unquote((args[4] if 4 < len(args) else None)))
         elif line.startswith("REQERR"):
@@ -4599,21 +4625,21 @@
                     self.state.s_slw = 332
                     self.state.traceState()
                     self.evtCheckAvg(result)
                 else:
                     pass
         return False
 
-    def evtMSGDONE(self,sequence,prog):
+    def evtMSGDONE(self,sequence,prog,response):
         self.traceEvent("MSGDONE")
         if com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.protocolLogger.isDebugEnabled():
-            com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.protocolLogger.debug(((("MSGDONE " + ("null" if sequence is None else sequence)) + " ") + Std.string(prog)))
+            com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.protocolLogger.debug(((((("MSGDONE " + ("null" if sequence is None else sequence)) + " ") + Std.string(prog)) + " ") + ("null" if response is None else response)))
         if self.state.inPushing():
             if self.isFreshData():
-                self.doMSGDONE(sequence,prog)
+                self.doMSGDONE(sequence,prog,response)
                 if self.state.inStreaming():
                     self.evtRestartKeepalive()
             else:
                 self.onStaleData()
                 if self.state.inStreaming():
                     self.evtRestartKeepalive()
 
@@ -5990,29 +6016,29 @@
         self.options.setPollingInterval(pollingMs)
 
     def doPROG(self,prog):
         if (prog > self.rec_clientProg):
             raise com_lightstreamer_internal_IllegalStateException(("Assertion failure: " + "prog <= rec_clientProg"))
         self.rec_serverProg = prog
 
-    def doMSGDONE(self,sequence,prog):
+    def doMSGDONE(self,sequence,prog,response):
         self.onFreshData()
         def _hx_local_0(msg):
             if (msg.sequence == sequence):
                 return (msg.prog == prog)
             else:
                 return False
         messages = self.messageManagers.filter(_hx_local_0)
         if (messages.length > 1):
             raise com_lightstreamer_internal_IllegalStateException(("Assertion failure: " + "messages.length <= 1"))
         _g_head = messages.h
         while (_g_head is not None):
             val = _g_head.item
             _g_head = _g_head.next
-            val.evtMSGDONE()
+            val.evtMSGDONE(response)
 
     def doMSGFAIL(self,sequence,prog,errorCode,errorMsg):
         self.onFreshData()
         if (errorCode == 39):
             count = Std.parseInt(errorMsg)
             if (count is None):
                 raise com_lightstreamer_internal_IllegalStateException(("Assertion failure: " + "count != null"))
@@ -7336,18 +7362,18 @@
 
     def onError(self,originalMessage):
         def _hx_local_0(listener):
             if (listener.onError is not None):
                 listener.onError(originalMessage)
         self.dispatchToAll(_hx_local_0)
 
-    def onProcessed(self,originalMessage):
+    def onProcessed(self,originalMessage,response):
         def _hx_local_0(listener):
             if (listener.onProcessed is not None):
-                listener.onProcessed(originalMessage)
+                listener.onProcessed(originalMessage,response)
         self.dispatchToAll(_hx_local_0)
 
 com_lightstreamer_client_internal_MessageEventDispatcher._hx_class = com_lightstreamer_client_internal_MessageEventDispatcher
 
 
 class com_lightstreamer_client_internal_MessageManager:
     _hx_class_name = "com.lightstreamer.client.internal.MessageManager"
@@ -7413,26 +7439,26 @@
         elif (_g == 12):
             self.doMSGFAIL(code,msg)
             self.finalize()
             self.goto(14)
         else:
             pass
 
-    def evtMSGDONE(self):
+    def evtMSGDONE(self,response):
         self.traceEvent("MSGDONE")
         _g = self.s_m
         if (_g == 10):
             self.finalize()
             self.goto(13)
         elif (_g == 11):
-            self.doMSGDONE()
+            self.doMSGDONE(response)
             self.finalize()
             self.goto(13)
         elif (_g == 12):
-            self.doMSGDONE()
+            self.doMSGDONE(response)
             self.finalize()
             self.goto(13)
         else:
             pass
 
     def evtREQOK(self,reqId):
         self.traceEvent("REQOK")
@@ -7508,16 +7534,16 @@
 
     def encode(self,isWS):
         return self.encodeMsg(isWS)
 
     def encodeWS(self):
         return ("msg\r\n" + HxOverrides.stringOrNull(self.encode(True)))
 
-    def doMSGDONE(self):
-        self.fireOnProcessed()
+    def doMSGDONE(self,response):
+        self.fireOnProcessed(response)
 
     def doMSGFAIL(self,code,msg):
         if ((code == 38) or ((code == 39))):
             self.fireOnDiscarded()
         elif (code <= 0):
             self.fireOnDeny(code,msg)
         elif ((code != 32) and ((code != 33))):
@@ -7554,18 +7580,18 @@
             req.LS_outcome(False)
             if isWS:
                 req.LS_ack(False)
         if com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.protocolLogger.isInfoEnabled():
             com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.protocolLogger.info(("Sending message: " + Std.string(req)))
         return req.getEncodedString()
 
-    def fireOnProcessed(self):
+    def fireOnProcessed(self,response):
         if com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.messageLogger.isInfoEnabled():
             com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.messageLogger.info((((("Message " + HxOverrides.stringOrNull(self.sequence)) + ":") + Std.string(self.prog)) + " processed"))
-        self.eventDispatcher.onProcessed(self.txt)
+        self.eventDispatcher.onProcessed(self.txt,response)
 
     def fireOnDiscarded(self):
         if com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.messageLogger.isWarnEnabled():
             com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.messageLogger.warn((((("Message " + HxOverrides.stringOrNull(self.sequence)) + ":") + Std.string(self.prog)) + " discarded"))
         self.eventDispatcher.onDiscarded(self.txt)
 
     def fireOnDeny(self,code,msg):
@@ -8403,15 +8429,15 @@
 
 
 class com_lightstreamer_client_internal_SubscriptionManagerLiving:
     _hx_class_name = "com.lightstreamer.client.internal.SubscriptionManagerLiving"
     _hx_is_interface = "False"
     __slots__ = ("subId", "m_subscription", "m_strategy", "m_lastAddReqId", "m_lastDeleteReqId", "m_lastReconfReqId", "m_currentMaxFrequency", "m_reqMaxFrequency", "m_client", "lock", "state")
     _hx_fields = ["subId", "m_subscription", "m_strategy", "m_lastAddReqId", "m_lastDeleteReqId", "m_lastReconfReqId", "m_currentMaxFrequency", "m_reqMaxFrequency", "m_client", "lock", "state"]
-    _hx_methods = ["finalize", "evtExtSubscribe", "evtExtUnsubscribe", "evtExtAbort", "evtREQERR", "evtREQOK", "evtSUBOK", "evtSUBCMD", "evtUNSUB", "evtU", "evtEOS", "evtCS", "evtOV", "evtCONF", "evtCheckFrequency", "evtExtConfigure", "isPending", "encode", "encodeWS", "getValue", "getCommandValue", "encodeAdd", "encodeDelete", "encodeReconf", "doSetActive", "doSetInactive", "doSubscribe", "doUnsubscribe", "doAbort", "genSendControl", "notifyOnSubscription", "notifyOnUnsubscription", "notifyOnSubscriptionError", "doConfigure", "doREQOKConfigure", "doSUBOK", "doSUBCMD", "doUNSUB", "doU", "doEOS", "doCS", "doOV", "doCONF", "traceEvent"]
+    _hx_methods = ["finalize", "evtExtSubscribe", "evtExtUnsubscribe", "evtExtAbort", "evtREQERR", "evtREQOK", "checkItems", "checkFields", "checkItemsAndFields", "evtSUBOK", "evtSUBCMD", "evtUNSUB", "evtU", "evtEOS", "evtCS", "evtOV", "evtCONF", "evtCheckFrequency", "evtExtConfigure", "isPending", "encode", "encodeWS", "getValue", "getCommandValue", "encodeAdd", "encodeDelete", "encodeReconf", "doSetActive", "doSetInactive", "doSubscribe", "doUnsubscribe", "doAbort", "genSendControl", "notifyOnSubscription", "notifyOnUnsubscription", "notifyOnSubscriptionError", "notifyOnSubscriptionError_CountMismatch", "doConfigure", "doREQOKConfigure", "doSUBOK", "doSUBCMD", "doUNSUB", "doU", "doEOS", "doCS", "doOV", "doCONF", "traceEvent"]
     _hx_statics = ["is2LevelCommand"]
     _hx_interfaces = [com_lightstreamer_client_internal_SubscriptionManager]
 
     def __init__(self,sub,client):
         self.state = None
         self.m_client = None
         self.m_reqMaxFrequency = None
@@ -8548,56 +8574,82 @@
             elif ((_gthis.state.s_c == 22) and ((reqId == _gthis.m_lastReconfReqId))):
                 _gthis.doREQOKConfigure()
                 _gthis.state.s_c = 20
                 _gthis.state.traceState()
                 _gthis.evtCheckFrequency()
         com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
 
+    def checkItems(self,expItems,nItems):
+        if (expItems is not None):
+            return (expItems == nItems)
+        else:
+            return True
+
+    def checkFields(self,expFields,nFields):
+        if (expFields is not None):
+            return (expFields == nFields)
+        else:
+            return True
+
+    def checkItemsAndFields(self,expItems,expFields,nItems,nFields):
+        if self.checkItems(expItems,nItems):
+            return self.checkFields(expFields,nFields)
+        else:
+            return False
+
     def evtSUBOK(self,nItems,nFields):
         _gthis = self
         def _hx_local_0():
             _gthis.traceEvent("SUBOK")
-            if (_gthis.state.s_m == 2):
-                _gthis.doSUBOK(nItems,nFields)
-                _gthis.notifyOnSubscription()
-                _gthis.state.s_m = 4
-                _gthis.state.s_s = 10
-                _gthis.state.s_c = 20
-                _gthis.state.traceState()
-                _gthis.evtCheckFrequency()
-            elif (_gthis.state.s_m == 3):
-                _gthis.doSUBOK(nItems,nFields)
-                _gthis.notifyOnSubscription()
-                _gthis.state.s_m = 4
-                _gthis.state.s_s = 10
-                _gthis.state.s_c = 20
-                _gthis.state.traceState()
-                _gthis.evtCheckFrequency()
+            if ((_gthis.state.s_m == 2) or ((_gthis.state.s_m == 3))):
+                tmp = _gthis.m_subscription.fetch_items()
+                expItems = (len(tmp) if ((tmp is not None)) else None)
+                tmp = _gthis.m_subscription.fetch_fields()
+                expFields = (len(tmp) if ((tmp is not None)) else None)
+                if _gthis.checkItemsAndFields(expItems,expFields,nItems,nFields):
+                    _gthis.doSUBOK(nItems,nFields)
+                    _gthis.notifyOnSubscription()
+                    _gthis.state.s_m = 4
+                    _gthis.state.s_s = 10
+                    _gthis.state.s_c = 20
+                    _gthis.state.traceState()
+                    _gthis.evtCheckFrequency()
+                else:
+                    _gthis.doUnsubscribe()
+                    _gthis.doSetInactive()
+                    _gthis.notifyOnSubscriptionError_CountMismatch(expItems,expFields,nItems,nFields)
+                    _gthis.state.s_m = 5
+                    _gthis.state.traceState()
+                    _gthis.genSendControl()
         com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
 
     def evtSUBCMD(self,nItems,nFields,keyIdx,cmdIdx):
         _gthis = self
         def _hx_local_0():
             _gthis.traceEvent("SUBCMD")
-            if (_gthis.state.s_m == 2):
-                _gthis.doSUBCMD(nItems,nFields,cmdIdx,keyIdx)
-                _gthis.notifyOnSubscription()
-                _gthis.state.s_m = 4
-                _gthis.state.s_s = 10
-                _gthis.state.s_c = 20
-                _gthis.state.traceState()
-                _gthis.evtCheckFrequency()
-            elif (_gthis.state.s_m == 3):
-                _gthis.doSUBCMD(nItems,nFields,cmdIdx,keyIdx)
-                _gthis.notifyOnSubscription()
-                _gthis.state.s_m = 4
-                _gthis.state.s_s = 10
-                _gthis.state.s_c = 20
-                _gthis.state.traceState()
-                _gthis.evtCheckFrequency()
+            if ((_gthis.state.s_m == 2) or ((_gthis.state.s_m == 3))):
+                tmp = _gthis.m_subscription.fetch_items()
+                expItems = (len(tmp) if ((tmp is not None)) else None)
+                tmp = _gthis.m_subscription.fetch_fields()
+                expFields = (len(tmp) if ((tmp is not None)) else None)
+                if _gthis.checkItemsAndFields(expItems,expFields,nItems,nFields):
+                    _gthis.doSUBCMD(nItems,nFields,cmdIdx,keyIdx)
+                    _gthis.notifyOnSubscription()
+                    _gthis.state.s_m = 4
+                    _gthis.state.s_s = 10
+                    _gthis.state.s_c = 20
+                    _gthis.state.traceState()
+                    _gthis.evtCheckFrequency()
+                else:
+                    _gthis.doUnsubscribe()
+                    _gthis.doSetInactive()
+                    _gthis.notifyOnSubscriptionError_CountMismatch(expItems,expFields,nItems,nFields)
+                    _gthis.state.s_m = 5
+                    _gthis.state.traceState()
+                    _gthis.genSendControl()
         com_lightstreamer_internal__RLock_RLock_Impl_.synchronized(self.lock,_hx_local_0)
 
     def evtUNSUB(self):
         _gthis = self
         def _hx_local_0():
             _gthis.traceEvent("UNSUB")
             if (_gthis.state.s_s == 10):
@@ -8866,14 +8918,20 @@
 
     def notifyOnUnsubscription(self):
         self.m_subscription.fireOnUnsubscription(self.subId)
 
     def notifyOnSubscriptionError(self,code,msg):
         self.m_subscription.fireOnSubscriptionError(self.subId,code,msg)
 
+    def notifyOnSubscriptionError_CountMismatch(self,expItems,expFields,nItems,nFields):
+        if (not self.checkItems(expItems,nItems)):
+            self.m_subscription.fireOnSubscriptionError(self.subId,61,((("Expected " + Std.string(expItems)) + " items but got ") + Std.string(nItems)))
+        else:
+            self.m_subscription.fireOnSubscriptionError(self.subId,61,((("Expected " + Std.string(expFields)) + " fields but got ") + Std.string(nFields)))
+
     def doConfigure(self):
         self.m_reqMaxFrequency = self.m_subscription.fetch_requestedMaxFrequency()
         self.m_strategy.evtSetRequestedMaxFrequency(self.m_reqMaxFrequency)
 
     def doREQOKConfigure(self):
         self.m_currentMaxFrequency = self.m_reqMaxFrequency
 
@@ -9615,29 +9673,29 @@
 
 
 class com_lightstreamer_client_internal_update_ItemUpdate2Level(com_lightstreamer_client_internal_update_AbstractItemUpdate):
     _hx_class_name = "com.lightstreamer.client.internal.update.ItemUpdate2Level"
     _hx_is_interface = "False"
     __slots__ = ("m_itemIdx", "m_items", "m_nFields", "m_fields", "m_fields2", "m_newValues", "m_changedFields", "m_isSnapshot", "m_jsonPatches")
     _hx_fields = ["m_itemIdx", "m_items", "m_nFields", "m_fields", "m_fields2", "m_newValues", "m_changedFields", "m_isSnapshot", "m_jsonPatches"]
-    _hx_methods = ["getItemName", "getItemPos", "isSnapshot", "getValue", "isValueChanged", "_getValueAsJSONPatchIfAvailable", "getValueAsJSONPatchIfAvailable", "getChangedFields", "getChangedFieldsByPosition", "getFields", "getFieldsByPosition", "getValuePos", "getValueName", "isValueChangedPos", "isValueChangedName", "getFieldNameFromIdx", "getFieldNameOrNullFromIdx", "getFieldIdxFromName", "toString"]
+    _hx_methods = ["getItemName", "getItemPos", "isSnapshot", "getValue", "isValueChanged", "_getValueAsJSONPatchIfAvailable", "getValueAsJSONPatchIfAvailable", "getChangedFields", "getChangedFieldsByPosition", "getFields", "getFieldsByPosition", "getValuePos", "getValueName", "isValueChangedPos", "isValueChangedName", "getFieldNameFromIdx", "getFieldIdxFromName", "toString"]
     _hx_statics = []
     _hx_interfaces = []
     _hx_super = com_lightstreamer_client_internal_update_AbstractItemUpdate
 
 
     def __init__(self,itemIdx,sub,newValues,changedFields,isSnapshot,jsonPatches):
-        items = sub.getItems()
-        fields = sub.getFields()
-        fields2 = sub.getCommandSecondLevelFields()
+        items = sub.fetch_items()
+        fields = sub.fetch_fields()
+        fields2 = sub.fetch_fields2()
         self.m_itemIdx = itemIdx
-        self.m_items = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap((list(items) if ((items is not None)) else None))
+        self.m_items = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap(items)
         self.m_nFields = com_lightstreamer_internal_NullTools.sure(sub.fetch_nFields())
-        self.m_fields = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap((list(fields) if ((fields is not None)) else None))
-        self.m_fields2 = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap((list(fields2) if ((fields2 is not None)) else None))
+        self.m_fields = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap(fields)
+        self.m_fields2 = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap(fields2)
         self.m_newValues = newValues.copy()
         self.m_changedFields = changedFields.copy()
         self.m_isSnapshot = isSnapshot
         self.m_jsonPatches = jsonPatches
 
     def getItemName(self):
         if (self.m_items is not None):
@@ -9687,17 +9745,18 @@
         _g = self.m_changedFields.iterator()
         while (_g.current < len(_g.array)):
             def _hx_local_1():
                 _hx_local_0 = _g.current
                 _g.current = (_g.current + 1)
                 return _hx_local_0
             fieldPos = python_internal_ArrayImpl._get(_g.array, _hx_local_1())
-            k = self.getFieldNameFromIdx(fieldPos)
-            v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(self.m_newValues.h.get(fieldPos,None))
-            res.h[k] = v
+            fieldName = self.getFieldNameFromIdx(fieldPos)
+            if (fieldName is not None):
+                v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(self.m_newValues.h.get(fieldPos,None))
+                res.h[fieldName] = v
         return com_lightstreamer_internal__NativeTypes_NativeStringMap_Impl_._new(res)
 
     def getChangedFieldsByPosition(self):
         res = haxe_ds_IntMap()
         _g = self.m_changedFields.iterator()
         while (_g.current < len(_g.array)):
             def _hx_local_1():
@@ -9714,17 +9773,18 @@
             raise com_lightstreamer_internal_IllegalStateException(com_lightstreamer_client_internal_update__ItemUpdateBase_ItemUpdateBase_Fields_.NO_FIELDS)
         res = haxe_ds_StringMap()
         this1 = self.m_newValues
         _g_keys = this1.keys()
         while _g_keys.hasNext():
             key = _g_keys.next()
             _g_value = this1.get(key)
-            k = self.getFieldNameFromIdx(key)
-            v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(_g_value)
-            res.h[k] = v
+            fieldName = self.getFieldNameFromIdx(key)
+            if (fieldName is not None):
+                v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(_g_value)
+                res.h[fieldName] = v
         return com_lightstreamer_internal__NativeTypes_NativeStringMap_Impl_._new(res)
 
     def getFieldsByPosition(self):
         _g = haxe_ds_IntMap()
         this1 = self.m_newValues
         _g_keys = this1.keys()
         while _g_keys.hasNext():
@@ -9751,21 +9811,14 @@
             raise com_lightstreamer_internal_IllegalStateException(com_lightstreamer_client_internal_update__ItemUpdateBase_ItemUpdateBase_Fields_.NO_FIELDS)
         fieldPos = self.getFieldIdxFromName(fieldName)
         if (fieldPos is None):
             raise com_lightstreamer_internal_IllegalArgumentException(com_lightstreamer_client_internal_update__ItemUpdateBase_ItemUpdateBase_Fields_.UNKNOWN_FIELD_NAME)
         return self.m_changedFields.contains(fieldPos)
 
     def getFieldNameFromIdx(self,fieldIdx):
-        if (self.m_fields is None):
-            raise com_lightstreamer_internal_IllegalStateException(("Assertion failure: " + "m_fields != null"))
-        if (self.m_fields2 is None):
-            raise com_lightstreamer_internal_IllegalStateException(("Assertion failure: " + "m_fields2 != null"))
-        return com_lightstreamer_internal_NullTools.sure(self.getFieldNameOrNullFromIdx(fieldIdx))
-
-    def getFieldNameOrNullFromIdx(self,fieldIdx):
         if (fieldIdx <= self.m_nFields):
             if (self.m_fields is not None):
                 return self.m_fields.h.get(fieldIdx,None)
             else:
                 return None
         elif (self.m_fields2 is not None):
             return self.m_fields2.h.get((fieldIdx - self.m_nFields),None)
@@ -9801,15 +9854,15 @@
         s_b = python_lib_io_StringIO()
         s_b.write("[")
         this1 = self.m_newValues
         _g_keys = this1.keys()
         while _g_keys.hasNext():
             key = _g_keys.next()
             _g_value = this1.get(key)
-            tmp = self.getFieldNameOrNullFromIdx(key)
+            tmp = self.getFieldNameFromIdx(key)
             fieldName = (tmp if ((tmp is not None)) else Std.string(key))
             fieldVal = Std.string(_g_value)
             if (key > 1):
                 s_b.write(",")
             s_b.write(Std.string(fieldName))
             s_b.write(":")
             s_b.write(Std.string(fieldVal))
@@ -9827,20 +9880,27 @@
     _hx_methods = ["getItemName", "getItemPos", "isSnapshot", "getValue", "isValueChanged", "_getValueAsJSONPatchIfAvailable", "getValueAsJSONPatchIfAvailable", "getChangedFields", "getChangedFieldsByPosition", "getFields", "getFieldsByPosition", "getValuePos", "getValueName", "isValueChangedPos", "isValueChangedName", "getFieldNameOrNullFromIdx", "getFieldIdxFromName", "toString"]
     _hx_statics = []
     _hx_interfaces = []
     _hx_super = com_lightstreamer_client_internal_update_AbstractItemUpdate
 
 
     def __init__(self,itemIdx,sub,newValues,changedFields,isSnapshot,jsonPatches):
-        items = sub.getItems()
-        fields = sub.getFields()
+        self.m_jsonPatches = None
+        self.m_isSnapshot = None
+        self.m_changedFields = None
+        self.m_newValues = None
+        items = sub.fetch_items()
+        fields = sub.fetch_fields()
         self.m_itemIdx = itemIdx
-        self.m_items = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap((list(items) if ((items is not None)) else None))
+        self.m_items = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap(items)
         self.m_nFields = com_lightstreamer_internal_NullTools.sure(sub.fetch_nFields())
-        self.m_fields = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap((list(fields) if ((fields is not None)) else None))
+        self.m_fields = com_lightstreamer_client_internal_update__UpdateUtils_UpdateUtils_Fields_.toMap(fields)
+        if ((fields is not None) and ((len(fields) != self.m_nFields))):
+            if com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.subscriptionLogger.isErrorEnabled():
+                com_lightstreamer_log__LoggerTools_LoggerTools_Fields_.subscriptionLogger.error(((((("Expected " + Std.string(self.m_nFields)) + " field names but got ") + Std.string(len(fields))) + ": ") + Std.string(fields)))
         self.m_newValues = newValues.copy()
         self.m_changedFields = changedFields.copy()
         self.m_isSnapshot = isSnapshot
         self.m_jsonPatches = jsonPatches
 
     def getItemName(self):
         if (self.m_items is not None):
@@ -9887,17 +9947,18 @@
         _g = self.m_changedFields.iterator()
         while (_g.current < len(_g.array)):
             def _hx_local_1():
                 _hx_local_0 = _g.current
                 _g.current = (_g.current + 1)
                 return _hx_local_0
             fieldPos = python_internal_ArrayImpl._get(_g.array, _hx_local_1())
-            k = com_lightstreamer_internal_NullTools.sure(self.m_fields.h.get(fieldPos,None))
-            v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(self.m_newValues.h.get(fieldPos,None))
-            res.h[k] = v
+            fieldName = self.m_fields.h.get(fieldPos,None)
+            if (fieldName is not None):
+                v = com_lightstreamer_client_internal_update_CurrFieldValTools.toString(self.m_newValues.h.get(fieldPos,None))
+                res.h[fieldName] = v
         return com_lightstreamer_internal__NativeTypes_NativeStringMap_Impl_._new(res)
 
     def getChangedFieldsByPosition(self):
         res = haxe_ds_IntMap()
         _g = self.m_changedFields.iterator()
         while (_g.current < len(_g.array)):
             def _hx_local_1():
@@ -16777,18 +16838,18 @@
 Math.PI = python_lib_Math.pi
 sys_thread__Thread_HxThread.threads = haxe_ds_ObjectMap()
 sys_thread__Thread_HxThread.threadsMutex = sys_thread_Mutex()
 sys_thread__Thread_HxThread.mainThread = sys_thread__Thread_HxThread(python_lib_Threading.current_thread())
 sys_thread__Thread_HxThread.mainThread.events = sys_thread_EventLoop()
 
 com_lightstreamer_client__ConnectionDetails_ConnectionDetails_Fields_.DEFAULT_SERVER = None
-com_lightstreamer_internal__Constants_Constants_Fields_.TLCP_VERSION = "TLCP-2.4.0"
+com_lightstreamer_internal__Constants_Constants_Fields_.TLCP_VERSION = "TLCP-2.5.0"
 com_lightstreamer_internal__Constants_Constants_Fields_.FULL_TLCP_VERSION = (HxOverrides.stringOrNull(com_lightstreamer_internal__Constants_Constants_Fields_.TLCP_VERSION) + ".lightstreamer.com")
-com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION = (("1.0.3" + " build ") + "20230622")
-com_lightstreamer_internal__Constants_Constants_Fields_.LS_CID = "v Wntytg4pkpW36AK3P4hwLri8M4OA68h8x"
+com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION = (("2.0.0" + " build ") + "20230711")
+com_lightstreamer_internal__Constants_Constants_Fields_.LS_CID = "v Wntytg4pkpW37AK3M4hwLri8M4OA69g7u"
 com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_NAME = "python_client"
 com_lightstreamer_internal__Constants_Constants_Fields_.LS_CREATE_REALM = ""
 LSLightstreamerClient.LIB_NAME = com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_NAME
 LSLightstreamerClient.LIB_VERSION = com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION
 com_lightstreamer_client__Proxy_ProxyType_Impl_.HTTP = "HTTP"
 com_lightstreamer_client__Proxy_ProxyType_Impl_.SOCKS4 = "SOCKS4"
 com_lightstreamer_client__Proxy_ProxyType_Impl_.SOCKS5 = "SOCKS5"
```

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_wrapper.py` & `lightstreamer-client-lib-2.0.0/src/lightstreamer/client/ls_python_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/PKG-INFO` & `lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightstreamer-client-lib
-Version: 1.0.3
+Version: 2.0.0
 Summary: Lightstreamer Client SDK
 Author-email: Lightstreamer Srl <support@lightstreamer.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Lightstreamer/Lightstreamer-lib-client-haxe
 Keywords: lightstreamer,push,realtime,real-time
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -28,35 +28,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -82,34 +82,34 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/2.0.0/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
 LightstreamerClient.setLoggerProvider(loggerProvider)
 ```
 
 ## Compatibility ##
 
-Compatible with Lightstreamer Server since version 7.3.2.
+Compatible with Lightstreamer Server since version 7.4.0.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/2.0.0/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/SOURCES.txt` & `lightstreamer-client-lib-2.0.0/src/lightstreamer_client_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

