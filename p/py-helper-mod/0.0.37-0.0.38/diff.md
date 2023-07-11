# Comparing `tmp/py-helper-mod-0.0.37.tar.gz` & `tmp/py-helper-mod-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.37.tar", last modified: Tue Jul 11 19:38:55 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.38.tar", last modified: Tue Jul 11 19:52:54 2023, max compression
```

## Comparing `py-helper-mod-0.0.37.tar` & `py-helper-mod-0.0.38.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89044 2023-07-11 19:38:03.000000 py-helper-mod-0.0.37/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.37/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89040 2023-07-11 19:52:17.000000 py-helper-mod-0.0.38/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 19:52:54.000000 py-helper-mod-0.0.38/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.38/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 19:52:54.730598 py-helper-mod-0.0.38/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.38/setup.py
```

### Comparing `py-helper-mod-0.0.37/LICENSE` & `py-helper-mod-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.37/PKG-INFO` & `py-helper-mod-0.0.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.37
+Version: 0.0.38
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.37/py_helper.py` & `py-helper-mod-0.0.38/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,36)
+VERSION=(0,0,37)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1483,15 +1483,15 @@
 			return
 
 		if callerframe == None:
 			callerframe = inspect.currentframe().f_back
 
 		module = callerframe.f_code.co_filename
 		line = callerframe.f_lineno
-		host = os.uname().nodename
+		host = platform.node()
 
 		caller_str = f"{host}[{module}({line})]"
 
 		if timestamp:
 			prefix = f"{prefix} {datetime.now()}"
 
 		if delta != None:
```

### Comparing `py-helper-mod-0.0.37/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.38/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.37
+Version: 0.0.38
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.37/setup.cfg` & `py-helper-mod-0.0.38/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.37
+version = 0.0.38
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

