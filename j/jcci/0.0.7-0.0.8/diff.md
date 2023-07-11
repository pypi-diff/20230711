# Comparing `tmp/jcci-0.0.7.tar.gz` & `tmp/jcci-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.7.tar", last modified: Mon Jul 10 09:35:38 2023, max compression
+gzip compressed data, was "jcci-0.0.8.tar", last modified: Tue Jul 11 02:09:53 2023, max compression
```

## Comparing `jcci-0.0.7.tar` & `jcci-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:35:38.235099 jcci-0.0.7/
--rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3029 2023-07-10 09:35:38.234095 jcci-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.7/README.md
--rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.7/README.pypi.md
--rw-rw-rw-   0        0        0      708 2023-07-10 09:35:18.000000 jcci-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 09:35:38.235099 jcci-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 09:35:38.219094 jcci-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 09:35:38.227096 jcci-0.0.7/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.7/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.7/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    42792 2023-07-10 09:35:09.000000 jcci-0.0.7/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:35:38.232098 jcci-0.0.7/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     3029 2023-07-10 09:35:38.000000 jcci-0.0.7/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-10 09:35:38.000000 jcci-0.0.7/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:35:38.000000 jcci-0.0.7/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-10 09:35:38.000000 jcci-0.0.7/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 09:35:38.000000 jcci-0.0.7/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.699941 jcci-0.0.8/
+-rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3031 2023-07-11 02:09:53.698940 jcci-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.8/README.pypi.md
+-rw-rw-rw-   0        0        0      710 2023-07-11 02:09:44.000000 jcci-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 02:09:53.699941 jcci-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.679939 jcci-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.690941 jcci-0.0.8/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.8/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.8/src/jcci/java_analyzer.py
+-rw-rw-rw-   0        0        0    43818 2023-07-11 02:04:09.000000 jcci-0.0.8/src/jcci/jcci.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.696940 jcci-0.0.8/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0     3031 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/top_level.txt
```

### Comparing `jcci-0.0.7/LICENSE` & `jcci-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.0.7/PKG-INFO` & `jcci-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.7
+Version: 0.0.8
 Summary: Java code commit impact analyze in pure Python
-Author-email: Quan Li <441640312@qq.com>
+Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
```

### Comparing `jcci-0.0.7/README.md` & `jcci-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jcci-0.0.7/README.pypi.md` & `jcci-0.0.8/README.pypi.md`

 * *Files identical despite different names*

### Comparing `jcci-0.0.7/src/jcci/java_analyzer.py` & `jcci-0.0.8/src/jcci/java_analyzer.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.7/src/jcci/jcci.py` & `jcci-0.0.8/src/jcci/jcci.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     methods_list = []
     methods_name_list = [method.name for method in types.methods]
     for method_obj in types.methods:
         method_name = method_obj.name
         method_start_line = method_obj.position.line
         if method_obj.annotations:
             method_start_line = method_obj.annotations[0].position.line
-        method_end_line = _get_method_end_line(method_obj)
+        method_end_line = _get_method_end_line_new(method_obj)
         method_content = lines[method_start_line - 1: method_end_line]
         # method is api or not
         is_api = False
         api_path_list = []
         if is_controller:
             method_annotations = method_obj.annotations
             req_method_list = []
@@ -283,14 +283,43 @@
     part_class = type(part).__name__
     if part_class == 'MemberReference':
         return part.member
     elif part_class == 'Literal':
         return part.value
 
 
+def _get_method_end_line_new(method_obj):
+    method_end_line = method_obj.position.line
+    while True:
+        if isinstance(method_obj, list):
+            if None in method_obj:
+                method_obj.remove(None)
+            if len(method_obj) == 0:
+                break
+            length = len(method_obj)
+            for i in range(0, length):
+                temp = method_obj[length-1-i]
+                if temp is not None:
+                    method_obj = temp
+                    break
+            if method_obj is None:
+                break
+        if isinstance(method_obj, list):
+            continue
+        if hasattr(method_obj, 'position') \
+                and method_obj.position is not None \
+                and method_obj.position.line > method_end_line:
+            method_end_line = method_obj.position.line
+        if hasattr(method_obj, 'children'):
+            method_obj = method_obj.children
+        else:
+            break
+    return method_end_line
+
+
 def _get_method_end_line(method_obj):
     method_end_line = method_obj.position.line
     if method_obj.body is not None and len(method_obj.body) > 0:
         method_end_line = method_obj.body[-1].position.line
         method_body = method_obj.body[-1]
         while True:
             method_obj_dict = method_body.__dict__
@@ -543,15 +572,15 @@
 def _clean_occupy(occupy_path):
     if os.path.exists(occupy_path):
         os.remove(occupy_path)
 
 
 def _class_in_method(class_name, method):
     if method.contains_declarators is not None:
-        dcl_in_method = [d for d in method.contains_declarators if d.type == class_name]
+        dcl_in_method = [d for d in method.contains_declarators if d['type'] == class_name]
         if len(dcl_in_method) > 0:
             return True
     method_content = str(method.content)
     if class_name + ' ' in method_content \
             or '<' + class_name + '>' in method_content \
             or class_name + '.' in method_content:
         return True
```

### Comparing `jcci-0.0.7/src/jcci.egg-info/PKG-INFO` & `jcci-0.0.8/src/jcci.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.7
+Version: 0.0.8
 Summary: Java code commit impact analyze in pure Python
-Author-email: Quan Li <441640312@qq.com>
+Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
```

