# Comparing `tmp/typetype-1.0.7.tar.gz` & `tmp/typetype-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.7.tar", last modified: Mon Jul 10 23:40:21 2023, max compression
+gzip compressed data, was "typetype-1.0.8.tar", last modified: Tue Jul 11 18:51:18 2023, max compression
```

## Comparing `typetype-1.0.7.tar` & `typetype-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.368714 typetype-1.0.7/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.7/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-10 23:40:21.368564 typetype-1.0.7/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.0.7/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 23:40:21.368772 typetype-1.0.7/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-10 23:39:37.000000 typetype-1.0.7/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.361978 typetype-1.0.7/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.7/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8008 2023-07-10 23:14:56.000000 typetype-1.0.7/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.363570 typetype-1.0.7/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.7/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.365213 typetype-1.0.7/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 22:57:55.000000 typetype-1.0.7/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.362674 typetype-1.0.7/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.571642 typetype-1.0.8/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.8/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 18:51:18.571476 typetype-1.0.8/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.0.8/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 18:51:18.571690 typetype-1.0.8/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      683 2023-07-11 18:10:16.000000 typetype-1.0.8/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.565325 typetype-1.0.8/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.8/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     9049 2023-07-11 18:44:09.000000 typetype-1.0.8/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.567382 typetype-1.0.8/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.8/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 17:23:53.000000 typetype-1.0.8/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.0.8/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.568932 typetype-1.0.8/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 18:47:22.000000 typetype-1.0.8/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.8/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 18:51:18.566487 typetype-1.0.8/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      550 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/requires.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 18:51:18.000000 typetype-1.0.8/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.7/PKG-INFO` & `typetype-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.0.7
+Version: 1.0.8
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.0.7/README.md` & `typetype-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/setup.py` & `typetype-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.0.7',
+    version='1.0.8',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'typetype=typetype.ahmetsgame:callmain'
         ]
     },
     install_requires=[
-] + (['windows-curses'] if sys.platform == 'win32' else [])
+] + (['windows-curses','keyboard'] if sys.platform == 'win32' else ['keyboard'])
 )
```

### Comparing `typetype-1.0.7/typetype/ahmetsgame.py` & `typetype-1.0.8/typetype/ahmetsgame.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     from typetype.functions.setup_results import setup, end_screen
     from typetype.functions.refresh_update import refresh_screen, update_status, find_start_word
 import curses
 import time
 import random
 import os
 import argparse
-
+import keyboard
+import ctypes
+import sys
 
 
 def main(stdscr):
     
     #get command line args
     cursor = False
     parser = argparse.ArgumentParser(description='Typing Game')
@@ -130,16 +132,16 @@
     
     #initialize the screen with the message and the initial sentence
     refresh_screen(stdscr, status, original_words, playing_game, new_words, extras, onword, start_time, timed, cursor)
     
     #loop that waits for user input
     while True:
         
-        #allow the getch() function to timeout so we can refresh the screen every 0.1 seconds
-        stdscr.timeout(100)
+        #allow the getch() function to timeout so we can refresh the screen every 0.3 seconds
+        stdscr.timeout(300)
         
         #wait for an input key
         key = stdscr.getch()
         try:
             char = chr(key)
         except:
             char = 'NA'
@@ -153,32 +155,56 @@
         if key == -1:
             refresh_screen(stdscr, status, original_words, playing_game, new_words, extras, onword, start_time, timed, cursor)
             continue
             
         
         #if the key is not a valid character, the delete key, or the esc key: go to the start of the loop
         #127 is the delete key and 27 is the esc key
-        if char not in valid_characters and key!=127 and key!=27:
+        if char not in valid_characters and key!=127 and key!=27 and key!=8:
             continue
         
         
         #start time when the user starts typing for the first time
         if not time_started:
             #* will return to menu if the game hasn't started
             if key == 42:
                 return 'm'
             time_started = True
             playing_game = True
             start_time = time.time()
         
         
         #if the delete key is pressed
-        if key == 127:
+        if key == 127 or key == 8:
+            try:
+                if sys.platform == 'win32':
+                    if keyboard.is_pressed('ctrl') or (ctypes.windll.user32.GetKeyState(0x11) & 0x8000):
+                        ctrldown = True
+                    else:
+                        ctrldown = False
+                else:
+                    ctrldown = False
+            except:
+                ctrldown = False
+            #if ctrl is also pressed
+            if ctrldown:
+                #delete the whole word plus extras
+                if len(extras[onword])>0:
+                    extras[onword] = ''
+                    new_words[onword] = ''
+                elif len(new_words[onword])>0:
+                    new_words[onword] = ''
+                elif onword>0:
+                    #if the word is empty then delete the whole previous word
+                    onword-=1
+                    extras[onword] = ''
+                    new_words[onword] = ''
+            #normal delete key
             #deleting from the current word
-            if len(extras[onword])>0:
+            elif len(extras[onword])>0:
                 extras[onword] = extras[onword][:-1]
             elif len(new_words[onword])>0:
                 new_words[onword] = new_words[onword][:-1]
             #move to previous word if the cursor is at the beginning of a word (if its not the first word)
             elif onword>0:
                 onword -= 1
             
@@ -231,8 +257,8 @@
 #used to call main
 def callmain():
     #this is to take away the escape delay
     os.environ.setdefault('ESCDELAY', '25')
     #run main
     curses.wrapper(main)
 
-
+callmain()
```

### Comparing `typetype-1.0.7/typetype/functions/game_selection.py` & `typetype-1.0.8/typetype/functions/game_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             elif active == 4:
                 return get_diff(stdscr, get_game(stdscr))
             elif active == 1 and (choice == 'x'):
                 return choice + 's'
             elif active == 3 and (choice == 'x'):
                 return choice + 'l'
         #delete
-        elif key == 127:
+        elif key == 127 or key == 8:
             return get_diff(stdscr, get_game(stdscr))
         
 
 
 
 
 
@@ -249,11 +249,11 @@
             elif active == 4 and choice[0] == 't':
                 return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
             elif active == 14 and choice[0] == 'w':
                 return choice + '4'
             elif active == 5:
                 return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
         #delete
-        elif key == 127:
+        elif key == 127 or key == 8:
             return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
```

### Comparing `typetype-1.0.7/typetype/functions/refresh_update.py` & `typetype-1.0.8/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype/functions/setup_results.py` & `typetype-1.0.8/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype/words/200words.txt` & `typetype-1.0.8/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype/words/25000words.txt` & `typetype-1.0.8/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype/words/5000words.txt` & `typetype-1.0.8/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype/words/text.txt` & `typetype-1.0.8/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.7/typetype.egg-info/PKG-INFO` & `typetype-1.0.8/typetype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.0.7
+Version: 1.0.8
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.0.7/typetype.egg-info/SOURCES.txt` & `typetype-1.0.8/typetype.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 typetype/__init__.py
 typetype/ahmetsgame.py
 typetype.egg-info/PKG-INFO
 typetype.egg-info/SOURCES.txt
 typetype.egg-info/dependency_links.txt
 typetype.egg-info/entry_points.txt
+typetype.egg-info/requires.txt
 typetype.egg-info/top_level.txt
 typetype/functions/__init__.py
 typetype/functions/game_selection.py
 typetype/functions/refresh_update.py
 typetype/functions/setup_results.py
 typetype/words/200words.txt
 typetype/words/25000words.txt
```

