# Comparing `tmp/bb_dirtree-0.2.5.tar.gz` & `tmp/bb_dirtree-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.2.5.tar", max compression
+gzip compressed data, was "bb_dirtree-0.2.6.tar", max compression
```

## Comparing `bb_dirtree-0.2.5.tar` & `bb_dirtree-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.5/LICENSE
--rw-r--r--   0        0        0     4014 2023-07-11 03:32:12.417191 bb_dirtree-0.2.5/README.md
--rw-r--r--   0        0        0       77 2023-07-11 03:31:23.937190 bb_dirtree-0.2.5/bbdirtree/.__init__.py.kate-swp
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.5/bbdirtree/COLORS.py
--rw-r--r--   0        0        0     3419 2023-07-10 19:51:24.590003 bb_dirtree-0.2.5/bbdirtree/__init__.py
--rw-r--r--   0        0        0    18143 2023-07-11 03:31:14.493857 bb_dirtree-0.2.5/bbdirtree/__main__.py
--rw-r--r--   0        0        0      554 2023-07-11 03:31:33.620524 bb_dirtree-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 bb_dirtree-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4014 2023-07-11 03:37:28.013864 bb_dirtree-0.2.6/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.6/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0     3419 2023-07-11 03:37:24.467197 bb_dirtree-0.2.6/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    18137 2023-07-11 03:37:09.593863 bb_dirtree-0.2.6/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      554 2023-07-11 03:37:26.383864 bb_dirtree-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 bb_dirtree-0.2.6/PKG-INFO
```

### Comparing `bb_dirtree-0.2.5/LICENSE` & `bb_dirtree-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.5/README.md` & `bb_dirtree-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -142,10 +142,10 @@
 - added git project titles to output
     - searches for .SRCINFO file
 
 #### v0.2.4 - 7-10-2023
 
 - fixed typo in __main__
 
-#### v0.2.5 - 7-10-2023
+#### v0.2.6 - 7-10-2023
 
 - bugfixes
```

### Comparing `bb_dirtree-0.2.5/bbdirtree/COLORS.py` & `bb_dirtree-0.2.6/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.5/bbdirtree/__init__.py` & `bb_dirtree-0.2.6/bbdirtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.4'
+__version__ = '0.2.6'
 
 __doc__="""
 Create a nice looking directory tree
 
 Installation:
 =============
```

### Comparing `bb_dirtree-0.2.5/bbdirtree/__main__.py` & `bb_dirtree-0.2.6/bbdirtree/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,8 +509,8 @@
         print(x.list_gui())
     else:
         print(x.list_tty())
 
     return 0
 
 if __name__ == "__main__":
-    sys.exit( exec(main()) )
+    sys.exit( main() )
```

### Comparing `bb_dirtree-0.2.5/pyproject.toml` & `bb_dirtree-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.2.5"
+version = "0.2.6"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.2.5/PKG-INFO` & `bb_dirtree-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.2.5
+Version: 0.2.6
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -158,11 +158,11 @@
 - added git project titles to output
     - searches for .SRCINFO file
 
 #### v0.2.4 - 7-10-2023
 
 - fixed typo in __main__
 
-#### v0.2.5 - 7-10-2023
+#### v0.2.6 - 7-10-2023
 
 - bugfixes
```

