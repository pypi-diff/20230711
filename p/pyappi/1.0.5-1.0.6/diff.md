# Comparing `tmp/pyappi-1.0.5.tar.gz` & `tmp/pyappi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappi-1.0.5.tar", last modified: Sat Jul  8 00:36:20 2023, max compression
+gzip compressed data, was "pyappi-1.0.6.tar", last modified: Tue Jul 11 18:55:17 2023, max compression
```

## Comparing `pyappi-1.0.5.tar` & `pyappi-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 00:36:20.485476 pyappi-1.0.5/
--rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      324 2023-07-08 00:36:20.484463 pyappi-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-22 21:24:09.000000 pyappi-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 00:36:20.458100 pyappi-1.0.5/pyappi/
--rw-rw-rw-   0        0        0       21 2023-07-08 00:33:13.000000 pyappi-1.0.5/pyappi/__init__.py
--rw-rw-rw-   0        0        0      509 2023-07-03 23:24:25.000000 pyappi-1.0.5/pyappi/api_base.py
--rw-rw-rw-   0        0        0      128 2023-07-08 00:30:49.000000 pyappi-1.0.5/pyappi/client.py
--rw-rw-rw-   0        0        0      393 2023-07-07 20:33:20.000000 pyappi-1.0.5/pyappi/endpoints.py
--rw-rw-rw-   0        0        0      365 2023-07-08 00:30:21.000000 pyappi-1.0.5/pyappi/main.py
-drwxrwxrwx   0        0        0        0 2023-07-08 00:36:20.479393 pyappi-1.0.5/pyappi.egg-info/
--rw-rw-rw-   0        0        0      324 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-08 00:36:20.000000 pyappi-1.0.5/pyappi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 00:36:20.485476 pyappi-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      589 2023-07-08 00:35:08.000000 pyappi-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 00:36:20.482424 pyappi-1.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-06-13 18:44:20.000000 pyappi-1.0.5/tests/test_core.py
--rw-rw-rw-   0        0        0     1051 2023-06-13 18:55:48.000000 pyappi-1.0.5/tests/test_log.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.184359 pyappi-1.0.6/
+-rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      324 2023-07-11 18:55:17.183366 pyappi-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-22 21:24:09.000000 pyappi-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.108371 pyappi-1.0.6/pyappi/
+-rw-rw-rw-   0        0        0       21 2023-07-08 00:33:13.000000 pyappi-1.0.6/pyappi/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-07-03 23:24:25.000000 pyappi-1.0.6/pyappi/api_base.py
+-rw-rw-rw-   0        0        0     1685 2023-07-08 03:59:51.000000 pyappi-1.0.6/pyappi/client.py
+-rw-rw-rw-   0        0        0      393 2023-07-07 20:33:20.000000 pyappi-1.0.6/pyappi/endpoints.py
+-rw-rw-rw-   0        0        0      420 2023-07-08 00:44:19.000000 pyappi-1.0.6/pyappi/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.148967 pyappi-1.0.6/pyappi.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:55:17.185367 pyappi-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-07-11 18:54:56.000000 pyappi-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.181369 pyappi-1.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-06-13 18:44:20.000000 pyappi-1.0.6/tests/test_core.py
+-rw-rw-rw-   0        0        0     1051 2023-06-13 18:55:48.000000 pyappi-1.0.6/tests/test_log.py
```

### Comparing `pyappi-1.0.5/tests/test_core.py` & `pyappi-1.0.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyappi-1.0.5/tests/test_log.py` & `pyappi-1.0.6/tests/test_log.py`

 * *Files identical despite different names*

