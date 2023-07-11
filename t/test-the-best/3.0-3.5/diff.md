# Comparing `tmp/test_the_best-3.0.tar.gz` & `tmp/test_the_best-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_the_best-3.0.tar", last modified: Tue Jul 11 15:30:52 2023, max compression
+gzip compressed data, was "test_the_best-3.5.tar", last modified: Tue Jul 11 15:41:34 2023, max compression
```

## Comparing `test_the_best-3.0.tar` & `test_the_best-3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.704999 test_the_best-3.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:30:52.704999 test_the_best-3.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:30:52.708999 test_the_best-3.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:30:27.000000 test_the_best-3.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.700999 test_the_best-3.0/test_the_best/
--rw-r--r--   0 runner    (1000) runner    (1000)      654 2023-07-11 15:29:00.000000 test_the_best-3.0/test_the_best/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.700999 test_the_best-3.0/test_the_best.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:30:52.000000 test_the_best-3.0/test_the_best.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-3.0/test_the_best.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:41:34.500925 test_the_best-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:41:34.500925 test_the_best-3.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:38:45.000000 test_the_best-3.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/test_the_best/
+-rw-r--r--   0 runner    (1000) runner    (1000)      956 2023-07-11 15:41:07.000000 test_the_best-3.5/test_the_best/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/test_the_best.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-3.5/test_the_best.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/top_level.txt
```

### Comparing `test_the_best-3.0/test_the_best/__init__.py` & `test_the_best-3.5/test_the_best/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from time import sleep
 from sys import stdout
 
 def test(x = None):
   JUMP_LEFT_SEQ = '\u001b[100D'
   DELAY = 0.05
-  for i in range(0, 101):
-    sleep(DELAY)
-    print(JUMP_LEFT_SEQ, end='')
-    print(f'Progress: {i:0>3}%', end='')
-    stdout.flush()
   y = "Тест пройден?"
   if x == y:
+    for i in range(0, 101):
+      sleep(DELAY)
+      print(JUMP_LEFT_SEQ, end='')
+      print(f'Progress: {i:0>3}%', end='')
+      stdout.flush()
     x = "Пройден!"
     return x
   if x != None:
+    for i in range(0, 101):
+      sleep(DELAY)
+      print(JUMP_LEFT_SEQ, end='')
+      print(f'Progress: {i:0>3}%', end='')
+      stdout.flush()
     return x
   else:
+    for i in range(0, 101):
+      sleep(DELAY)
+      print(JUMP_LEFT_SEQ, end='')
+      print(f'Progress: {i:0>3}%', end='')
+      stdout.flush()
     x = "Тест успешно пройден!"
     return x
 
 def loading(DELAY):
     JUMP_LEFT_SEQ = '\u001b[100D'
     for i in range(0, 101):
         sleep(DELAY)
```

