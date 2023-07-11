# Comparing `tmp/atro_victoria-0.0.7.tar.gz` & `tmp/atro_victoria-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_victoria-0.0.7.tar", max compression
+gzip compressed data, was "atro_victoria-0.0.8.tar", max compression
```

## Comparing `atro_victoria-0.0.7.tar` & `atro_victoria-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.7/README.md
--rw-r--r--   0        0        0     1967 2023-07-11 20:51:13.945750 atro_victoria-0.0.7/atro_victoria/__init__.py
--rw-r--r--   0        0        0      409 2023-07-11 20:50:25.904739 atro_victoria-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.8/README.md
+-rw-r--r--   0        0        0     1745 2023-07-11 20:58:48.045299 atro_victoria-0.0.8/atro_victoria/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-11 20:58:52.975403 atro_victoria-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.8/PKG-INFO
```

### Comparing `atro_victoria-0.0.7/atro_victoria/__init__.py` & `atro_victoria-0.0.8/atro_victoria/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime
 from pydantic_core import Url
 import requests
 from pydantic import AnyHttpUrl, PastDatetime
 from pydantic_settings import BaseSettings, SettingsConfigDict
 from pathlib import Path
 
-def strigify_datetime(dt: datetime):
+def strigify_datetime(dt: datetime | None):
+  dt = dt or datetime.now()
   return int(dt.timestamp() * 1000)
 
 class VmCsvRowBase(BaseSettings):
   job: str 
   name: str
   timestamp: PastDatetime | None = None
   url: AnyHttpUrl = Url("http://localhost:8480/")
@@ -20,36 +21,30 @@
     vals = self.model_dump()
     counter = 0
     output = ""
     vals.pop('url')
     for val in vals:
       counter+=1
       if val == "timestamp":
-        if vals[val] is not None and isinstance(vals[val], datetime):
-          output += "," + str(counter) + ":time:unix_ms"
+        output += "," + str(counter) + ":time:unix_ms"
         continue
       if isinstance(vals[val], (int, float)):
         output += "," + str(counter) + ":metric:" + val
       else:
         output += "," + str(counter) + ":label:" + val
     if output == "":
       raise Exception("No values to format")
     return output[1:]
 
   def data_as_csv(self):
     vals = self.model_dump()
     vals.pop('url')
-    if "timestamp" in vals and vals["timestamp"] is not None and isinstance(vals["timestamp"], datetime):
-      vals['timestamp'] = strigify_datetime(vals['timestamp'])
-    else:
-      if "timestamp" in vals:
-        vals.pop('timestamp')
+    vals['timestamp'] = strigify_datetime(vals['timestamp'])
     output = ""
     for val in vals.values():
-      
       output += "," + str(val)
     if output == "":
       raise Exception("No values to format")
     return output[1:]
 
   def post(self):
     headers = {
```

