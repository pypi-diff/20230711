# Comparing `tmp/typetype-1.0.8.tar.gz` & `tmp/typetype-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.8.tar", last modified: Tue Jul 11 18:51:18 2023, max compression
+gzip compressed data, was "typetype-1.1.0.tar", last modified: Tue Jul 11 21:46:40 2023, max compression
```

## Comparing `typetype-1.0.8.tar` & `typetype-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.571642 typetype-1.0.8/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.8/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 18:51:18.571476 typetype-1.0.8/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.0.8/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 18:51:18.571690 typetype-1.0.8/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      683 2023-07-11 18:10:16.000000 typetype-1.0.8/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.565325 typetype-1.0.8/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.8/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     9049 2023-07-11 18:44:09.000000 typetype-1.0.8/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.567382 typetype-1.0.8/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.8/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 17:23:53.000000 typetype-1.0.8/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.0.8/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.568932 typetype-1.0.8/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 18:47:22.000000 typetype-1.0.8/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.566487 typetype-1.0.8/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      550 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/requires.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.443306 typetype-1.1.0/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.0/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 21:46:40.443154 typetype-1.1.0/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.1.0/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 21:46:40.443352 typetype-1.1.0/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      683 2023-07-11 21:45:24.000000 typetype-1.1.0/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.436918 typetype-1.1.0/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.0/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     9072 2023-07-11 21:45:25.000000 typetype-1.1.0/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.438493 typetype-1.1.0/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.0/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 17:23:53.000000 typetype-1.1.0/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.0/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.439956 typetype-1.1.0/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 21:44:48.000000 typetype-1.1.0/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.437743 typetype-1.1.0/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      550 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/requires.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.8/PKG-INFO` & `typetype-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.0.8
+Version: 1.1.0
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.0.8/README.md` & `typetype-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/setup.py` & `typetype-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.0.8',
+    version='1.1.0',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.0.8/typetype/ahmetsgame.py` & `typetype-1.1.0/typetype/ahmetsgame.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     from typetype.functions.setup_results import setup, end_screen
     from typetype.functions.refresh_update import refresh_screen, update_status, find_start_word
 import curses
 import time
 import random
 import os
 import argparse
-import keyboard
 import ctypes
 import sys
 
 
 def main(stdscr):
     
     #get command line args
@@ -28,15 +27,16 @@
         cursor = True
     
     #start and setup colors and use the default terminal color as the background
     curses.start_color()
     curses.use_default_colors()
     stdscr.clear()
     #grey
-    curses.init_pair(1, 235, -1)
+    curses.init_color(curses.COLOR_CYAN, 500, 500, 500)
+    curses.init_pair(1, curses.COLOR_CYAN, -1)
     #white
     curses.init_pair(2, curses.COLOR_WHITE, -1)
     #(error)
     curses.init_pair(3, 160, -1)
     #(extra)
     #change color red to a greyish salmon color
     curses.init_color(curses.COLOR_RED, 300, 150, 150)
@@ -173,15 +173,15 @@
             start_time = time.time()
         
         
         #if the delete key is pressed
         if key == 127 or key == 8:
             try:
                 if sys.platform == 'win32':
-                    if keyboard.is_pressed('ctrl') or (ctypes.windll.user32.GetKeyState(0x11) & 0x8000):
+                    if (ctypes.windll.user32.GetKeyState(0x11) & 0x8000):
                         ctrldown = True
                     else:
                         ctrldown = False
                 else:
                     ctrldown = False
             except:
                 ctrldown = False
```

### Comparing `typetype-1.0.8/typetype/functions/game_selection.py` & `typetype-1.1.0/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/functions/refresh_update.py` & `typetype-1.1.0/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/functions/setup_results.py` & `typetype-1.1.0/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/words/200words.txt` & `typetype-1.1.0/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/words/25000words.txt` & `typetype-1.1.0/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/words/5000words.txt` & `typetype-1.1.0/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype/words/text.txt` & `typetype-1.1.0/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.8/typetype.egg-info/PKG-INFO` & `typetype-1.1.0/typetype.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.0.8
+Version: 1.1.0
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.0.8/typetype.egg-info/SOURCES.txt` & `typetype-1.1.0/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

