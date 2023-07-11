# Comparing `tmp/bondzai.gateway-sdk-0.0.7.tar.gz` & `tmp/bondzai.gateway-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-sdk-0.0.7.tar", last modified: Mon Jul 10 18:00:20 2023, max compression
+gzip compressed data, was "bondzai.gateway-sdk-0.0.8.tar", last modified: Tue Jul 11 18:22:54 2023, max compression
```

## Comparing `bondzai.gateway-sdk-0.0.7.tar` & `bondzai.gateway-sdk-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:20.200379 bondzai.gateway-sdk-0.0.7/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      604 2023-07-10 18:00:20.201395 bondzai.gateway-sdk-0.0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      155 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:19.504550 bondzai.gateway-sdk-0.0.7/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:19.992056 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/
--rwxrwxrwx   0 root         (0) root         (0)      139 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10202 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/agent.py
--rwxrwxrwx   0 root         (0) root         (0)     2497 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/commands.py
--rwxrwxrwx   0 root         (0) root         (0)      255 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/config.py
--rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     6937 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/events.py
--rwxrwxrwx   0 root         (0) root         (0)     4429 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/gateway.py
--rwxrwxrwx   0 root         (0) root         (0)     3288 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/message.py
--rwxrwxrwx   0 root         (0) root         (0)      810 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/request.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/responses.py
--rwxrwxrwx   0 root         (0) root         (0)      771 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/timer.py
--rwxrwxrwx   0 root         (0) root         (0)     1396 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/transcode.py
--rwxrwxrwx   0 root         (0) root         (0)      738 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:20.173659 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      604 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 18:00:18.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)    21241 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-07-10 18:00:20.205415 bondzai.gateway-sdk-0.0.7/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.648080 bondzai.gateway-sdk-0.0.8/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-11 18:22:54.648179 bondzai.gateway-sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      155 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.639413 bondzai.gateway-sdk-0.0.8/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.646008 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/
+-rw-r--r--   0 theo       (501) staff       (20)      139 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)    10475 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/agent.py
+-rw-r--r--   0 theo       (501) staff       (20)     2593 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/commands.py
+-rw-r--r--   0 theo       (501) staff       (20)      255 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/config.py
+-rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     6937 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/events.py
+-rw-r--r--   0 theo       (501) staff       (20)     4429 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/gateway.py
+-rw-r--r--   0 theo       (501) staff       (20)     3288 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/message.py
+-rw-r--r--   0 theo       (501) staff       (20)      810 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/request.py
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/responses.py
+-rw-r--r--   0 theo       (501) staff       (20)      771 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/timer.py
+-rw-r--r--   0 theo       (501) staff       (20)     1396 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/transcode.py
+-rw-r--r--   0 theo       (501) staff       (20)      738 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.647874 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      770 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       61 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)    21241 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-11 18:22:54.648746 bondzai.gateway-sdk-0.0.8/setup.cfg
```

### Comparing `bondzai.gateway-sdk-0.0.7/NOTICE` & `bondzai.gateway-sdk-0.0.8/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/PKG-INFO` & `bondzai.gateway-sdk-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/agent.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .gateway import Gateway
 
 from .request import Request, RequestActions
 from .message import EventMessage, Message, MessageModule, MessageType, CommandMessage
 from .enums import EventOperationID, AgentAIMode, AgentAIType, AgentTriggerType, CommandOperationID, \
-    LogCommand, DBMCommandParameter, DBMTable, DBMCommand, LogCommandParameter
+    LogCommand, DBMCommandParameter, DBMTable, DBMCommand, LogCommandParameter, RUNCommandParameter
 from .utils import unpack_buffer_to_list, b642b
 from .timer import Timer
 
 from .transcode import transcode
 
 
 class Agent:
@@ -244,7 +244,13 @@
                 msg.add_payload(DBMCommand.DBM_EXPORT_ROW.value, table.get("handle"), "", i)
                 data = self.send_message(msg, sync=True)
                 attr = data.get("attributes")
                 if attr is not None:
                     results.append(attr)
 
         return results
+    
+    def get_asl_meta(self) -> dict:
+        msg = CommandMessage(CommandOperationID.CMD_GET, MessageModule.RUN)
+        msg.add_payload(RUNCommandParameter.RUN_PARAM_APPS.value)
+        data = self.send_message(msg, sync=True)
+        return data
```

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/commands.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
         }
     },
     MessageModule.DBM: {
         CommandOperationID.CMD_GET : CommandGet,            
         CommandOperationID.CMD_START : {
             DBMCommand.DBM_EXPORT_ROW.value: CommandStartDbmExportRow
         }
+    },
+    MessageModule.RUN: {
+        CommandOperationID.CMD_GET : CommandGet,            
     }
 }
 
 
 def get_command_class(command_op_id: CommandOperationID, module: MessageModule, *args):
     if module not in OP_TO_COMMAND_TYPES:
         return None
```

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/enums.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -259,7 +259,28 @@
     KPI_SIZE_BYTE = 17
     KPI_SIZE_KBYTE = 18
     KPI_QI = 19
     KPI_OTHER_FLOAT = 20
     KPI_TRAINING_NET_LAYERS = 21
 
 
+class RUNCommandParameter(Enum):
+    RUN_PARAM_BREAK = 0x0100
+    RUN_PARAM_APPS = 0x0200
+    RUN_PARAM_OPS = 0x0300
+
+
+class MALCommandParameter(Enum):
+    MAL_PARAM_NB_THREADS = 0x0100
+    MAL_PARAM_DATA_SOURCES = 0x0200
+    MAL_PARAM_LIFE_CYCLE = 0x0300
+    MAL_PARAM_NVM_FILE = 0x8100
+    MAL_PARAM_CLEAR_NVM = 0x8200
+    MAL_PARAM_MONITORING = 0x2000
+
+
+class BLDCommandParameter(Enum):
+    BLD_PARAM_LINUX_LIB_NAMES = 0x8000
+    BLD_PARAM_LINUX_PYTHON_SCRIPT_NAME = 0x8001
+    BLD_PARAM_CORTEXM_INIT_DONE = 0x8002
+
+
```

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/events.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/gateway.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/gateway.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/message.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/message.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/request.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/timer.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/transcode.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/transcode.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/utils.py` & `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/PKG-INFO` & `bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/SOURCES.txt` & `bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/pyproject.toml` & `bondzai.gateway-sdk-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.7/setup.cfg` & `bondzai.gateway-sdk-0.0.8/setup.cfg`

 * *Files identical despite different names*

