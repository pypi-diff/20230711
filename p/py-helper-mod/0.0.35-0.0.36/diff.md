# Comparing `tmp/py-helper-mod-0.0.35.tar.gz` & `tmp/py-helper-mod-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.35.tar", last modified: Mon Jun 26 22:26:58 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.36.tar", last modified: Tue Jul 11 15:23:22 2023, max compression
```

## Comparing `py-helper-mod-0.0.35.tar` & `py-helper-mod-0.0.36.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    88590 2023-06-26 22:19:23.000000 py-helper-mod-0.0.35/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-06-26 22:26:58.592314 py-helper-mod-0.0.35/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.35/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89038 2023-07-11 15:22:01.000000 py-helper-mod-0.0.36/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-11 15:23:22.000000 py-helper-mod-0.0.36/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.36/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-11 15:23:22.024596 py-helper-mod-0.0.36/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.36/setup.py
```

### Comparing `py-helper-mod-0.0.35/LICENSE` & `py-helper-mod-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.35/PKG-INFO` & `py-helper-mod-0.0.36/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.35
+Version: 0.0.36
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.35/py_helper.py` & `py-helper-mod-0.0.36/py_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1181,26 +1181,26 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,34)
+VERSION=(0,0,35)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
 
 # Debug/Breakpoint Flags
-DebugEnabled = None
-DebugLabelExists = False
+DebugEnabled = None		# Dictionary of labels, not enabled is None
+DebugLabelExists = True		# If true, NONE (no label) and non-explicitly defined labels are all enabled by default
 
 # Signals Module is being used in Cmd Line Mode
 __CmdLineMode__ = False
 
 # Notes:
 # DebugMode puts the module in DebugMode, i.e. it activates DbgMsg() to output
 # 	when DebugMode is false, DbgMsg does nothing.
@@ -1393,42 +1393,55 @@
 	SetDebugLabel(dbglabel,True)
 
 def DisableDebugLabel(dbglabel):
 	"""Disable Debug Label"""
 
 	SetDebugLabel(dbglabel,False)
 
+def DebugLabelBehavior(value=None):
+	"""Set the default debug label behavior"""
+
+	global DebugLabelExists
+
+	if not value is None:
+		DebugLabelExists = value
+
+	return DebugLabelExists
+
 def LoadDebugEnableFile(filename):
 	"""Load Debug Enablement Data File"""
 
-	global DebugEnabled
+	global DebugEnabled, DebugLabelExists
 
 	if DebugEnabled is not None:
 		del DebugEnabled
 
 	DebugEnabled = None
 
 	if os.path.exists(filename):
 		DebugEnabled = dict()
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
-				DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","Yes","yes","y","Y" ] else False
+				if row[0] == "default":
+					DebugLabelExists = True if row[1] in [ "True","true","TRUE","1","yes","Yes","y","Y" ] else False
+				else:
+					DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","1","Yes","yes","y","Y" ] else False
 
 def IsDebugLabelEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugEnabled, DebugLabelExists
 
-	enabled = True if not DebugLabelExists else False
+	enabled = DebugLabelExists
 
 	if DebugEnabled is not None and dbglabel is not None:
-		if dbglabel in DebugEnabled and test:
+		if dbglabel in DebugEnabled:
 			enabled = DebugEnabled[dbglabel]
 
 	return enabled
 
 def Breakpoint(dbglabel,test_flag=True):
 	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
```

### Comparing `py-helper-mod-0.0.35/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.36/py_helper_mod.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.35
+Version: 0.0.36
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.35/setup.cfg` & `py-helper-mod-0.0.36/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.35
+version = 0.0.36
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

