# Comparing `tmp/tictactools-1.2.tar.gz` & `tmp/tictactools-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactools-1.2.tar", last modified: Tue Jul 11 02:37:31 2023, max compression
+gzip compressed data, was "tictactools-1.3.tar", last modified: Tue Jul 11 02:42:43 2023, max compression
```

## Comparing `tictactools-1.2.tar` & `tictactools-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.380905 tictactools-1.2/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 01:01:40.000000 tictactools-1.2/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:37:31.379794 tictactools-1.2/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1321 2023-07-11 01:22:01.000000 tictactools-1.2/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 02:37:31.381069 tictactools-1.2/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      492 2023-07-11 02:36:37.000000 tictactools-1.2/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.372867 tictactools-1.2/tictactools/
--rw-r--r--   0 simon      (502) staff       (20)     1094 2023-07-11 02:36:03.000000 tictactools-1.2/tictactools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-08 16:01:12.000000 tictactools-1.2/tictactools/tictactoe_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9298 2023-07-11 02:27:56.000000 tictactools-1.2/tictactools/tictactools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.378924 tictactools-1.2/tictactools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      253 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       12 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:42:43.138059 tictactools-1.3/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 01:01:40.000000 tictactools-1.3/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:42:43.137506 tictactools-1.3/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1321 2023-07-11 01:22:01.000000 tictactools-1.3/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 02:42:43.138229 tictactools-1.3/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      492 2023-07-11 02:42:10.000000 tictactools-1.3/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:42:43.132763 tictactools-1.3/tictactools/
+-rw-r--r--   0 simon      (502) staff       (20)     1104 2023-07-11 02:42:10.000000 tictactools-1.3/tictactools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-08 16:01:12.000000 tictactools-1.3/tictactools/tictactoe_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)     9298 2023-07-11 02:27:56.000000 tictactools-1.3/tictactools/tictactools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:42:43.136615 tictactools-1.3/tictactools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:42:43.000000 tictactools-1.3/tictactools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      253 2023-07-11 02:42:43.000000 tictactools-1.3/tictactools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 02:42:43.000000 tictactools-1.3/tictactools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       12 2023-07-11 02:42:43.000000 tictactools-1.3/tictactools.egg-info/top_level.txt
```

### Comparing `tictactools-1.2/LICENSE` & `tictactools-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactools-1.2/PKG-INFO` & `tictactools-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactools
-Version: 1.2
+Version: 1.3
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tictactools-1.2/README.md` & `tictactools-1.3/README.md`

 * *Files identical despite different names*

### Comparing `tictactools-1.2/tictactools/__init__.py` & `tictactools-1.3/tictactools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlite3
+import os
 
 __package_dir = os.path.dirname(__file__)
 __db_path = os.path.join(__package_dir, "tic_tac_toe.db")
 
 with sqlite3.connect(__db_path) as conn:
     conn.execute("""
     CREATE TABLE IF NOT EXISTS "matches" (
```

### Comparing `tictactools-1.2/tictactools/tictactools.py` & `tictactools-1.3/tictactools/tictactools.py`

 * *Files identical despite different names*

### Comparing `tictactools-1.2/tictactools.egg-info/PKG-INFO` & `tictactools-1.3/tictactools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactools
-Version: 1.2
+Version: 1.3
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

