# Comparing `tmp/styledlogger-0.1.2.tar.gz` & `tmp/styledlogger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.1.2.tar", last modified: Tue Jul 11 15:12:33 2023, max compression
+gzip compressed data, was "styledlogger-0.1.3.tar", last modified: Tue Jul 11 18:56:46 2023, max compression
```

## Comparing `styledlogger-0.1.2.tar` & `styledlogger-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-11 15:12:17.000000 styledlogger-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 15:12:33.586098 styledlogger-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-11 15:12:17.000000 styledlogger-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:12:33.586098 styledlogger-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 15:12:17.000000 styledlogger-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.451903 styledlogger-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-11 18:56:29.000000 styledlogger-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 18:56:46.451903 styledlogger-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-11 18:56:29.000000 styledlogger-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:56:46.451903 styledlogger-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 18:56:29.000000 styledlogger-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.447903 styledlogger-0.1.3/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.451903 styledlogger-0.1.3/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/callbackctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-11 18:56:29.000000 styledlogger-0.1.3/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:46.447903 styledlogger-0.1.3/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 18:56:46.000000 styledlogger-0.1.3/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.1.2/LICENSE` & `styledlogger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/PKG-INFO` & `styledlogger-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
```

### Comparing `styledlogger-0.1.2/README.md` & `styledlogger-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/setup.py` & `styledlogger-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/styledlogger/classes/callback.py` & `styledlogger-0.1.3/styledlogger/classes/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from .callbackctx import CallbackContext
+
 class Callback:
     """
     A callback that can be added to a logger. The callback will be called with the logger name as the first argument and message as the second argument.
 
     :param name:
     The name of the callback. This is used to identify the callback.
 
     :param activation_level:
     The level at which the callback will be called. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
 
     :param callback:
     The callback function. This will be called with the logger name as the first argument, the level as the second and message as the third argument.
     """
 
-    def __init__(self, name: str, activation_level: int, callback: callable):
+    def __init__(self, name: str, activation_levels: int | tuple, callback: callable):
         self.name = name
-        self.activation_level = activation_level
+        self.activation_levels = activation_levels
         self.callback = callback
 
     def run_callback(self, level, message):
-        self.callback(self.name, level, message)
+        self.callback(CallbackContext(self.name, level, message))
 
     def __repr__(self):
-        return f"<Callback name={self.name} activation_level={self.activation_level} callback={self.callback}>"
+        return f"<Callback name={self.name} activation_levels={self.activation_levels} callback={self.callback}>"
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `styledlogger-0.1.2/styledlogger/classes/printcolors.py` & `styledlogger-0.1.3/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/styledlogger/classes/printtypes.py` & `styledlogger-0.1.3/styledlogger/classes/printtypes.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/styledlogger/classes/styleconfig.py` & `styledlogger-0.1.3/styledlogger/classes/styleconfig.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.2/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.1.3/styledlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
```

