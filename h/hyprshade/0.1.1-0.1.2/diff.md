# Comparing `tmp/hyprshade-0.1.1.tar.gz` & `tmp/hyprshade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.1.1.tar", max compression
+gzip compressed data, was "hyprshade-0.1.2.tar", max compression
```

## Comparing `hyprshade-0.1.1.tar` & `hyprshade-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.1.1/LICENSE
--rw-r--r--   0        0        0       44 2023-07-05 23:37:20.434170 hyprshade-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.1.1/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.1.1/hyprshade/__main__.py
--rw-r--r--   0        0        0     2577 2023-07-11 02:45:55.459709 hyprshade-0.1.1/hyprshade/cli.py
--rw-r--r--   0        0        0     3553 2023-07-11 02:52:15.538679 hyprshade-0.1.1/hyprshade/config.py
--rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.1.1/hyprshade/helpers.py
--rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.1.1/hyprshade/utils.py
--rw-r--r--   0        0        0     1002 2023-07-11 02:51:45.314681 hyprshade-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 hyprshade-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.1.2/LICENSE
+-rw-r--r--   0        0        0       44 2023-07-05 23:37:20.434170 hyprshade-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.1.2/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.1.2/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2577 2023-07-11 08:22:08.168519 hyprshade-0.1.2/hyprshade/cli.py
+-rw-r--r--   0        0        0     3349 2023-07-11 12:47:30.057291 hyprshade-0.1.2/hyprshade/config.py
+-rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.1.2/hyprshade/helpers.py
+-rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.1.2/hyprshade/utils.py
+-rw-r--r--   0        0        0     1002 2023-07-11 12:52:04.437286 hyprshade-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 hyprshade-0.1.2/PKG-INFO
```

### Comparing `hyprshade-0.1.1/LICENSE` & `hyprshade-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.1/hyprshade/cli.py` & `hyprshade-0.1.2/hyprshade/cli.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.1/hyprshade/config.py` & `hyprshade-0.1.2/hyprshade/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from collections.abc import Iterable
 from datetime import time
 from itertools import chain, pairwise
 from os import path
-from typing import Any, Literal, NotRequired, TypedDict, TypeGuard, cast
+from typing import Literal, NotRequired, TypedDict, cast
 
 import tomllib
 from more_itertools import nth, partition
 
 from hyprshade.utils import hyprshade_config_home, is_time_between
 
+TimeInterval = tuple[time, time]
+
 
 class ShadeDict(TypedDict):
     name: str
     start_time: time
     end_time: NotRequired[time]
 
 
@@ -62,52 +64,44 @@
     def __init__(self, config_dict: ConfigDict):
         default_shade, other_shades = partition_shades(config_dict["shades"])
         sorted_shades = sorted(other_shades, key=lambda s: s["start_time"])
         self.entries = list(map(ScheduleEntry, sorted_shades))
         self.default_shade_name = default_shade and default_shade["name"]
 
     def find_shade(self, t: time) -> str | None:
-        for entry_name, start_time, end_time in self._resolved_entries():
+        for entry_name, (start_time, end_time) in self._resolved_entries():
             if is_time_between(t, start_time, end_time):
                 return entry_name
 
         return self.default_shade_name
 
     def on_calendar_entries(self) -> Iterable[time]:
         for entry in self.entries:
             yield entry.start_time
             if entry.end_time is not None:
                 yield entry.end_time
 
-    def _resolved_entries(self):
+    def _resolved_entries(self) -> Iterable[tuple[str, TimeInterval]]:
         for entry, next_entry in pairwise(chain(self.entries, [self.entries[0]])):
             start_time = entry.start_time
             end_time = entry.end_time or next_entry.start_time
-            yield entry.name, start_time, end_time
+            yield entry.name, (start_time, end_time)
 
 
 class Config:
     """Parses config.toml into a dict"""
 
     _config_dict: ConfigDict
 
     def __init__(self, config_path: str | None = None):
         if config_path is None:
             config_path = Config.get_path()
 
         config_dict = Config._load(config_path)
-        if Config._validate(config_dict):
-            self._config_dict = config_dict
-
-    @staticmethod
-    def _validate(config_dict: dict[str, Any]) -> TypeGuard[ConfigDict]:
-        """Validates schema, and rejects any config that has overlapping time ranges."""
-
-        return True
-        raise NotImplementedError
+        self._config_dict = cast(ConfigDict, config_dict)
 
     @staticmethod
     def _load(config_path: str) -> dict[str, object]:
         with open(config_path, "rb") as f:
             return tomllib.load(f)
 
     @staticmethod
```

### Comparing `hyprshade-0.1.1/hyprshade/helpers.py` & `hyprshade-0.1.2/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.1/hyprshade/utils.py` & `hyprshade-0.1.2/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.1/pyproject.toml` & `hyprshade-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 
 [tool.poetry.dependencies]
```

