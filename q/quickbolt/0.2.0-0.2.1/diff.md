# Comparing `tmp/quickbolt-0.2.0.tar.gz` & `tmp/quickbolt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.2.0.tar", max compression
+gzip compressed data, was "quickbolt-0.2.1.tar", max compression
```

## Comparing `quickbolt-0.2.0.tar` & `quickbolt-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.2.0/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.2.0/README.md
--rw-r--r--   0        0        0     1238 2023-07-10 03:58:55.439034 quickbolt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.2.0/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.2.0/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    11377 2023-07-07 23:59:06.071578 quickbolt-0.2.0/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.2.0/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0    10215 2023-07-10 03:29:24.475286 quickbolt-0.2.0/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10430 2023-07-10 03:29:24.475556 quickbolt-0.2.0/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.2.0/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.2.0/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.2.0/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.2.0/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.2.0/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     8518 2023-07-10 03:29:24.475798 quickbolt-0.2.0/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.2.0/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.2.0/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.2.0/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     2802 2023-07-07 23:59:06.071757 quickbolt-0.2.0/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.2.0/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.2.0/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.2.0/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.2.1/README.md
+-rw-r--r--   0        0        0     1238 2023-07-11 14:12:04.234128 quickbolt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.2.1/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.2.1/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    11377 2023-07-07 23:59:06.071578 quickbolt-0.2.1/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.2.1/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0    10215 2023-07-10 03:29:24.475286 quickbolt-0.2.1/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10430 2023-07-10 03:29:24.475556 quickbolt-0.2.1/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.2.1/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.2.1/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.2.1/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.2.1/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.2.1/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     8518 2023-07-10 03:29:24.475798 quickbolt-0.2.1/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.2.1/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     4412 2023-07-11 13:57:47.205851 quickbolt-0.2.1/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.2.1/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     2802 2023-07-07 23:59:06.071757 quickbolt-0.2.1/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.2.1/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.2.1/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.2.1/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.2.1/PKG-INFO
```

### Comparing `quickbolt-0.2.0/LICENSE` & `quickbolt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/README.md` & `quickbolt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/pyproject.toml` & `quickbolt-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.2.0"
+version = "0.2.1"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.2.0/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.2.1/quickbolt/batch_generation/batch_generation.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/clients/aio_requests.py` & `quickbolt-0.2.1/quickbolt/clients/aio_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/clients/httpx_requests.py` & `quickbolt-0.2.1/quickbolt/clients/httpx_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/logging/async_logger.py` & `quickbolt-0.2.1/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.2.1/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/reporting/response_csv.py` & `quickbolt-0.2.1/quickbolt/reporting/response_csv.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/utils/dictionary.py` & `quickbolt-0.2.1/quickbolt/utils/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,47 +42,48 @@
 
     Returns:
         unflattened_dict: The unflattened dict.
     """
 
     def assign(keys, value, d):
         key = keys.pop(0)
+
+        if key.isdigit():
+            key = int(key)
+            if isinstance(d, dict):
+                d = [d]
+            while len(d) <= key:
+                d.append(None)
+        else:
+            if isinstance(d, list):
+                d[-1] = {}
+
         if len(keys) == 0:
-            if key.isdigit():
-                while len(d) <= int(key):
-                    d.append(None)
-                d[int(key)] = value
-            else:
-                d[key] = value
+            d[key] = value
         else:
-            if key.isdigit():
-                if int(key) < len(d):
-                    assign(keys, value, d[int(key)])
-                else:
-                    while len(d) < int(key):
-                        d.append({})
-                    d.append({})
-                    assign(keys, value, d[int(key)])
+            if isinstance(d, list):
+                d[key] = assign(
+                    keys, value, d[key] if key < len(d) and d[key] is not None else {}
+                )
             else:
-                if key in d.keys():
-                    assign(keys, value, d[key])
-                else:
-                    d[key] = [{}] if keys[0].isdigit() else {}
-                    assign(keys, value, d[key])
+                d[key] = assign(
+                    keys, value, d.get(key, [{}] if keys[0].isdigit() else {})
+                )
+
+        return d
 
     if len(flat_dict) == 1 and "" in flat_dict:
         return flat_dict[""]
 
-    unflattened_dict = {}
-
+    unflattened = {}
     for flat_key, value in flat_dict.items():
         keys = flat_key.split(".")
-        assign(keys, value, unflattened_dict)
+        unflattened = assign(keys, value, unflattened)
 
-    return unflattened_dict
+    return unflattened
 
 
 def compare_dictionaries(
     d1: dict,
     d2: dict,
     skipped_keys: None | list = None,
     exclusive_keys: None | list = None,
```

### Comparing `quickbolt-0.2.0/quickbolt/utils/directory.py` & `quickbolt-0.2.1/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/utils/json.py` & `quickbolt-0.2.1/quickbolt/utils/json.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/quickbolt/validations/validations.py` & `quickbolt-0.2.1/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.2.0/PKG-INFO` & `quickbolt-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.2.0
+Version: 0.2.1
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
```

