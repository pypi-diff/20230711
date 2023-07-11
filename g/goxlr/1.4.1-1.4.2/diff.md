# Comparing `tmp/goxlr-1.4.1.tar.gz` & `tmp/goxlr-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.1.tar", last modified: Tue Jul 11 12:56:42 2023, max compression
+gzip compressed data, was "goxlr-1.4.2.tar", last modified: Tue Jul 11 14:12:13 2023, max compression
```

## Comparing `goxlr-1.4.1.tar` & `goxlr-1.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 12:56:31.000000 goxlr-1.4.1/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 12:56:31.000000 goxlr-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 12:56:42.517770 goxlr-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 12:56:31.000000 goxlr-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 12:56:31.000000 goxlr-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 12:56:42.517770 goxlr-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 12:56:31.000000 goxlr-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 14:11:59.000000 goxlr-1.4.2/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 14:11:59.000000 goxlr-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 14:12:13.123291 goxlr-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 14:11:59.000000 goxlr-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.119291 goxlr-1.4.2/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.119291 goxlr-1.4.2/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 14:11:59.000000 goxlr-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 14:12:13.123291 goxlr-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 14:11:59.000000 goxlr-1.4.2/setup.py
```

### Comparing `goxlr-1.4.1/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.2/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/LICENSE.txt` & `goxlr-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/PKG-INFO` & `goxlr-1.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.1/README.md` & `goxlr-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/goxlr/commands/daemon.py` & `goxlr-1.4.2/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/goxlr/commands/goxlr.py` & `goxlr-1.4.2/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/goxlr/commands/status.py` & `goxlr-1.4.2/goxlr/commands/status.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.1/goxlr/socket.py` & `goxlr-1.4.2/goxlr/socket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import List
 import websockets
 import json
 
-from goxlr.types.models import Mixer, Status
+from .types.models import Mixer, Patch, Status, IDType
 
 from .commands import DaemonCommands, GoXLRCommands, StatusCommands
 
 from .error import DaemonError, MixerNotFoundError
 
 
 class Socket:
@@ -72,36 +72,34 @@
             if status := data.get("Status"):
                 return status
             elif patch := data.get("Patch"):
                 return patch
             elif error := data.get("Error"):
                 raise DaemonError(error)
 
-    async def receive(self, id=None):
+    async def receive(self, id: IDType | int = None):
         """
         Waits for a response from the daemon. If an ID is specified, it will
         wait until it receives a response with the same ID and queue all other
         responses.
 
-        If no ID is specified, it will wait for the first response and will
-        not add it to the queue.
-
-        To wait for a heartbeat response, specify an ID of 0.
-        To wait for a patch response, specify an ID of 2**64 - 1.
-
-        :param id: The ID of the response to wait for.
+        :param id: The ID of the response to wait for. If not specified, it
+                   will wait for the first response and will not add it to
+                   the queue.
 
         :return: The response from the daemon.
 
         :raises: `DaemonError` if the daemon returns an error.
         """
         if not id:
             response = await self.socket.recv()
             response = json.loads(response)
             return response
+        elif isinstance(id, IDType):
+            id = id.value
 
         # if we already have the response, return it
         for r in self.response_queue:
             if r.get("id") == id:
                 self.response_queue.remove(r)
                 return r
 
@@ -116,14 +114,25 @@
                 if response.get("id") in (0, 2**64 - 1):
                     # no need to queue heartbeat and patch responses
                     # if we want to do something with them, either specify
                     # the id or don't specify one at all
                     continue
                 self.response_queue.append(response)
 
+    async def receive_patch(self) -> List[Patch]:
+        """
+        Helper method to wait for a patch message from the daemon.
+
+        :return: The patch from the daemon.
+        """
+        response = await self.receive(IDType.Patch)
+        patches = response.get("data").get("Patch")
+
+        return [Patch(p) for p in patches]
+
     async def open(self):
         """
         Alias for `connect()`.
 
         :return: True if the connection was successful, False otherwise.
         """
         return await self.connect()
@@ -186,14 +195,31 @@
         self.status = await self.get_status()
 
         if self.serial:
             self.mixer = self.select_mixer(self.serial)
 
         return self.status
 
+    async def receive_patch(self, update: bool = True) -> List[Patch]:
+        """
+        Helper method to wait for a patch message from the daemon.
+
+        :param update: Whether or not to update the status and mixers attributes
+                       after receiving the patch.
+
+        :return: The patch from the daemon.
+        """
+
+        patches = await self.receive_patch()
+
+        if update:
+            await self.update()
+
+        return patches
+
     def select_mixer(self, serial: str = None):
         """
         Chooses a mixer to interact with.
 
         :param serial: The serial number of the mixer to interact with.
                        If not specified, it will default to the first mixer.
```

### Comparing `goxlr-1.4.1/goxlr/types/enums.py` & `goxlr-1.4.2/goxlr/types/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,7 +586,21 @@
     Off = 3
 
 
 class DeviceType(Enum):
     Unknown = 1
     Full = 2
     Mini = 3
+
+
+class IDType(Enum):
+    Heartbeat: int = 0
+    Patch: int = 2**64 - 1
+
+
+class PatchOperation(Enum):
+    Add = 1
+    Remove = 2
+    Replace = 3
+    Copy = 4
+    Move = 5
+    Test = 6
```

### Comparing `goxlr-1.4.1/goxlr/types/models.py` & `goxlr-1.4.2/goxlr/types/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from .enums import *
 
 # --------------------------------------------------
 # Config
 # --------------------------------------------------
 
 
@@ -767,7 +767,24 @@
     def __init__(self, status: dict):
         self.config = Config(status.get("config"))
         self.mixers = {
             serial: Mixer(mixer) for serial, mixer in status.get("mixers").items()
         }
         self.paths = Paths(status.get("paths"))
         self.files = Files(status.get("files"))
+
+
+# -------------------------------------------------------
+# Patch
+# -------------------------------------------------------
+
+
+@dataclass
+class Patch:
+    operation: PatchOperation
+    path: str
+    value: Any
+
+    def __init__(self, patch: dict):
+        self.operation = PatchOperation[patch.get("op").title()]
+        self.path = patch.get("path")
+        self.value = patch.get("value")
```

### Comparing `goxlr-1.4.1/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.2/goxlr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.1/setup.py` & `goxlr-1.4.2/setup.py`

 * *Files identical despite different names*

