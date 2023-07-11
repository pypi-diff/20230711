# Comparing `tmp/velikafkaclient-1.0.2.tar.gz` & `tmp/velikafkaclient-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.2.tar", last modified: Mon Jul 10 13:03:20 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.3.tar", last modified: Tue Jul 11 15:34:47 2023, max compression
```

## Comparing `velikafkaclient-1.0.2.tar` & `velikafkaclient-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.310267 velikafkaclient-1.0.2/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-10 13:03:20.310158 velikafkaclient-1.0.2/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-10 13:03:20.310296 velikafkaclient-1.0.2/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-10 13:03:03.000000 velikafkaclient-1.0.2/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.308621 velikafkaclient-1.0.2/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      374 2023-07-10 13:02:55.000000 velikafkaclient-1.0.2/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309446 velikafkaclient-1.0.2/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      126 2023-07-10 12:56:14.000000 velikafkaclient-1.0.2/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-10 12:56:14.000000 velikafkaclient-1.0.2/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309980 velikafkaclient-1.0.2/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309084 velikafkaclient-1.0.2/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      577 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060711 velikafkaclient-1.0.3/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3464 2023-07-11 15:34:47.060600 velikafkaclient-1.0.3/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3279 2023-07-11 15:34:28.000000 velikafkaclient-1.0.3/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-11 15:34:47.060741 velikafkaclient-1.0.3/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-11 15:34:36.000000 velikafkaclient-1.0.3/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.059157 velikafkaclient-1.0.3/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      374 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060042 velikafkaclient-1.0.3/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      126 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060416 velikafkaclient-1.0.3/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.059662 velikafkaclient-1.0.3/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3464 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      577 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.2/velikafkaclient/consumer.py` & `velikafkaclient-1.0.3/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.2/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.3/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.2/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.3/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.2/velikafkaclient/producer.py` & `velikafkaclient-1.0.3/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.2/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.3/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.2/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.3/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

