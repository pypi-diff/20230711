# Comparing `tmp/pyappi-1.0.6.tar.gz` & `tmp/pyappi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappi-1.0.6.tar", last modified: Tue Jul 11 18:55:17 2023, max compression
+gzip compressed data, was "pyappi-1.0.7.tar", last modified: Tue Jul 11 19:04:29 2023, max compression
```

## Comparing `pyappi-1.0.6.tar` & `pyappi-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.184359 pyappi-1.0.6/
--rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      324 2023-07-11 18:55:17.183366 pyappi-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-22 21:24:09.000000 pyappi-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.108371 pyappi-1.0.6/pyappi/
--rw-rw-rw-   0        0        0       21 2023-07-08 00:33:13.000000 pyappi-1.0.6/pyappi/__init__.py
--rw-rw-rw-   0        0        0      509 2023-07-03 23:24:25.000000 pyappi-1.0.6/pyappi/api_base.py
--rw-rw-rw-   0        0        0     1685 2023-07-08 03:59:51.000000 pyappi-1.0.6/pyappi/client.py
--rw-rw-rw-   0        0        0      393 2023-07-07 20:33:20.000000 pyappi-1.0.6/pyappi/endpoints.py
--rw-rw-rw-   0        0        0      420 2023-07-08 00:44:19.000000 pyappi-1.0.6/pyappi/main.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.148967 pyappi-1.0.6/pyappi.egg-info/
--rw-rw-rw-   0        0        0      324 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 18:55:16.000000 pyappi-1.0.6/pyappi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:55:17.185367 pyappi-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-07-11 18:54:56.000000 pyappi-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:55:17.181369 pyappi-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-06-13 18:44:20.000000 pyappi-1.0.6/tests/test_core.py
--rw-rw-rw-   0        0        0     1051 2023-06-13 18:55:48.000000 pyappi-1.0.6/tests/test_log.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.650276 pyappi-1.0.7/
+-rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      324 2023-07-11 19:04:29.649707 pyappi-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-22 21:24:09.000000 pyappi-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.461182 pyappi-1.0.7/pyappi/
+-rw-rw-rw-   0        0        0       21 2023-07-08 00:33:13.000000 pyappi-1.0.7/pyappi/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-07-03 23:24:25.000000 pyappi-1.0.7/pyappi/api_base.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.504892 pyappi-1.0.7/pyappi/block/
+-rw-rw-rw-   0        0        0       20 2023-06-29 21:07:31.000000 pyappi-1.0.7/pyappi/block/__init__.py
+-rw-rw-rw-   0        0        0      805 2023-06-29 22:48:03.000000 pyappi-1.0.7/pyappi/block/block.py
+-rw-rw-rw-   0        0        0     1151 2023-06-30 15:38:36.000000 pyappi-1.0.7/pyappi/block/endpoints.py
+-rw-rw-rw-   0        0        0     1685 2023-07-08 03:59:51.000000 pyappi-1.0.7/pyappi/client.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.573630 pyappi-1.0.7/pyappi/document/
+-rw-rw-rw-   0        0        0        0 2023-06-29 22:51:45.000000 pyappi-1.0.7/pyappi/document/__init__.py
+-rw-rw-rw-   0        0        0     4004 2023-07-04 03:13:30.000000 pyappi-1.0.7/pyappi/document/access.py
+-rw-rw-rw-   0        0        0      831 2023-07-03 23:41:45.000000 pyappi-1.0.7/pyappi/document/delta.py
+-rw-rw-rw-   0        0        0     5853 2023-07-06 20:35:40.000000 pyappi-1.0.7/pyappi/document/document.py
+-rw-rw-rw-   0        0        0     1399 2023-07-07 16:34:29.000000 pyappi-1.0.7/pyappi/document/endpoints.py
+-rw-rw-rw-   0        0        0     1407 2023-07-07 16:33:46.000000 pyappi-1.0.7/pyappi/document/enumeration.py
+-rw-rw-rw-   0        0        0      522 2023-07-04 00:22:35.000000 pyappi-1.0.7/pyappi/document/exceptions.py
+-rw-rw-rw-   0        0        0       51 2023-06-09 00:47:46.000000 pyappi-1.0.7/pyappi/document/file_handler.py
+-rw-rw-rw-   0        0        0      732 2023-07-06 20:35:11.000000 pyappi-1.0.7/pyappi/document/history.py
+-rw-rw-rw-   0        0        0     1082 2023-07-04 03:03:24.000000 pyappi-1.0.7/pyappi/document/local.py
+-rw-rw-rw-   0        0        0       56 2023-06-30 17:52:39.000000 pyappi-1.0.7/pyappi/document/lock.py
+-rw-rw-rw-   0        0        0      268 2023-07-04 02:54:45.000000 pyappi-1.0.7/pyappi/document/merge.py
+-rw-rw-rw-   0        0        0       44 2023-05-23 15:16:01.000000 pyappi-1.0.7/pyappi/document/random_handler.py
+-rw-rw-rw-   0        0        0       28 2023-06-30 21:02:53.000000 pyappi-1.0.7/pyappi/document/rules.py
+-rw-rw-rw-   0        0        0    12100 2023-07-04 03:08:43.000000 pyappi-1.0.7/pyappi/document/transaction.py
+-rw-rw-rw-   0        0        0      214 2023-05-23 16:15:55.000000 pyappi-1.0.7/pyappi/document/type.py
+-rw-rw-rw-   0        0        0     2251 2023-06-30 23:06:17.000000 pyappi-1.0.7/pyappi/document/volatile_document.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.577633 pyappi-1.0.7/pyappi/encoding/
+-rw-rw-rw-   0        0        0       18 2023-06-30 15:37:44.000000 pyappi-1.0.7/pyappi/encoding/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-06-30 22:03:19.000000 pyappi-1.0.7/pyappi/encoding/url.py
+-rw-rw-rw-   0        0        0      393 2023-07-07 20:33:20.000000 pyappi-1.0.7/pyappi/endpoints.py
+-rw-rw-rw-   0        0        0      420 2023-07-08 00:44:19.000000 pyappi-1.0.7/pyappi/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.582129 pyappi-1.0.7/pyappi/stats/
+-rw-rw-rw-   0        0        0        0 2023-07-07 16:51:33.000000 pyappi-1.0.7/pyappi/stats/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-07 20:29:18.000000 pyappi-1.0.7/pyappi/stats/endpoints.py
+-rw-rw-rw-   0        0        0     3093 2023-07-07 21:03:15.000000 pyappi-1.0.7/pyappi/stats/stats.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.593600 pyappi-1.0.7/pyappi/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:02:07.000000 pyappi-1.0.7/pyappi/sync/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-07-07 22:53:32.000000 pyappi-1.0.7/pyappi/sync/endpoints.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.597379 pyappi-1.0.7/pyappi/user/
+-rw-rw-rw-   0        0        0        0 2023-06-29 22:57:32.000000 pyappi-1.0.7/pyappi/user/__init__.py
+-rw-rw-rw-   0        0        0     1433 2023-07-07 03:34:20.000000 pyappi-1.0.7/pyappi/user/endpoints.py
+-rw-rw-rw-   0        0        0     1297 2023-07-04 01:55:41.000000 pyappi-1.0.7/pyappi/user/session.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.641599 pyappi-1.0.7/pyappi/util/
+-rw-rw-rw-   0        0        0        0 2023-07-03 21:45:39.000000 pyappi-1.0.7/pyappi/util/__init__.py
+-rw-rw-rw-   0        0        0      300 2023-07-07 03:06:32.000000 pyappi-1.0.7/pyappi/util/filename.py
+-rw-rw-rw-   0        0        0      740 2023-07-07 20:13:32.000000 pyappi-1.0.7/pyappi/util/interval.py
+-rw-rw-rw-   0        0        0      654 2023-07-08 03:58:38.000000 pyappi-1.0.7/pyappi/util/login.py
+-rw-rw-rw-   0        0        0      274 2023-07-03 22:20:39.000000 pyappi-1.0.7/pyappi/util/merge.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.485433 pyappi-1.0.7/pyappi.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1266 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 19:04:29.000000 pyappi-1.0.7/pyappi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 19:04:29.651283 pyappi-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-07-11 19:04:19.000000 pyappi-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:04:29.646996 pyappi-1.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-06-13 18:44:20.000000 pyappi-1.0.7/tests/test_core.py
+-rw-rw-rw-   0        0        0     1051 2023-06-13 18:55:48.000000 pyappi-1.0.7/tests/test_log.py
```

### Comparing `pyappi-1.0.6/pyappi/client.py` & `pyappi-1.0.7/pyappi/client.py`

 * *Files identical despite different names*

### Comparing `pyappi-1.0.6/setup.py` & `pyappi-1.0.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 
 setup(
     name='pyappi',
-    version='1.0.6',
-    packages=['pyappi', 'tests'],
+    version='1.0.7',
+    packages=['pyappi', 'tests','pyappi.block','pyappi.document','pyappi.encoding','pyappi.stats','pyappi.stats','pyappi.sync','pyappi.user','pyappi.util'],
     license='Copyright (c) All Rights Reserved',
     description="Native Python Appi implementation. Single threaded, single node, no plug-ins.",
     long_description=open('README.md').read(),
     entry_points={
         'console_scripts': ['pyappi=pyappi.main:main',
                             'pyappi-client=pyappi.client:main'
                             ],
```

### Comparing `pyappi-1.0.6/tests/test_core.py` & `pyappi-1.0.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyappi-1.0.6/tests/test_log.py` & `pyappi-1.0.7/tests/test_log.py`

 * *Files identical despite different names*

