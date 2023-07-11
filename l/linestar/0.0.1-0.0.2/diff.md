# Comparing `tmp/linestar-0.0.1.tar.gz` & `tmp/linestar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linestar-0.0.1.tar", last modified: Tue Jul 11 10:44:54 2023, max compression
+gzip compressed data, was "linestar-0.0.2.tar", last modified: Tue Jul 11 11:39:05 2023, max compression
```

## Comparing `linestar-0.0.1.tar` & `linestar-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 zyler      (501) staff       (20)        0 2023-07-11 10:44:54.977456 linestar-0.0.1/
--rw-r--r--   0 zyler      (501) staff       (20)      270 2023-07-11 10:44:54.977362 linestar-0.0.1/PKG-INFO
-drwxr-xr-x   0 zyler      (501) staff       (20)        0 2023-07-11 10:44:54.977192 linestar-0.0.1/linestar.egg-info/
--rw-r--r--   0 zyler      (501) staff       (20)      270 2023-07-11 10:44:54.000000 linestar-0.0.1/linestar.egg-info/PKG-INFO
--rw-r--r--   0 zyler      (501) staff       (20)      167 2023-07-11 10:44:54.000000 linestar-0.0.1/linestar.egg-info/SOURCES.txt
--rw-r--r--   0 zyler      (501) staff       (20)        1 2023-07-11 10:44:54.000000 linestar-0.0.1/linestar.egg-info/dependency_links.txt
--rw-r--r--   0 zyler      (501) staff       (20)       22 2023-07-11 10:44:54.000000 linestar-0.0.1/linestar.egg-info/requires.txt
--rw-r--r--   0 zyler      (501) staff       (20)        1 2023-07-11 10:44:54.000000 linestar-0.0.1/linestar.egg-info/top_level.txt
--rw-r--r--   0 zyler      (501) staff       (20)       38 2023-07-11 10:44:54.977517 linestar-0.0.1/setup.cfg
--rw-r--r--   0 zyler      (501) staff       (20)      394 2023-07-11 10:44:28.000000 linestar-0.0.1/setup.py
+drwxr-xr-x   0 zyler      (501) staff       (20)        0 2023-07-11 11:39:05.712082 linestar-0.0.2/
+-rw-r--r--   0 zyler      (501) staff       (20)      270 2023-07-11 11:39:05.711987 linestar-0.0.2/PKG-INFO
+-rw-r--r--   0 zyler      (501) staff       (20)     2255 2023-07-11 11:38:10.000000 linestar-0.0.2/README.md
+drwxr-xr-x   0 zyler      (501) staff       (20)        0 2023-07-11 11:39:05.711841 linestar-0.0.2/linestar.egg-info/
+-rw-r--r--   0 zyler      (501) staff       (20)      270 2023-07-11 11:39:05.000000 linestar-0.0.2/linestar.egg-info/PKG-INFO
+-rw-r--r--   0 zyler      (501) staff       (20)      177 2023-07-11 11:39:05.000000 linestar-0.0.2/linestar.egg-info/SOURCES.txt
+-rw-r--r--   0 zyler      (501) staff       (20)        1 2023-07-11 11:39:05.000000 linestar-0.0.2/linestar.egg-info/dependency_links.txt
+-rw-r--r--   0 zyler      (501) staff       (20)       49 2023-07-11 11:39:05.000000 linestar-0.0.2/linestar.egg-info/requires.txt
+-rw-r--r--   0 zyler      (501) staff       (20)        1 2023-07-11 11:39:05.000000 linestar-0.0.2/linestar.egg-info/top_level.txt
+-rw-r--r--   0 zyler      (501) staff       (20)       38 2023-07-11 11:39:05.712123 linestar-0.0.2/setup.cfg
+-rw-r--r--   0 zyler      (501) staff       (20)      454 2023-07-11 11:39:01.000000 linestar-0.0.2/setup.py
```

