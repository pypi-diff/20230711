# Comparing `tmp/test_the_best-3.5.tar.gz` & `tmp/test_the_best-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_the_best-3.5.tar", last modified: Tue Jul 11 15:41:34 2023, max compression
+gzip compressed data, was "test_the_best-4.0.tar", last modified: Tue Jul 11 15:45:42 2023, max compression
```

## Comparing `test_the_best-3.5.tar` & `test_the_best-4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:41:34.500925 test_the_best-3.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:41:34.500925 test_the_best-3.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:38:45.000000 test_the_best-3.5/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/test_the_best/
--rw-r--r--   0 runner    (1000) runner    (1000)      956 2023-07-11 15:41:07.000000 test_the_best-3.5/test_the_best/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:41:34.500925 test_the_best-3.5/test_the_best.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-3.5/test_the_best.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:41:34.000000 test_the_best-3.5/test_the_best.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:45:42.896896 test_the_best-4.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:45:42.896896 test_the_best-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 15:45:42.896896 test_the_best-4.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-07-11 15:45:19.000000 test_the_best-4.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:45:42.892896 test_the_best-4.0/test_the_best/
+-rw-r--r--   0 runner    (1000) runner    (1000)      471 2023-07-11 15:45:02.000000 test_the_best-4.0/test_the_best/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 15:45:42.896896 test_the_best-4.0/test_the_best.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      153 2023-07-11 15:45:42.000000 test_the_best-4.0/test_the_best.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-11 15:45:42.000000 test_the_best-4.0/test_the_best.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 15:45:42.000000 test_the_best-4.0/test_the_best.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-4.0/test_the_best.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 15:45:42.000000 test_the_best-4.0/test_the_best.egg-info/top_level.txt
```

