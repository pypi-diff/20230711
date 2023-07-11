# Comparing `tmp/UnrealCV-0.4.0.tar.gz` & `tmp/UnrealCV-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/UnrealCV-0.4.0.tar", last modified: Mon Jul 15 04:50:57 2019, max compression
+gzip compressed data, was "UnrealCV-1.0.1.tar", last modified: Tue Jul 11 16:18:45 2023, max compression
```

## Comparing `UnrealCV-0.4.0.tar` & `UnrealCV-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-07-15 04:50:57.000000 UnrealCV-0.4.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2019-07-15 04:42:29.000000 UnrealCV-0.4.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      393 2019-07-15 04:50:57.000000 UnrealCV-0.4.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-07-15 04:50:57.000000 UnrealCV-0.4.0/unrealcv/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11887 2019-07-15 04:39:23.000000 UnrealCV-0.4.0/unrealcv/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10620 2018-12-19 03:00:54.000000 UnrealCV-0.4.0/unrealcv/automation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1052 2018-12-19 03:00:54.000000 UnrealCV-0.4.0/unrealcv/util.py
+drwxrwxr-x   0 zfw       (1000) zfw       (1000)        0 2023-07-11 16:18:45.825416 UnrealCV-1.0.1/
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)      383 2023-07-11 16:18:45.825416 UnrealCV-1.0.1/PKG-INFO
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)      634 2023-07-11 15:37:46.000000 UnrealCV-1.0.1/README.md
+drwxrwxr-x   0 zfw       (1000) zfw       (1000)        0 2023-07-11 16:18:45.825416 UnrealCV-1.0.1/UnrealCV.egg-info/
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)      383 2023-07-11 16:18:45.000000 UnrealCV-1.0.1/UnrealCV.egg-info/PKG-INFO
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)      207 2023-07-11 16:18:45.000000 UnrealCV-1.0.1/UnrealCV.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)        1 2023-07-11 16:18:45.000000 UnrealCV-1.0.1/UnrealCV.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)        9 2023-07-11 16:18:45.000000 UnrealCV-1.0.1/UnrealCV.egg-info/top_level.txt
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)       38 2023-07-11 16:18:45.825416 UnrealCV-1.0.1/setup.cfg
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)      540 2023-07-11 16:13:03.000000 UnrealCV-1.0.1/setup.py
+drwxrwxr-x   0 zfw       (1000) zfw       (1000)        0 2023-07-11 16:18:45.825416 UnrealCV-1.0.1/unrealcv/
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)    16312 2023-04-09 14:40:03.000000 UnrealCV-1.0.1/unrealcv/__init__.py
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)    10620 2023-04-07 14:00:53.000000 UnrealCV-1.0.1/unrealcv/automation.py
+-rw-rw-r--   0 zfw       (1000) zfw       (1000)     1052 2023-04-07 14:00:53.000000 UnrealCV-1.0.1/unrealcv/util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `UnrealCV-0.4.0/unrealcv/automation.py` & `UnrealCV-1.0.1/unrealcv/automation.py`

 * *Files identical despite different names*

### Comparing `UnrealCV-0.4.0/unrealcv/util.py` & `UnrealCV-1.0.1/unrealcv/util.py`

 * *Files identical despite different names*

