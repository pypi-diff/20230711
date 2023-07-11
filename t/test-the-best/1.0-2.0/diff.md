# Comparing `tmp/test_the_best-1.0.tar.gz` & `tmp/test_the_best-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_the_best-1.0.tar", last modified: Tue Jul 11 14:16:45 2023, max compression
+gzip compressed data, was "test_the_best-2.0.tar", last modified: Tue Jul 11 14:49:34 2023, max compression
```

## Comparing `test_the_best-1.0.tar` & `test_the_best-2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:16:45.617924 test_the_best-1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 14:16:45.617924 test_the_best-1.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 14:16:45.617924 test_the_best-1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 14:00:49.000000 test_the_best-1.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:16:45.617924 test_the_best-1.0/test_the_best/
--rw-r--r--   0 runner    (1000) runner    (1000)      204 2023-07-11 14:13:35.000000 test_the_best-1.0/test_the_best/_init_.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:16:45.617924 test_the_best-1.0/test_the_best.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 14:16:45.000000 test_the_best-1.0/test_the_best.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-07-11 14:16:45.000000 test_the_best-1.0/test_the_best.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-1.0/test_the_best.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-1.0/test_the_best.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 14:16:45.000000 test_the_best-1.0/test_the_best.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:49:34.552749 test_the_best-2.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 14:49:34.552749 test_the_best-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 14:49:34.556748 test_the_best-2.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 14:47:34.000000 test_the_best-2.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:49:34.552749 test_the_best-2.0/test_the_best/
+-rw-r--r--   0 runner    (1000) runner    (1000)      204 2023-07-11 14:46:43.000000 test_the_best-2.0/test_the_best/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 14:49:34.552749 test_the_best-2.0/test_the_best.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 14:49:33.000000 test_the_best-2.0/test_the_best.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 14:49:33.000000 test_the_best-2.0/test_the_best.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:49:33.000000 test_the_best-2.0/test_the_best.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-2.0/test_the_best.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 14:49:33.000000 test_the_best-2.0/test_the_best.egg-info/top_level.txt
```

