# Comparing `tmp/test_the_best-2.5.tar.gz` & `tmp/test_the_best-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_the_best-2.5.tar", last modified: Tue Jul 11 15:24:13 2023, max compression
+gzip compressed data, was "test_the_best-3.0.tar", last modified: Tue Jul 11 15:30:52 2023, max compression
```

## Comparing `test_the_best-2.5.tar` & `test_the_best-3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:24:13.894969 test_the_best-2.5/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:24:13.894969 test_the_best-2.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:24:13.894969 test_the_best-2.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:23:32.000000 test_the_best-2.5/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:24:13.894969 test_the_best-2.5/test_the_best/
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2023-07-11 15:21:05.000000 test_the_best-2.5/test_the_best/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:24:13.894969 test_the_best-2.5/test_the_best.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:24:13.000000 test_the_best-2.5/test_the_best.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:24:13.000000 test_the_best-2.5/test_the_best.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:24:13.000000 test_the_best-2.5/test_the_best.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-2.5/test_the_best.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:24:13.000000 test_the_best-2.5/test_the_best.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.704999 test_the_best-3.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:30:52.704999 test_the_best-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:30:52.708999 test_the_best-3.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:30:27.000000 test_the_best-3.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.700999 test_the_best-3.0/test_the_best/
+-rw-r--r--   0 runner    (1000) runner    (1000)      654 2023-07-11 15:29:00.000000 test_the_best-3.0/test_the_best/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:30:52.700999 test_the_best-3.0/test_the_best.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:30:52.000000 test_the_best-3.0/test_the_best.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-3.0/test_the_best.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:30:51.000000 test_the_best-3.0/test_the_best.egg-info/top_level.txt
```

### Comparing `test_the_best-2.5/test_the_best/__init__.py` & `test_the_best-3.0/test_the_best/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
   JUMP_LEFT_SEQ = '\u001b[100D'
   DELAY = 0.05
   for i in range(0, 101):
     sleep(DELAY)
     print(JUMP_LEFT_SEQ, end='')
     print(f'Progress: {i:0>3}%', end='')
     stdout.flush()
-    print()
   y = "Тест пройден?"
   if x == y:
     x = "Пройден!"
     return x
   if x != None:
     return x
   else:
```

