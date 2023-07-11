# Comparing `tmp/py-helper-mod-0.0.36.tar.gz` & `tmp/py-helper-mod-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.36.tar", last modified: Tue Jul 11 15:23:22 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.37.tar", last modified: Tue Jul 11 19:38:55 2023, max compression
```

## Comparing `py-helper-mod-0.0.36.tar` & `py-helper-mod-0.0.37.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89038 2023-07-11 15:22:01.000000 py-helper-mod-0.0.36/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.36/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89044 2023-07-11 19:38:03.000000 py-helper-mod-0.0.37/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 19:38:55.000000 py-helper-mod-0.0.37/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.37/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 19:38:55.426773 py-helper-mod-0.0.37/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.37/setup.py
```

### Comparing `py-helper-mod-0.0.36/LICENSE` & `py-helper-mod-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.36/PKG-INFO` & `py-helper-mod-0.0.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.36
+Version: 0.0.37
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.36/py_helper.py` & `py-helper-mod-0.0.37/py_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # The Usual Suspects
 # import keyser_soze
-import os, sys, io
+import os, sys, io, platform
 import shutil, subprocess, getpass
 import random
 import math
 
 # Reg Exprs... I have the POWER!!!!!!!!!
 import re
 
@@ -1181,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,35)
+VERSION=(0,0,36)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1318,15 +1318,15 @@
 	buffer = msg
 
 	if timestamp: prefix = datetime.now()
 
 	if includeCaller:
 		module = callerframe.f_code.co_filename
 		line = callerframe.f_lineno
-		host = os.uname().nodename
+		host = platform.node()
 
 		caller_str = f"{host}[{module}({line})]"
 
 		buffer = f"{buffer} {caller_str}"
 
 	if prefix != None:
 		buffer = f"{prefix} - {msg}"
```

### Comparing `py-helper-mod-0.0.36/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.37/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.36
+Version: 0.0.37
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.36/setup.cfg` & `py-helper-mod-0.0.37/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.36
+version = 0.0.37
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

