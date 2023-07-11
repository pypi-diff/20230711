# Comparing `tmp/strinpy-0.0.2.tar.gz` & `tmp/strinpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strinpy-0.0.2.tar", last modified: Tue Jun 27 11:07:42 2023, max compression
+gzip compressed data, was "strinpy-0.0.3.tar", last modified: Tue Jul 11 12:51:13 2023, max compression
```

## Comparing `strinpy-0.0.2.tar` & `strinpy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.402502 strinpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 11:07:29.000000 strinpy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 11:07:42.402502 strinpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-27 11:07:29.000000 strinpy-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:07:42.402502 strinpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 11:07:29.000000 strinpy-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.398502 strinpy-0.0.2/strinpy/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 11:07:29.000000 strinpy-0.0.2/strinpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-27 11:07:29.000000 strinpy-0.0.2/strinpy/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.402502 strinpy-0.0.2/strinpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 12:51:05.000000 strinpy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 12:51:13.594259 strinpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 12:51:05.000000 strinpy-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:51:13.594259 strinpy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 12:51:05.000000 strinpy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/strinpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 12:51:05.000000 strinpy-0.0.3/strinpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-11 12:51:05.000000 strinpy-0.0.3/strinpy/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/strinpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/top_level.txt
```

### Comparing `strinpy-0.0.2/LICENSE` & `strinpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.2/PKG-INFO` & `strinpy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
```

### Comparing `strinpy-0.0.2/README.rst` & `strinpy-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.2/setup.py` & `strinpy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 author = 'am230'
 name = 'strinpy'
 py_modules = [name]
 
 setup(
     name=name,
-    version="0.0.2",
+    version="0.0.3",
     keywords=["string"],
     description="React like string builder",
     long_description=long_description,
     license="MIT Licence",
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     url=f"https://github.com/{author}/{name}",
```

### Comparing `strinpy-0.0.2/strinpy/builder.py` & `strinpy-0.0.3/strinpy/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,32 @@
 import asyncio
 Value = _t.Union[str, int, float, bool, None, _t.List, _t.Tuple, _t.List['Value']]
 
 EMPTY_TUPLE = tuple()
 
 V = _t.TypeVar('V', bound=Value)
 
+
 class Formatter:
     def format_value(self, value: _t.Any) -> _t.Tuple[str]:
-        if value in (False, None):
-            return EMPTY_TUPLE
-        if isinstance(value, list):
-            return tuple(itertools.chain.from_iterable(map(self.format_value, value)))
-        elif callable(value):
-            return value()
         return (str(value),)
 
+
 class Builder(_t.Generic[V]):
     def __init__(self, formatter: Formatter = Formatter()) -> None:
         self.formatter = formatter
 
     def format_value(self, value: V | Value) -> _t.Tuple[str]:
-        if value == False:
+        if value in (False, None):
             return EMPTY_TUPLE
         if isinstance(value, list):
             return tuple(itertools.chain.from_iterable(map(self.format_value, value)))
         elif callable(value):
             return value()
-        return (str(value),)
+        return self.formatter.format_value(value)
 
     def build(self, value: V) -> str:
         parts = self.format_value(value)
         return ''.join(parts)
 
 
 class AsyncBuilder(Builder[V]):
```

### Comparing `strinpy-0.0.2/strinpy.egg-info/PKG-INFO` & `strinpy-0.0.3/strinpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
```

