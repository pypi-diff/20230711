# Comparing `tmp/logutils_serpucga-0.1.8.tar.gz` & `tmp/logutils_serpucga-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logutils_serpucga-0.1.8.tar", last modified: Fri Jan 20 07:42:42 2023, max compression
+gzip compressed data, was "logutils_serpucga-0.1.9.tar", last modified: Tue Jul 11 10:33:30 2023, max compression
```

## Comparing `logutils_serpucga-0.1.8.tar` & `logutils_serpucga-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-01-20 07:42:42.176305 logutils_serpucga-0.1.8/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      817 2023-01-20 07:42:42.176305 logutils_serpucga-0.1.8/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      516 2022-11-16 09:47:27.000000 logutils_serpucga-0.1.8/README.md
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-01-20 07:42:42.176305 logutils_serpucga-0.1.8/logutils/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     3151 2023-01-20 07:41:58.000000 logutils_serpucga-0.1.8/logutils/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      666 2022-11-16 09:42:02.000000 logutils_serpucga-0.1.8/logutils/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-01-20 07:42:42.176305 logutils_serpucga-0.1.8/logutils_serpucga.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      817 2023-01-20 07:42:42.000000 logutils_serpucga-0.1.8/logutils_serpucga.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      222 2023-01-20 07:42:42.000000 logutils_serpucga-0.1.8/logutils_serpucga.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-01-20 07:42:42.000000 logutils_serpucga-0.1.8/logutils_serpucga.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        9 2023-01-20 07:42:42.000000 logutils_serpucga-0.1.8/logutils_serpucga.egg-info/top_level.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-01-20 07:42:42.176305 logutils_serpucga-0.1.8/setup.cfg
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      940 2022-11-15 09:26:18.000000 logutils_serpucga-0.1.8/setup.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 10:33:30.025486 logutils_serpucga-0.1.9/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      817 2023-07-11 10:33:30.025486 logutils_serpucga-0.1.9/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      516 2022-11-16 09:47:27.000000 logutils_serpucga-0.1.9/README.md
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 10:33:30.021486 logutils_serpucga-0.1.9/logutils/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     3197 2023-07-11 10:31:50.000000 logutils_serpucga-0.1.9/logutils/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      666 2022-11-16 09:42:02.000000 logutils_serpucga-0.1.9/logutils/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 10:33:30.021486 logutils_serpucga-0.1.9/logutils_serpucga.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      817 2023-07-11 10:33:30.000000 logutils_serpucga-0.1.9/logutils_serpucga.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      222 2023-07-11 10:33:30.000000 logutils_serpucga-0.1.9/logutils_serpucga.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-11 10:33:30.000000 logutils_serpucga-0.1.9/logutils_serpucga.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        9 2023-07-11 10:33:30.000000 logutils_serpucga-0.1.9/logutils_serpucga.egg-info/top_level.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-11 10:33:30.025486 logutils_serpucga-0.1.9/setup.cfg
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      940 2022-11-15 09:26:18.000000 logutils_serpucga-0.1.9/setup.py
```

### Comparing `logutils_serpucga-0.1.8/PKG-INFO` & `logutils_serpucga-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logutils_serpucga
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to generate pretty logs quickly using default logging library
 Home-page: https://gitlab.com/Serbaf/logging_utils
 Author: Sergio Puche García
 Author-email: spuche@upv.es
 License: GPL3
 Description-Content-Type: text/markdown
```

### Comparing `logutils_serpucga-0.1.8/README.md` & `logutils_serpucga-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `logutils_serpucga-0.1.8/logutils/__init__.py` & `logutils_serpucga-0.1.9/logutils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 import logging
 from logging.handlers import RotatingFileHandler
 from typing import Optional
 from pathlib import Path
 from logutils.consts import (
     lila,
@@ -62,14 +62,16 @@
     handler_list=["stream"],
     level=logging.INFO,
     propagate=False,
     colored=True,
     filepath: Optional[Path] = None,
 ):
     logger = logging.getLogger(name)
+    if logger.handlers:
+        return logger
     logger.setLevel(logging.DEBUG)
     handlers = []
     if "stream" in handler_list:
         handler = logging.StreamHandler()
         handler.setLevel(level)
         handler.setFormatter(CustomFormatter(colored=colored))
         handlers.append(handler)
```

### Comparing `logutils_serpucga-0.1.8/logutils/consts.py` & `logutils_serpucga-0.1.9/logutils/consts.py`

 * *Files identical despite different names*

### Comparing `logutils_serpucga-0.1.8/logutils_serpucga.egg-info/PKG-INFO` & `logutils_serpucga-0.1.9/logutils_serpucga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logutils-serpucga
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to generate pretty logs quickly using default logging library
 Home-page: https://gitlab.com/Serbaf/logging_utils
 Author: Sergio Puche García
 Author-email: spuche@upv.es
 License: GPL3
 Description-Content-Type: text/markdown
```

### Comparing `logutils_serpucga-0.1.8/setup.py` & `logutils_serpucga-0.1.9/setup.py`

 * *Files identical despite different names*

