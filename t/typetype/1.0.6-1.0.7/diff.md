# Comparing `tmp/typetype-1.0.6.tar.gz` & `tmp/typetype-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.6.tar", last modified: Mon Jul 10 22:58:29 2023, max compression
+gzip compressed data, was "typetype-1.0.7.tar", last modified: Mon Jul 10 23:40:21 2023, max compression
```

## Comparing `typetype-1.0.6.tar` & `typetype-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.839564 typetype-1.0.6/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.6/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 22:58:29.839438 typetype-1.0.6/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.6/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 22:58:29.839611 typetype-1.0.6/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      487 2023-07-10 22:56:21.000000 typetype-1.0.6/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.834201 typetype-1.0.6/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.6/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8008 2023-07-10 22:56:38.000000 typetype-1.0.6/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.835687 typetype-1.0.6/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.6/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.837079 typetype-1.0.6/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 22:57:55.000000 typetype-1.0.6/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.6/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:58:29.834941 typetype-1.0.6/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 22:58:29.000000 typetype-1.0.6/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.368714 typetype-1.0.7/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.0.7/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-10 23:40:21.368564 typetype-1.0.7/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.0.7/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 23:40:21.368772 typetype-1.0.7/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-10 23:39:37.000000 typetype-1.0.7/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.361978 typetype-1.0.7/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.0.7/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8008 2023-07-10 23:14:56.000000 typetype-1.0.7/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.363570 typetype-1.0.7/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.7/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.365213 typetype-1.0.7/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 22:57:55.000000 typetype-1.0.7/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.7/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 23:40:21.362674 typetype-1.0.7/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 23:40:21.000000 typetype-1.0.7/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.6/typetype/ahmetsgame.py` & `typetype-1.0.7/typetype/ahmetsgame.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/functions/game_selection.py` & `typetype-1.0.7/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/functions/refresh_update.py` & `typetype-1.0.7/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/functions/setup_results.py` & `typetype-1.0.7/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/words/200words.txt` & `typetype-1.0.7/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/words/25000words.txt` & `typetype-1.0.7/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/words/5000words.txt` & `typetype-1.0.7/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype/words/text.txt` & `typetype-1.0.7/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.6/typetype.egg-info/SOURCES.txt` & `typetype-1.0.7/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

