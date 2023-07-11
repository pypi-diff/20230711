# Comparing `tmp/saracendb-0.0.3.tar.gz` & `tmp/saracendb-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.0.3.tar", last modified: Tue Jul 11 15:57:42 2023, max compression
+gzip compressed data, was "saracendb-0.1.tar", last modified: Tue Jul 11 15:08:45 2023, max compression
```

## Comparing `saracendb-0.0.3.tar` & `saracendb-0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:57:42.023779 saracendb-0.0.3/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     2343 2023-07-11 15:57:42.023574 saracendb-0.0.3/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1914 2023-07-11 15:57:26.000000 saracendb-0.0.3/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:57:42.022647 saracendb-0.0.3/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1674 2023-07-11 15:22:02.000000 saracendb-0.0.3/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:57:42.023333 saracendb-0.0.3/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     2343 2023-07-11 15:57:41.000000 saracendb-0.0.3/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-11 15:57:42.000000 saracendb-0.0.3/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-11 15:57:41.000000 saracendb-0.0.3/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        8 2023-07-11 15:57:41.000000 saracendb-0.0.3/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-11 15:57:41.000000 saracendb-0.0.3/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-11 15:57:42.023816 saracendb-0.0.3/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      916 2023-07-11 15:57:37.000000 saracendb-0.0.3/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.712320 saracendb-0.1/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.712176 saracendb-0.1/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      125 2023-07-11 14:51:10.000000 saracendb-0.1/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711159 saracendb-0.1/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 14:52:10.000000 saracendb-0.1/saracendb/__init__.py
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     1674 2023-07-11 14:51:30.000000 saracendb-0.1/saracendb/main.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711967 saracendb-0.1/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      222 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        8 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-11 15:08:45.712364 saracendb-0.1/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      914 2023-07-11 15:06:06.000000 saracendb-0.1/setup.py
```

### Comparing `saracendb-0.0.3/saracendb/__init__.py` & `saracendb-0.1/saracendb/main.py`

 * *Files identical despite different names*

### Comparing `saracendb-0.0.3/setup.py` & `saracendb-0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.1'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

