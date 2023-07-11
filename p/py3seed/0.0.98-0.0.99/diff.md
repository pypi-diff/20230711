# Comparing `tmp/py3seed-0.0.98.tar.gz` & `tmp/py3seed-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.0.98.tar", last modified: Wed May 11 02:55:21 2022, max compression
+gzip compressed data, was "py3seed-0.0.99.tar", last modified: Wed May 11 04:06:54 2022, max compression
```

## Comparing `py3seed-0.0.98.tar` & `py3seed-0.0.99.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 02:55:21.898618 py3seed-0.0.98/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.0.98/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 02:55:21.898762 py3seed-0.0.98/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.0.98/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.0.98/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      932 2022-05-11 02:55:21.899604 py3seed-0.0.98/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      257 2021-12-04 07:21:56.000000 py3seed-0.0.98/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 02:55:21.877043 py3seed-0.0.98/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 02:55:21.894807 py3seed-0.0.98/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      609 2022-05-06 09:20:10.000000 py3seed-0.0.98/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1646 2022-05-06 09:20:10.000000 py3seed-0.0.98/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.0.98/src/py3seed/admin.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 02:55:21.898094 py3seed-0.0.98/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.0.98/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    12356 2022-05-11 02:36:42.000000 py3seed-0.0.98/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      665 2021-09-15 09:23:34.000000 py3seed-0.0.98/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.0.98/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    39377 2022-05-10 01:49:39.000000 py3seed-0.0.98/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    23006 2022-01-14 03:15:02.000000 py3seed-0.0.98/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6008 2022-05-06 14:11:36.000000 py3seed-0.0.98/src/py3seed/utils.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 02:55:21.896973 py3seed-0.0.98/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      503 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       66 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2022-05-11 02:55:21.000000 py3seed-0.0.98/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.551836 py3seed-0.0.99/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.0.99/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 04:06:54.551971 py3seed-0.0.99/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.0.99/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.0.99/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      932 2022-05-11 04:06:54.552575 py3seed-0.0.99/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      257 2021-12-04 07:21:56.000000 py3seed-0.0.99/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.536575 py3seed-0.0.99/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.547448 py3seed-0.0.99/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      609 2022-05-06 09:20:10.000000 py3seed-0.0.99/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1646 2022-05-06 09:20:10.000000 py3seed-0.0.99/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.0.99/src/py3seed/admin.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.551156 py3seed-0.0.99/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.0.99/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    12399 2022-05-11 03:45:53.000000 py3seed-0.0.99/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      665 2021-09-15 09:23:34.000000 py3seed-0.0.99/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.0.99/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    39377 2022-05-10 01:49:39.000000 py3seed-0.0.99/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    23006 2022-01-14 03:15:02.000000 py3seed-0.0.99/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6008 2022-05-06 14:11:36.000000 py3seed-0.0.99/src/py3seed/utils.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.550168 py3seed-0.0.99/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      503 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       66 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/top_level.txt
```

### Comparing `py3seed-0.0.98/LICENSE` & `py3seed-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/PKG-INFO` & `py3seed-0.0.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.0.98/setup.cfg` & `py3seed-0.0.99/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.0.98
+version = 0.0.99
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.0.98/src/py3seed/__init__.py` & `py3seed-0.0.99/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/__main__.py` & `py3seed-0.0.99/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/admin.py` & `py3seed-0.0.99/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/commands/gen.py` & `py3seed-0.0.99/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,33 +74,36 @@
     env.filters['urlquote'] = urlquote
 
     def update_query(**new_values):
         """ Update query. """
         args = request.args.copy()
         for key, value in new_values.items():
             args[key] = value
-        return '{}?{}'.format(request.path, url_encode(args))
+        return url_encode(args)
 
     def new_model(class_name):
         """ New a model by class name. """
         klass = globals()[class_name]
         return klass()
 
-    def guess_field(columns, matcher):
+    def guess_field(fields, matcher):
         """ Get the first matching field from columns.
 
-        :param columns - list of field name
+        :param fields - list of field name
         :param matcher - name|title|\w+_name
         """
         matcher = re.compile(matcher if matcher.startswith('(') else f'({matcher})')
-        for c in columns:
-            if matcher.match(c):
-                return c
+        if isinstance(fields, dict):
+            fields = fields.keys()
+        #
+        for f in fields:
+            if matcher.match(f):
+                return f
         # If no matching, return first column
-        return columns[0]
+        return None
 
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
     env.globals['guess_field'] = guess_field
     #
     return env
```

### Comparing `py3seed-0.0.98/src/py3seed/error.py` & `py3seed-0.0.99/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/log.py` & `py3seed-0.0.99/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/model.py` & `py3seed-0.0.99/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/mongosupport.py` & `py3seed-0.0.99/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed/utils.py` & `py3seed-0.0.99/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.98/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.0.99/src/py3seed.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

