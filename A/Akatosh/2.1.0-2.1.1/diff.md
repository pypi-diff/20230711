# Comparing `tmp/Akatosh-2.1.0.tar.gz` & `tmp/Akatosh-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.0.tar", last modified: Tue Jul 11 11:43:22 2023, max compression
+gzip compressed data, was "Akatosh-2.1.1.tar", last modified: Tue Jul 11 12:53:33 2023, max compression
```

## Comparing `Akatosh-2.1.0.tar` & `Akatosh-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.080116 Akatosh-2.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.064604 Akatosh-2.1.0/Akatosh/
--rw-rw-rw-   0        0        0      181 2023-07-11 07:31:54.000000 Akatosh-2.1.0/Akatosh/__init__.py
--rw-rw-rw-   0        0        0     5122 2023-07-11 11:37:41.000000 Akatosh-2.1.0/Akatosh/entity.py
--rw-rw-rw-   0        0        0    11594 2023-07-11 11:31:04.000000 Akatosh-2.1.0/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-06-30 03:47:46.000000 Akatosh-2.1.0/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-11 05:33:51.000000 Akatosh-2.1.0/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-11 04:40:17.000000 Akatosh-2.1.0/Akatosh/states.py
--rw-rw-rw-   0        0        0     5467 2023-07-11 08:04:04.000000 Akatosh-2.1.0/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.076116 Akatosh-2.1.0/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-11 11:43:22.078115 Akatosh-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-11 11:42:13.000000 Akatosh-2.1.0/README.md
--rw-rw-rw-   0        0        0      635 2023-07-11 11:42:45.000000 Akatosh-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 11:43:22.080116 Akatosh-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.871408 Akatosh-2.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.856414 Akatosh-2.1.1/Akatosh/
+-rw-rw-rw-   0        0        0      181 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0     5122 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    11587 2023-07-11 12:50:46.000000 Akatosh-2.1.1/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/states.py
+-rw-rw-rw-   0        0        0     5467 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.867410 Akatosh-2.1.1/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-11 12:53:33.869408 Akatosh-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.1/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-11 12:52:28.000000 Akatosh-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:53:33.871408 Akatosh-2.1.1/setup.cfg
```

### Comparing `Akatosh-2.1.0/Akatosh/entity.py` & `Akatosh-2.1.1/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.0/Akatosh/event.py` & `Akatosh-2.1.1/Akatosh/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 import inspect
 from abc import abstractmethod
 from typing import Any, Callable, List
 from uuid import uuid4
 
-from Akatosh.event import Event
-
 from .logger import logger
 from .states import State
 from .universe import Mundus
 
 
 class Event:
     def __init__(
@@ -295,14 +293,15 @@
                 self._at = round(self.interval() + Mundus.now, Mundus.resolution)
             else:
                 self._at = round(self.interval + Mundus.now, Mundus.resolution)
             if self.at <= self.till:
                 logger.debug(f"Event {self.label} next step is at {self.at}.")
                 Mundus.future_events.append(self)
             else:
+                self.end()
                 logger.debug(f"Event {self.label} is ended.")
             Mundus.current_events.remove(self)
             Mundus.past_events.append(self)
 
     @property
     def interval(self) -> int | float | Callable[..., Any]:
         """Return the interval between each action repeat."""
```

### Comparing `Akatosh-2.1.0/Akatosh/resource.py` & `Akatosh-2.1.1/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.0/Akatosh/universe.py` & `Akatosh-2.1.1/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.0/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.1/Akatosh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.0/PKG-INFO` & `Akatosh-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.0/README.md` & `Akatosh-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.0/pyproject.toml` & `Akatosh-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.0"
+version = "2.1.1"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

