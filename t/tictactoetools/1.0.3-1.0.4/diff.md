# Comparing `tmp/tictactoetools-1.0.3.tar.gz` & `tmp/tictactoetools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-1.0.3.tar", last modified: Tue Jul 11 20:25:45 2023, max compression
+gzip compressed data, was "tictactoetools-1.0.4.tar", last modified: Tue Jul 11 20:43:26 2023, max compression
```

## Comparing `tictactoetools-1.0.3.tar` & `tictactoetools-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:25:45.870505 tictactoetools-1.0.3/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.3/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 20:25:45.869628 tictactoetools-1.0.3/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1338 2023-07-11 18:55:13.000000 tictactoetools-1.0.3/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 20:25:45.870654 tictactoetools-1.0.3/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      587 2023-07-11 20:25:04.000000 tictactoetools-1.0.3/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:25:45.859587 tictactoetools-1.0.3/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.3/tictactoetools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.3/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9300 2023-07-11 20:21:32.000000 tictactoetools-1.0.3/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:25:45.867926 tictactoetools-1.0.3/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1719 2023-07-11 20:25:45.000000 tictactoetools-1.0.3/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      274 2023-07-11 20:25:45.000000 tictactoetools-1.0.3/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 20:25:45.000000 tictactoetools-1.0.3/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 20:25:45.000000 tictactoetools-1.0.3/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.690092 tictactoetools-1.0.4/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.4/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 20:43:26.688947 tictactoetools-1.0.4/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1341 2023-07-11 20:31:43.000000 tictactoetools-1.0.4/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 20:43:26.690331 tictactoetools-1.0.4/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      593 2023-07-11 20:43:24.000000 tictactoetools-1.0.4/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.676184 tictactoetools-1.0.4/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.4/tictactoetools/__init__.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.685492 tictactoetools-1.0.4/tictactoetools/data/
+-rw-r--r--   0 simon      (502) staff       (20)    24576 2023-07-11 19:12:05.000000 tictactoetools-1.0.4/tictactoetools/data/tic_tac_toe.db
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.4/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)     9303 2023-07-11 20:36:27.000000 tictactoetools-1.0.4/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.682509 tictactoetools-1.0.4/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      309 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-1.0.3/LICENSE` & `tictactoetools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.3/PKG-INFO` & `tictactoetools-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 and storing the data of matches in a database.
 
 # Installation
 
 To install the tictactoetools package, you can use the following command:
 
 ```
-pip install tictactools
+pip install tictactoetools
 ```
 
 # Usage
 
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
```

### Comparing `tictactoetools-1.0.3/README.md` & `tictactoetools-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and storing the data of matches in a database.
 
 # Installation
 
 To install the tictactoetools package, you can use the following command:
 
 ```
-pip install tictactools
+pip install tictactoetools
 ```
 
 # Usage
 
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
```

### Comparing `tictactoetools-1.0.3/tictactoetools/tictactoetools.py` & `tictactoetools-1.0.4/tictactoetools/tictactoetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sqlite3
 from datetime import datetime
 from .tictac_exceptions import FullBoardError
 from dataclasses import dataclass
 import os
 
 __package_dir = os.path.dirname(__file__)
-__db_path = os.path.join(__package_dir, "data/tic_tac_toe.db")
+__db_path = os.path.join(__package_dir, "data", "tic_tac_toe.db")
 
 
 class Board:
     __BLANK_SPACE = " "
 
     def __init__(self, size: int = 3, num_consecutive_to_win: int = None) -> None:
         if size <= 0 or num_consecutive_to_win and num_consecutive_to_win <= 0:
```

### Comparing `tictactoetools-1.0.3/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-1.0.4/tictactoetools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 and storing the data of matches in a database.
 
 # Installation
 
 To install the tictactoetools package, you can use the following command:
 
 ```
-pip install tictactools
+pip install tictactoetools
 ```
 
 # Usage
 
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
```

