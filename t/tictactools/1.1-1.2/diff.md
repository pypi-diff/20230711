# Comparing `tmp/tictactools-1.1.tar.gz` & `tmp/tictactools-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactools-1.1.tar", last modified: Tue Jul 11 01:53:09 2023, max compression
+gzip compressed data, was "tictactools-1.2.tar", last modified: Tue Jul 11 02:37:31 2023, max compression
```

## Comparing `tictactools-1.1.tar` & `tictactools-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 01:53:09.876428 tictactools-1.1/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 01:01:40.000000 tictactools-1.1/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 01:53:09.875621 tictactools-1.1/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1321 2023-07-11 01:22:01.000000 tictactools-1.1/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 01:53:09.876640 tictactools-1.1/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      492 2023-07-11 01:52:15.000000 tictactools-1.1/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 01:53:09.871395 tictactools-1.1/tictactools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 00:11:34.000000 tictactools-1.1/tictactools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-08 16:01:12.000000 tictactools-1.1/tictactools/tictactoe_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9298 2023-07-11 00:32:19.000000 tictactools-1.1/tictactools/tictactools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 01:53:09.874874 tictactools-1.1/tictactools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 01:53:09.000000 tictactools-1.1/tictactools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      253 2023-07-11 01:53:09.000000 tictactools-1.1/tictactools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 01:53:09.000000 tictactools-1.1/tictactools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       12 2023-07-11 01:53:09.000000 tictactools-1.1/tictactools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.380905 tictactools-1.2/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 01:01:40.000000 tictactools-1.2/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:37:31.379794 tictactools-1.2/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1321 2023-07-11 01:22:01.000000 tictactools-1.2/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 02:37:31.381069 tictactools-1.2/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      492 2023-07-11 02:36:37.000000 tictactools-1.2/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.372867 tictactools-1.2/tictactools/
+-rw-r--r--   0 simon      (502) staff       (20)     1094 2023-07-11 02:36:03.000000 tictactools-1.2/tictactools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-08 16:01:12.000000 tictactools-1.2/tictactools/tictactoe_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)     9298 2023-07-11 02:27:56.000000 tictactools-1.2/tictactools/tictactools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 02:37:31.378924 tictactools-1.2/tictactools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1694 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      253 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       12 2023-07-11 02:37:31.000000 tictactools-1.2/tictactools.egg-info/top_level.txt
```

### Comparing `tictactools-1.1/LICENSE` & `tictactools-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactools-1.1/PKG-INFO` & `tictactools-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactools
-Version: 1.1
+Version: 1.2
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tictactools-1.1/README.md` & `tictactools-1.2/README.md`

 * *Files identical despite different names*

### Comparing `tictactools-1.1/tictactools/tictactools.py` & `tictactools-1.2/tictactools/tictactools.py`

 * *Files identical despite different names*

### Comparing `tictactools-1.1/tictactools.egg-info/PKG-INFO` & `tictactools-1.2/tictactools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactools
-Version: 1.1
+Version: 1.2
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

