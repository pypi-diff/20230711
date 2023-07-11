# Comparing `tmp/bondzai.gateway-0.0.6.tar.gz` & `tmp/bondzai.gateway-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.6.tar", last modified: Mon Jul 10 17:59:57 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.7.tar", last modified: Tue Jul 11 18:22:34 2023, max compression
```

## Comparing `bondzai.gateway-0.0.6.tar` & `bondzai.gateway-0.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:57.027040 bondzai.gateway-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      596 2023-07-10 17:59:57.028549 bondzai.gateway-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      195 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:55.529660 bondzai.gateway-0.0.6/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:55.739199 bondzai.gateway-0.0.6/bondzai/gateway/
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-07-10 17:59:44.000000 bondzai.gateway-0.0.6/bondzai/gateway/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      843 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/config.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.021670 bondzai.gateway-0.0.6/bondzai/gateway/core/
--rwxrwxrwx   0 root         (0) root         (0)     7995 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/application.py
--rwxrwxrwx   0 root         (0) root         (0)      328 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/device.py
--rwxrwxrwx   0 root         (0) root         (0)      577 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/events.py
--rwxrwxrwx   0 root         (0) root         (0)      833 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/fsm.py
--rwxrwxrwx   0 root         (0) root         (0)     2127 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2590 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.396433 bondzai.gateway-0.0.6/bondzai/gateway/core/message/
--rwxrwxrwx   0 root         (0) root         (0)     5391 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4968 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/command.py
--rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 17:59:44.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     6771 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/event.py
--rwxrwxrwx   0 root         (0) root         (0)      337 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/payload.py
--rwxrwxrwx   0 root         (0) root         (0)     6821 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/process_dbm.py
--rwxrwxrwx   0 root         (0) root         (0)     7864 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/response.py
--rwxrwxrwx   0 root         (0) root         (0)      942 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2276 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/observer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.564713 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/
--rwxrwxrwx   0 root         (0) root         (0)     1768 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/client.py
--rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/connector.py
--rwxrwxrwx   0 root         (0) root         (0)     1731 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/request.py
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.677460 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4426 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/serial.py
--rwxrwxrwx   0 root         (0) root         (0)     7630 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/socket_server.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.751476 bondzai.gateway-0.0.6/bondzai/gateway/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2280 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/tests/test_observer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.999090 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      596 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1382 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:54.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      913 2023-07-10 17:59:57.033070 bondzai.gateway-0.0.6/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.456060 bondzai.gateway-0.0.7/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-11 18:22:34.456163 bondzai.gateway-0.0.7/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.438880 bondzai.gateway-0.0.7/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.442073 bondzai.gateway-0.0.7/bondzai/gateway/
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/config.yml
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.445293 bondzai.gateway-0.0.7/bondzai/gateway/core/
+-rw-r--r--   0 theo       (501) staff       (20)     7995 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/application.py
+-rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/events.py
+-rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/fsm.py
+-rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/manager.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.449072 bondzai.gateway-0.0.7/bondzai/gateway/core/message/
+-rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/command.py
+-rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     6771 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/event.py
+-rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/payload.py
+-rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/process_dbm.py
+-rw-r--r--   0 theo       (501) staff       (20)     9408 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/response.py
+-rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.451662 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/
+-rw-r--r--   0 theo       (501) staff       (20)     1768 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/client.py
+-rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/connector.py
+-rw-r--r--   0 theo       (501) staff       (20)     1731 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/request.py
+-rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.452992 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/
+-rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/serial.py
+-rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/socket_server.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.453596 bondzai.gateway-0.0.7/bondzai/gateway/tests/
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/tests/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/tests/test_observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.455831 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/entry_points.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-11 18:22:34.456781 bondzai.gateway-0.0.7/setup.cfg
```

### Comparing `bondzai.gateway-0.0.6/NOTICE` & `bondzai.gateway-0.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/PKG-INFO` & `bondzai.gateway-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.7/bondzai/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/config.yml` & `bondzai.gateway-0.0.7/bondzai/gateway/config.yml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/application.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/command.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/enums.py`

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

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/event.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/event.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/process_dbm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import msgpack
 from dataclasses import dataclass
+from io import BytesIO
 
 from ..logger import log
 
 from .payload import MessagePayload
-from .enums import CommandOperationID, MessageModule, LogCommand, DBMCommand, LogCommandParameter,\
-                    DBMCommandParameter
+from .enums import BLDCommandParameter, CommandOperationID, MALCommandParameter, MessageModule, LogCommand, DBMCommand, LogCommandParameter,\
+                    DBMCommandParameter, RUNCommandParameter
 from .process_dbm import DbmProcesser
+from .utils import B2B64, B642B
 
 
 @dataclass
 class ResponseGetLogNbKpi:
     itemid: int    
     number: int
 
@@ -193,14 +196,73 @@
 
     def to_array(self) -> list:
         return [
             self.itemid,
             self.ops
         ]
 
+@dataclass
+class ResponseRunApp:
+    uuid: bytes
+    desc: str
+    threads: int
+    mem: list[int]
+    ops: list[int]
+    meta: dict
+
+    def to_dict(self) -> str:
+
+        stream = BytesIO(self.meta)
+        unpacker = msgpack.Unpacker(stream, raw=False, strict_map_key=False)
+
+        meta = unpacker.unpack()
+        return {
+            "uuid": B2B64(self.uuid),
+            "desc": self.desc,
+            "threads": self.threads,
+            "mem": self.mem,
+            "ops": self.ops,
+            "meta": meta
+        }
+    
+    def to_array(self) -> list:
+        packer = msgpack.Packer()
+        buffer = BytesIO()
+        buffer.write(packer.pack(self.meta))
+        buffer.seek(0)
+        return [
+            B642B(self.uuid),
+            self.desc,
+            self.threads,
+            self.mem,
+            self.ops,
+            buffer.read()
+        ]
+
+
+@dataclass
+class ResponseRunGetApps:
+    itemid: int
+    apps: list
+
+    def to_dict(self) -> str:
+
+        apps = [ResponseRunApp(*app).to_dict() for app in self.apps]
+
+        return {
+            "itemid": self.itemid,
+            "apps": apps
+        }
+
+    def to_array(self) -> list:
+        return [
+            self.itemid,
+            [self.app.to_array() for self.app in self.apps]
+        ]
+
 
 @dataclass
 class ResponseDbmCreateTable:
     itemid: int
     execid: int
     result: int
 
@@ -259,31 +321,32 @@
         CommandOperationID.CMD_START.value : {
             DBMCommand.DBM_EXPORT_ROW.value: ResponseDbmExportRow,
             DBMCommand.DBM_CREATE_TABLE.value: ResponseDbmCreateTable,
             DBMCommand.DBM_IMPORT_ROW.value: ResponseDbmImportRow
         } 
     },
 
-    # MessageModule.RUN.value: {
-    #     CommandOperationID.CMD_GET.value : {
-    #         PARAMETERS.RUN_PARAM_OPS.value: ResponseRunGetOps,
-    #     },
-    # },
-
-    # MessageModule.BLD.value: {
-    #     CommandOperationID.CMD_SET.value : {
-    #         PARAMETERS.BLD_PARAM_CORTEXM_INIT_DONE.value: ResponseBldSetInitDone,
-    #     },
-    # },
-
-    # MessageModule.MAL.value: {
-    #     CommandOperationID.CMD_GET.value : {
-    #         PARAMETERS.MAL_PARAM_LIFE_CYCLE.value: ResponseGetMalLifeCycle,
-    #     },
-    # },
+    MessageModule.RUN.value: {
+        CommandOperationID.CMD_GET.value : {
+            RUNCommandParameter.RUN_PARAM_OPS.value: ResponseRunGetOps,
+            RUNCommandParameter.RUN_PARAM_APPS.value: ResponseRunGetApps,
+        },
+    },
+
+    MessageModule.BLD.value: {
+        CommandOperationID.CMD_SET.value : {
+            BLDCommandParameter.BLD_PARAM_CORTEXM_INIT_DONE.value: ResponseBldSetInitDone,
+        },
+    },
+
+    MessageModule.MAL.value: {
+        CommandOperationID.CMD_GET.value : {
+            MALCommandParameter.MAL_PARAM_LIFE_CYCLE.value: ResponseGetMalLifeCycle,
+        },
+    },
 
 }
 
 
 def get_response_class(mod: int, op_id: int, raw_data: list):
     if not mod in OP_TO_RESPONSE_TYPES:
         return None
@@ -302,14 +365,15 @@
     def from_array(cls, mod: int, operation: int, raw_data: list) -> "MessagePayload":
         response_class = get_response_class(mod, operation, raw_data)
         if response_class is None:
             log(f"Operation {operation} unknown", logger_level="ERROR")
             return
 
         payload = cls()
+
         payload.command = response_class(*raw_data)
 
         return payload
 
     @classmethod
     def from_json(cls, mod: int, operation: int, raw_data: list) -> "MessagePayload":
         response_class = get_response_class(mod, operation, raw_data)
```

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/message/utils.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/message/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/client.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/serial.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/socket_server.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.7/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.7/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.6/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.7/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.6/setup.cfg` & `bondzai.gateway-0.0.7/setup.cfg`

 * *Files identical despite different names*

