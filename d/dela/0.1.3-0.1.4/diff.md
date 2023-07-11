# Comparing `tmp/dela-0.1.3.tar.gz` & `tmp/dela-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.1.3.tar", max compression
+gzip compressed data, was "dela-0.1.4.tar", max compression
```

## Comparing `dela-0.1.3.tar` & `dela-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1599 2023-07-11 05:47:54.958781 dela-0.1.3/README.md
--rw-r--r--   0        0        0      267 2023-07-11 05:47:54.958781 dela-0.1.3/dela/FileReader.py
--rw-r--r--   0        0        0     3729 2023-07-11 05:47:54.958781 dela-0.1.3/dela/ListCommand.py
--rw-r--r--   0        0        0     1295 2023-07-11 05:47:54.958781 dela-0.1.3/dela/Todo.py
--rw-r--r--   0        0        0      580 2023-07-11 05:47:54.958781 dela-0.1.3/dela/TodoPresentation.py
--rw-r--r--   0        0        0        0 2023-07-11 05:47:54.958781 dela-0.1.3/dela/__init__.py
--rw-r--r--   0        0        0     2030 2023-07-11 05:47:54.958781 dela-0.1.3/dela/__main__.py
--rw-r--r--   0        0        0      123 2023-07-11 05:47:54.958781 dela-0.1.3/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-11 05:47:54.966781 dela-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 dela-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1599 2023-07-11 06:05:23.840877 dela-0.1.4/README.md
+-rw-r--r--   0        0        0      267 2023-07-11 06:05:23.840877 dela-0.1.4/dela/FileReader.py
+-rw-r--r--   0        0        0     3731 2023-07-11 06:05:23.840877 dela-0.1.4/dela/ListCommand.py
+-rw-r--r--   0        0        0     1295 2023-07-11 06:05:23.840877 dela-0.1.4/dela/Todo.py
+-rw-r--r--   0        0        0      580 2023-07-11 06:05:23.840877 dela-0.1.4/dela/TodoPresentation.py
+-rw-r--r--   0        0        0        0 2023-07-11 06:05:23.840877 dela-0.1.4/dela/__init__.py
+-rw-r--r--   0        0        0     2030 2023-07-11 06:05:23.840877 dela-0.1.4/dela/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-11 06:05:23.840877 dela-0.1.4/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-11 06:05:23.848877 dela-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 dela-0.1.4/PKG-INFO
```

### Comparing `dela-0.1.3/README.md` & `dela-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dela-0.1.3/dela/ListCommand.py` & `dela-0.1.4/dela/ListCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 if i.status
                 not in [
                     *Todo.STATUSES_DONE,
                     *Todo.STATUSES_ARCHIVED,
                     *Todo.STATUSES_CLOSED,
                     *Todo.STATUSES_SOMEDAY,
                 ] 
-                and (not bool(i.date) or int(i.date) < YYYYmmDD)
+                and (not bool(i.date) or int(i.date) <= YYYYmmDD)
             ]
 
         if self.config.only_someday:
             result = [i for i in result if i.status in Todo.STATUSES_SOMEDAY]
 
         if self.config.only_done:
             result = [i for i in result if i.status not in Todo.STATUSES_DONE]
@@ -91,15 +91,15 @@
 
         if self.config.filter_by_tags:
             result = [
                 i for i in result if bool(set(i.tags) & set(self.config.filter_by_tags))
             ]
 
         if self.config.only_today:
-            result = [i for i in result if bool(i.date) and int(i.date) < YYYYmmDD]
+            result = [i for i in result if bool(i.date) and int(i.date) <= YYYYmmDD]
 
         return result
 
     def sort(self, todos):
         result = todos
 
         if self.config.sort_by:
```

### Comparing `dela-0.1.3/dela/Todo.py` & `dela-0.1.4/dela/Todo.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.3/dela/TodoPresentation.py` & `dela-0.1.4/dela/TodoPresentation.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.3/dela/__main__.py` & `dela-0.1.4/dela/__main__.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.3/PKG-INFO` & `dela-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dela
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: 'Anton Shuvalov'
 Author-email: anton@shuvalov.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

