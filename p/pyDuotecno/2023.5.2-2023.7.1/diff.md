# Comparing `tmp/pyDuotecno-2023.5.2.tar.gz` & `tmp/pyDuotecno-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.5.2.tar", last modified: Mon May  8 15:36:20 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.7.1.tar", last modified: Tue Jul 11 13:25:29 2023, max compression
```

## Comparing `pyDuotecno-2023.5.2.tar` & `pyDuotecno-2023.7.1.tar`

### file list

```diff
@@ -1,22 +1,37 @@
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-05-08 15:36:20.076539 pyDuotecno-2023.5.2/
--rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.5.2/LICENSE
--rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.5.2/MANIFEST.in
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-05-08 15:36:20.076539 pyDuotecno-2023.5.2/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      155 2023-05-05 12:02:57.000000 pyDuotecno-2023.5.2/README.md
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-05-08 15:36:20.066538 pyDuotecno-2023.5.2/duotecno/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     3435 2023-04-19 09:42:05.000000 pyDuotecno-2023.5.2/duotecno/controller.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     2396 2023-04-22 17:09:47.000000 pyDuotecno-2023.5.2/duotecno/node.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     7625 2023-04-19 09:37:06.000000 pyDuotecno-2023.5.2/duotecno/protocol.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     2948 2023-04-22 17:10:29.000000 pyDuotecno-2023.5.2/duotecno/unit.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-05-08 15:36:20.066538 pyDuotecno-2023.5.2/examples/
--rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.5.2/examples/read.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-05-08 15:36:20.073205 pyDuotecno-2023.5.2/pyDuotecno.egg-info/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-05-08 15:36:19.000000 pyDuotecno-2023.5.2/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      334 2023-05-08 15:36:20.000000 pyDuotecno-2023.5.2/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-05-08 15:36:20.000000 pyDuotecno-2023.5.2/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.5.2/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-05-08 15:36:20.000000 pyDuotecno-2023.5.2/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-05-08 15:29:25.000000 pyDuotecno-2023.5.2/pyproject.toml
--rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.5.2/requirements.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-05-08 15:36:20.076539 pyDuotecno-2023.5.2/setup.cfg
--rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.5.2/setup.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.1/LICENSE
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.1/MANIFEST.in
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      155 2023-05-05 12:02:57.000000 pyDuotecno-2023.7.1/README.md
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.233271 pyDuotecno-2023.7.1/duotecno/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     5254 2023-07-11 13:07:49.000000 pyDuotecno-2023.7.1/duotecno/controller.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      126 2023-05-26 08:51:17.000000 pyDuotecno-2023.7.1/duotecno/exceptions.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.1/duotecno/node.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.1/duotecno/protocol.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     3668 2023-05-26 08:51:18.000000 pyDuotecno-2023.7.1/duotecno/unit.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.236605 pyDuotecno-2023.7.1/examples/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.1/examples/read.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.243272 pyDuotecno-2023.7.1/pyDuotecno.egg-info/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-11 13:23:21.000000 pyDuotecno-2023.7.1/pyproject.toml
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.1/requirements.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/setup.cfg
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.1/setup.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.223271 pyDuotecno-2023.7.1/venv/
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/venv/bin/
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rstpep2html.py
```

### Comparing `pyDuotecno-2023.5.2/LICENSE` & `pyDuotecno-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.5.2/PKG-INFO` & `pyDuotecno-2023.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.5.2
+Version: 2023.7.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.5.2/duotecno/node.py` & `pyDuotecno-2023.7.1/duotecno/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 
 from duotecno.protocol import NodeType, EV_NODEDATABASEINFO_2
 from duotecno.unit import (
     BaseUnit,
     SwitchUnit,
     SensUnit,
@@ -14,14 +15,15 @@
 class Node:
     name: str
     index: int
     nodeType: NodeType
     address: int
     numUnits: int
     units: dict
+    isloaded: asyncio.Event
 
     def __init__(
         self,
         name: str,
         address: int,
         index: int,
         nodeType: NodeType,
@@ -31,25 +33,40 @@
         self._log = logging.getLogger("pyduotecno-node")
         self.name = name
         self.address = address
         self.index = index
         self.numUnits = numUnits
         self.nodeType = nodeType
         self.writer = writer
+        self.isLoaded = asyncio.Event()
+        self.isLoaded.clear()
         self.units = {}
-        self._log.info(f"New node found: {self.name}")
+        self._log.debug(f"New node found: {self.name}")
+
+    def get_name(self) -> str:
+        return self.name
+
+    def get_address(self) -> str:
+        return self.address
 
     def __repr__(self) -> str:
         items = []
         for k, v in self.__dict__.items():
             if k not in ["_log", "writer"]:
                 items.append(f"{k} = {v!r}")
         return "{}[{}]".format(type(self), ", ".join(items))
 
-    async def requestUnits(self) -> None:
+    def get_unit_by_type(self, unit_type):
+        res = []
+        for unit in self.units.values():
+            if str(type(unit)) == f"<class 'duotecno.unit.{unit_type}'>":
+                res.append(unit)
+        return res
+
+    async def load(self) -> None:
         self._log.debug(f"Node {self.name}: Requesting units")
         for i in range(self.numUnits - 1):
             await self.writer(f"[209,2,{self.address},{i}]")
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_NODEDATABASEINFO_2):
             if packet.unit not in self.units:
@@ -66,12 +83,13 @@
                     u = VirtualUnit
                 else:
                     self._log.warning(f"Unhandled unitType: {packet.unitTypeName}")
                 self.units[packet.unit] = u(
                     self, name=packet.unitName, unit=packet.unit, writer=self.writer
                 )
                 await self.units[packet.unit].requestStatus()
+            if len(self.units) == self.numUnits - 1:
+                self.isLoaded.set()
             return
         if hasattr(packet, "unit") and packet.unit in self.units:
             await self.units[packet.unit].handlePacket(packet)
-            print(self.units)
             return
```

### Comparing `pyDuotecno-2023.5.2/duotecno/protocol.py` & `pyDuotecno-2023.7.1/duotecno/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import final
 from enum import Enum, unique
 from dataclasses import dataclass, field
 import collections
 import sys
 import json
-import logging
 
 
 @unique
 class MsgType(Enum):
     EV_UNITCONTROLSTATUS = 4
     EV_UNITDIMSTATUS = 5
     EV_UNITSWITCHSTATUS = 6
```

### Comparing `pyDuotecno-2023.5.2/duotecno/unit.py` & `pyDuotecno-2023.7.1/duotecno/unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import final
+from typing import final, Awaitable, Callable
 import logging
 from duotecno.protocol import (
     EV_UNITDUOSWITCHSTATUS_0,
     EV_UNITDIMSTATUS_0,
     EV_UNITSWITCHSTATUS_0,
     EV_UNITSENSSTATUS_0,
 )
@@ -22,18 +22,33 @@
         writer,
     ) -> None:
         self._log = logging.getLogger("pyduotecno-unit")
         self.node = node
         self.name = name
         self.unit = unit
         self.writer = writer
-        self._log.info(
+        self._log.debug(
             f"New Unit: '{self.node.name}' => '{self.name}' = {type(self).__name__}"
         )
 
+    def get_node_address(self) -> str:
+        return self.node.get_address()
+
+    def get_node_name(self) -> str:
+        return self.node.get_name()
+
+    def get_name(self) -> str:
+        return self.name
+
+    def get_number(self) -> int:
+        return self.unit
+
+    def on_status_update(self, meth: Callable[[], Awaitable[None]]) -> None:
+        self._on_status_update.append(meth)
+
     def __repr__(self) -> str:
         items = []
         for k, v in self.__dict__.items():
             if k not in ["_log", "writer"]:
                 items.append(f"{k} = {v!r}")
         return "{}[{}]".format(type(self), ", ".join(items))
 
@@ -80,22 +95,33 @@
             await self._update({"state": packet.state, "value": packet.dimValue})
             return
         await super().handlePacket(packet)
 
 
 class SwitchUnit(BaseUnit):
     _unitType: final = 2
-    _state: int
+    _state: int = None
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITSWITCHSTATUS_0):
             await self._update({"state": packet.state})
             return
         await super().handlePacket(packet)
 
+    def is_on(self):
+        return self._state
+
+    async def turn_on(self):
+        """Switch on."""
+        await self.writer(f"[163,3,{self.node.address},{self.unit}]")
+
+    async def turn_off(self):
+        """Switch off."""
+        await self.writer(f"[163,2,{self.node.address},{self.unit}]")
+
 
 class DuoswitchUnit(BaseUnit):
     _unitType: final = 8
     _state: int
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITDUOSWITCHSTATUS_0):
```

### Comparing `pyDuotecno-2023.5.2/examples/read.py` & `pyDuotecno-2023.7.1/examples/read.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.5.2/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.7.1/pyDuotecno.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.5.2
+Version: 2023.7.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.5.2/pyproject.toml` & `pyDuotecno-2023.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name        = "pyDuotecno"
 license     = {text = "Apache"}
-version     = "2023.5.2"
+version     = "2023.7.1"
 description = "Open-source home automation platform running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords    = ["home", "duotecno", "automation"]
 classifiers = [
@@ -38,15 +38,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
 
 [tool.bumpver]
-current_version = "2023.5.2"
+current_version = "2023.7.1"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

