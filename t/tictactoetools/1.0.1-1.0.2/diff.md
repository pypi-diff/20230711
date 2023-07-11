# Comparing `tmp/tictactoetools-1.0.1.tar.gz` & `tmp/tictactoetools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-1.0.1.tar", last modified: Tue Jul 11 19:11:35 2023, max compression
+gzip compressed data, was "tictactoetools-1.0.2.tar", last modified: Tue Jul 11 19:53:03 2023, max compression
```

## Comparing `tictactoetools-1.0.1.tar` & `tictactoetools-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:11:35.469934 tictactoetools-1.0.1/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.1/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 19:11:35.469228 tictactoetools-1.0.1/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1338 2023-07-11 18:55:13.000000 tictactoetools-1.0.1/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 19:11:35.470139 tictactoetools-1.0.1/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      500 2023-07-11 19:11:15.000000 tictactoetools-1.0.1/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:11:35.465021 tictactoetools-1.0.1/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.1/tictactoetools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.1/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9312 2023-07-11 19:11:15.000000 tictactoetools-1.0.1/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:11:35.468300 tictactoetools-1.0.1/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 19:11:35.000000 tictactoetools-1.0.1/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      274 2023-07-11 19:11:35.000000 tictactoetools-1.0.1/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 19:11:35.000000 tictactoetools-1.0.1/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 19:11:35.000000 tictactoetools-1.0.1/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:53:03.230285 tictactoetools-1.0.2/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.2/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 19:53:03.229768 tictactoetools-1.0.2/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1338 2023-07-11 18:55:13.000000 tictactoetools-1.0.2/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 19:53:03.230422 tictactoetools-1.0.2/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      519 2023-07-11 19:52:35.000000 tictactoetools-1.0.2/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:53:03.225483 tictactoetools-1.0.2/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.2/tictactoetools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.2/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)     9366 2023-07-11 19:52:35.000000 tictactoetools-1.0.2/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 19:53:03.228923 tictactoetools-1.0.2/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 19:53:03.000000 tictactoetools-1.0.2/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      274 2023-07-11 19:53:03.000000 tictactoetools-1.0.2/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 19:53:03.000000 tictactoetools-1.0.2/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 19:53:03.000000 tictactoetools-1.0.2/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-1.0.1/LICENSE` & `tictactoetools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.1/PKG-INFO` & `tictactoetools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tictactoetools-1.0.1/README.md` & `tictactoetools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.1/tictactoetools/tictactoetools.py` & `tictactoetools-1.0.2/tictactoetools/tictactoetools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from datetime import datetime
 from .tictac_exceptions import FullBoardError
 from dataclasses import dataclass
 import os
 
 __package_dir = os.path.dirname(os.path.abspath(__file__))
 __db_path = os.path.join(__package_dir, "tic_tac_toe.db")
+print(__package_dir)
+print(__db_path)
+print(__file__)
 
 
 class Board:
     __BLANK_SPACE = " "
 
     def __init__(self, size: int = 3, num_consecutive_to_win: int = None) -> None:
         if size <= 0 or num_consecutive_to_win and num_consecutive_to_win <= 0:
```

### Comparing `tictactoetools-1.0.1/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-1.0.2/tictactoetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

