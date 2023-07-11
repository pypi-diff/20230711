# Comparing `tmp/fix_db_wifi-0.1.0.tar.gz` & `tmp/fix_db_wifi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fix_db_wifi-0.1.0.tar", last modified: Tue Jul 11 10:31:05 2023, max compression
+gzip compressed data, was "fix_db_wifi-0.1.1.tar", last modified: Tue Jul 11 10:45:32 2023, max compression
```

## Comparing `fix_db_wifi-0.1.0.tar` & `fix_db_wifi-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:31:05.197381 fix_db_wifi-0.1.0/
--rw-rw-r--   0 jina      (1001) jina      (1001)      246 2023-07-11 10:31:05.197381 fix_db_wifi-0.1.0/PKG-INFO
--rw-rw-r--   0 jina      (1001) jina      (1001)     1051 2023-07-11 08:34:44.000000 fix_db_wifi-0.1.0/README.md
-drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:31:05.197381 fix_db_wifi-0.1.0/fix_db_wifi/
--rw-rw-r--   0 jina      (1001) jina      (1001)        0 2023-07-11 08:37:25.000000 fix_db_wifi-0.1.0/fix_db_wifi/__init__.py
--rw-rw-r--   0 jina      (1001) jina      (1001)     3060 2023-07-11 09:33:33.000000 fix_db_wifi-0.1.0/fix_db_wifi/main.py
-drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:31:05.197381 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/
--rw-rw-r--   0 jina      (1001) jina      (1001)      246 2023-07-11 10:31:05.000000 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/PKG-INFO
--rw-rw-r--   0 jina      (1001) jina      (1001)      240 2023-07-11 10:31:05.000000 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/SOURCES.txt
--rw-rw-r--   0 jina      (1001) jina      (1001)        1 2023-07-11 10:31:05.000000 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/dependency_links.txt
--rw-rw-r--   0 jina      (1001) jina      (1001)       55 2023-07-11 10:31:05.000000 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/entry_points.txt
--rw-rw-r--   0 jina      (1001) jina      (1001)       12 2023-07-11 10:31:05.000000 fix_db_wifi-0.1.0/fix_db_wifi.egg-info/top_level.txt
--rw-rw-r--   0 jina      (1001) jina      (1001)       38 2023-07-11 10:31:05.197381 fix_db_wifi-0.1.0/setup.cfg
--rw-rw-r--   0 jina      (1001) jina      (1001)      406 2023-07-11 10:29:19.000000 fix_db_wifi-0.1.0/setup.py
+drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:45:32.617669 fix_db_wifi-0.1.1/
+-rw-rw-r--   0 jina      (1001) jina      (1001)     1322 2023-07-11 10:45:32.617669 fix_db_wifi-0.1.1/PKG-INFO
+-rw-rw-r--   0 jina      (1001) jina      (1001)     1051 2023-07-11 08:34:44.000000 fix_db_wifi-0.1.1/README.md
+drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:45:32.613669 fix_db_wifi-0.1.1/fix_db_wifi/
+-rw-rw-r--   0 jina      (1001) jina      (1001)        0 2023-07-11 08:37:25.000000 fix_db_wifi-0.1.1/fix_db_wifi/__init__.py
+-rw-rw-r--   0 jina      (1001) jina      (1001)     3060 2023-07-11 09:33:33.000000 fix_db_wifi-0.1.1/fix_db_wifi/main.py
+drwxrwxr-x   0 jina      (1001) jina      (1001)        0 2023-07-11 10:45:32.617669 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/
+-rw-rw-r--   0 jina      (1001) jina      (1001)     1322 2023-07-11 10:45:32.000000 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/PKG-INFO
+-rw-rw-r--   0 jina      (1001) jina      (1001)      240 2023-07-11 10:45:32.000000 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/SOURCES.txt
+-rw-rw-r--   0 jina      (1001) jina      (1001)        1 2023-07-11 10:45:32.000000 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/dependency_links.txt
+-rw-rw-r--   0 jina      (1001) jina      (1001)       55 2023-07-11 10:45:32.000000 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/entry_points.txt
+-rw-rw-r--   0 jina      (1001) jina      (1001)       12 2023-07-11 10:45:32.000000 fix_db_wifi-0.1.1/fix_db_wifi.egg-info/top_level.txt
+-rw-rw-r--   0 jina      (1001) jina      (1001)       38 2023-07-11 10:45:32.617669 fix_db_wifi-0.1.1/setup.cfg
+-rw-rw-r--   0 jina      (1001) jina      (1001)      618 2023-07-11 10:40:52.000000 fix_db_wifi-0.1.1/setup.py
```

### Comparing `fix_db_wifi-0.1.0/README.md` & `fix_db_wifi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fix_db_wifi-0.1.0/fix_db_wifi/main.py` & `fix_db_wifi-0.1.1/fix_db_wifi/main.py`

 * *Files identical despite different names*

