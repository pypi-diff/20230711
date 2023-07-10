# Comparing `tmp/typetype-1.0.5.tar.gz` & `tmp/typetype-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.5.tar", last modified: Mon Jul 10 06:33:03 2023, max compression
+gzip compressed data, was "typetype-1.0.6.tar", last modified: Mon Jul 10 22:58:29 2023, max compression
```

## Comparing `typetype-1.0.5.tar` & `typetype-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:33:03.300985 typetype-1.0.5/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 06:33:03.300844 typetype-1.0.5/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.5/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 06:33:03.301035 typetype-1.0.5/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      651 2023-07-10 06:30:06.000000 typetype-1.0.5/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:33:03.295109 typetype-1.0.5/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.5/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7772 2023-07-10 06:29:48.000000 typetype-1.0.5/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:33:03.296877 typetype-1.0.5/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.5/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:33:03.298385 typetype-1.0.5/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.5/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:33:03.295995 typetype-1.0.5/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 06:33:03.000000 typetype-1.0.5/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      507 2023-07-10 06:33:03.000000 typetype-1.0.5/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 06:33:03.000000 typetype-1.0.5/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 06:33:03.000000 typetype-1.0.5/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 06:33:03.000000 typetype-1.0.5/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.839564 typetype-1.0.6/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.6/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 22:58:29.839438 typetype-1.0.6/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.6/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 22:58:29.839611 typetype-1.0.6/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      487 2023-07-10 22:56:21.000000 typetype-1.0.6/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.834201 typetype-1.0.6/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.6/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8008 2023-07-10 22:56:38.000000 typetype-1.0.6/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.835687 typetype-1.0.6/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.6/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.837079 typetype-1.0.6/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 22:57:55.000000 typetype-1.0.6/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.834941 typetype-1.0.6/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.5/README.md` & `typetype-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/ahmetsgame.py` & `typetype-1.0.6/typetype/ahmetsgame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from typetype.functions.game_selection import get_game, get_diff, get_mode
-from typetype.functions.setup_results import setup, end_screen
-from typetype.functions.refresh_update import refresh_screen, update_status, find_start_word
+try:
+    from functions.game_selection import get_game, get_diff, get_mode
+    from functions.setup_results import setup, end_screen
+    from functions.refresh_update import refresh_screen, update_status, find_start_word
+except:
+    from typetype.functions.game_selection import get_game, get_diff, get_mode
+    from typetype.functions.setup_results import setup, end_screen
+    from typetype.functions.refresh_update import refresh_screen, update_status, find_start_word
 import curses
 import time
 import random
 import os
 import argparse
 
 
@@ -227,8 +232,7 @@
 def callmain():
     #this is to take away the escape delay
     os.environ.setdefault('ESCDELAY', '25')
     #run main
     curses.wrapper(main)
 
 
-
```

### Comparing `typetype-1.0.5/typetype/functions/game_selection.py` & `typetype-1.0.6/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/functions/refresh_update.py` & `typetype-1.0.6/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/functions/setup_results.py` & `typetype-1.0.6/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/words/200words.txt` & `typetype-1.0.6/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/words/25000words.txt` & `typetype-1.0.6/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/words/5000words.txt` & `typetype-1.0.6/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.5/typetype/words/text.txt` & `typetype-1.0.6/typetype/words/text.txt`

 * *Files identical despite different names*

