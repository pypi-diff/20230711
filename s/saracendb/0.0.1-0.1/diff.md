# Comparing `tmp/saracendb-0.0.1.tar.gz` & `tmp/saracendb-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.0.1.tar", last modified: Tue Jul 11 15:34:08 2023, max compression
+gzip compressed data, was "saracendb-0.1.tar", last modified: Tue Jul 11 15:08:45 2023, max compression
```

## Comparing `saracendb-0.0.1.tar` & `saracendb-0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:34:08.608301 saracendb-0.0.1/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      554 2023-07-11 15:34:08.608152 saracendb-0.0.1/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      125 2023-07-11 14:51:10.000000 saracendb-0.0.1/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:34:08.606824 saracendb-0.0.1/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1674 2023-07-11 15:22:02.000000 saracendb-0.0.1/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:34:08.607905 saracendb-0.0.1/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      554 2023-07-11 15:34:08.000000 saracendb-0.0.1/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-11 15:34:08.000000 saracendb-0.0.1/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-11 15:34:08.000000 saracendb-0.0.1/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        8 2023-07-11 15:34:08.000000 saracendb-0.0.1/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-11 15:34:08.000000 saracendb-0.0.1/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-11 15:34:08.608343 saracendb-0.0.1/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      916 2023-07-11 15:26:13.000000 saracendb-0.0.1/setup.py
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

### Comparing `saracendb-0.0.1/PKG-INFO` & `saracendb-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.0.1
+Version: 0.1
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.0.1/saracendb/__init__.py` & `saracendb-0.1/saracendb/main.py`

 * *Files identical despite different names*

### Comparing `saracendb-0.0.1/saracendb.egg-info/PKG-INFO` & `saracendb-0.1/saracendb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.0.1
+Version: 0.1
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.0.1/setup.py` & `saracendb-0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.1'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

