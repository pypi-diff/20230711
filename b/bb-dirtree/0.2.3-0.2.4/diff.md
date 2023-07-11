# Comparing `tmp/bb_dirtree-0.2.3.tar.gz` & `tmp/bb_dirtree-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.2.3.tar", max compression
+gzip compressed data, was "bb_dirtree-0.2.4.tar", max compression
```

## Comparing `bb_dirtree-0.2.3.tar` & `bb_dirtree-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.3/LICENSE
--rw-r--r--   0        0        0     3926 2023-07-10 00:01:14.767139 bb_dirtree-0.2.3/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.3/bbdirtree/COLORS.py
--rw-r--r--   0        0        0     3419 2023-07-10 00:01:45.007139 bb_dirtree-0.2.3/bbdirtree/__init__.py
--rw-r--r--   0        0        0    18132 2023-07-10 00:04:24.760475 bb_dirtree-0.2.3/bbdirtree/__main__.py
--rw-r--r--   0        0        0      554 2023-07-10 00:01:51.297139 bb_dirtree-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 bb_dirtree-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3977 2023-07-10 19:52:24.020004 bb_dirtree-0.2.4/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.4/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0     3419 2023-07-10 19:51:24.590003 bb_dirtree-0.2.4/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    18134 2023-07-10 19:50:59.966669 bb_dirtree-0.2.4/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      554 2023-07-10 19:52:27.830004 bb_dirtree-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 bb_dirtree-0.2.4/PKG-INFO
```

### Comparing `bb_dirtree-0.2.3/LICENSE` & `bb_dirtree-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.3/README.md` & `bb_dirtree-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -137,7 +137,11 @@
 
 #### v0.2.3 - 7-9-2023
 
 - added python project titles to output
     - searches for pyproject.toml or setup.py
 - added git project titles to output
     - searches for .SRCINFO file
+
+#### v0.2.4 - 7-10-2023
+
+- fixed typo in __main__
```

### Comparing `bb_dirtree-0.2.3/bbdirtree/COLORS.py` & `bb_dirtree-0.2.4/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.3/bbdirtree/__init__.py` & `bb_dirtree-0.2.4/bbdirtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 __doc__="""
 Create a nice looking directory tree
 
 Installation:
 =============
```

### Comparing `bb_dirtree-0.2.3/bbdirtree/__main__.py` & `bb_dirtree-0.2.4/bbdirtree/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,8 +509,8 @@
         print(x.list_gui())
     else:
         print(x.list_tty())
 
     return 0
 
 if __name__ == "__main__":
-    sys.exit( exec(main) )
+    sys.exit( exec(main()) )
```

### Comparing `bb_dirtree-0.2.3/pyproject.toml` & `bb_dirtree-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.2.3"
+version = "0.2.4"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.2.3/PKG-INFO` & `bb_dirtree-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.2.3
+Version: 0.2.4
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -154,7 +154,11 @@
 #### v0.2.3 - 7-9-2023
 
 - added python project titles to output
     - searches for pyproject.toml or setup.py
 - added git project titles to output
     - searches for .SRCINFO file
 
+#### v0.2.4 - 7-10-2023
+
+- fixed typo in __main__
+
```

