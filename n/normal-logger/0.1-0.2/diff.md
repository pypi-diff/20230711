# Comparing `tmp/normal_logger-0.1.tar.gz` & `tmp/normal-logger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normal_logger-0.1.tar", last modified: Mon Jul 10 22:15:34 2023, max compression
+gzip compressed data, was "normal-logger-0.2.tar", last modified: Mon Jul 10 22:26:28 2023, max compression
```

## Comparing `normal_logger-0.1.tar` & `normal-logger-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 22:15:34.301528 normal_logger-0.1/
--rw-rw-rw-   0        0        0      153 2023-07-10 22:15:34.295927 normal_logger-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 22:15:34.233594 normal_logger-0.1/normal_logger/
--rw-rw-rw-   0        0        0     1966 2023-07-10 22:09:33.000000 normal_logger-0.1/normal_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 22:15:34.290814 normal_logger-0.1/normal_logger.egg-info/
--rw-rw-rw-   0        0        0      153 2023-07-10 22:15:34.000000 normal_logger-0.1/normal_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-10 22:15:34.000000 normal_logger-0.1/normal_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 22:15:34.000000 normal_logger-0.1/normal_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 22:15:34.000000 normal_logger-0.1/normal_logger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 22:15:34.000000 normal_logger-0.1/normal_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 22:15:34.301528 normal_logger-0.1/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-07-10 22:15:26.000000 normal_logger-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 22:26:28.756192 normal-logger-0.2/
+-rw-rw-rw-   0        0        0      168 2023-07-10 22:26:28.756192 normal-logger-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 22:26:28.682944 normal-logger-0.2/normal-logger/
+-rw-rw-rw-   0        0        0     1964 2023-07-10 22:25:09.000000 normal-logger-0.2/normal-logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 22:26:28.746941 normal-logger-0.2/normal_logger.egg-info/
+-rw-rw-rw-   0        0        0      168 2023-07-10 22:26:28.000000 normal-logger-0.2/normal_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-10 22:26:28.000000 normal-logger-0.2/normal_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 22:26:28.000000 normal-logger-0.2/normal_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 22:26:28.000000 normal-logger-0.2/normal_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 22:26:28.000000 normal-logger-0.2/normal_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 22:26:28.756192 normal-logger-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      440 2023-07-10 22:22:42.000000 normal-logger-0.2/setup.py
```

### Comparing `normal_logger-0.1/normal_logger/__init__.py` & `normal-logger-0.2/normal-logger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 import time
 
 __autor__ = "N0rmalUser"
-__version__ = "0.0.1"
+__version__ = "0.1"
 
 def _tagger(func):
     def wrapper(self, *args):
         i=0
         message = ''
         while i < len(args):
             if i == len(args)-1:
```

