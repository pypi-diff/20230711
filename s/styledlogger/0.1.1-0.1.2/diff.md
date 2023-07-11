# Comparing `tmp/styledlogger-0.1.1.tar.gz` & `tmp/styledlogger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.1.1.tar", last modified: Tue Jul  4 09:17:11 2023, max compression
+gzip compressed data, was "styledlogger-0.1.2.tar", last modified: Tue Jul 11 15:12:33 2023, max compression
```

## Comparing `styledlogger-0.1.1.tar` & `styledlogger-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.591174 styledlogger-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 09:16:56.000000 styledlogger-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-04 09:17:11.591174 styledlogger-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 09:16:56.000000 styledlogger-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:17:11.591174 styledlogger-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 09:16:56.000000 styledlogger-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.587174 styledlogger-0.1.1/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.591174 styledlogger-0.1.1/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.587174 styledlogger-0.1.1/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-11 15:12:17.000000 styledlogger-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 15:12:33.586098 styledlogger-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-11 15:12:17.000000 styledlogger-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:12:33.586098 styledlogger-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 15:12:17.000000 styledlogger-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-11 15:12:17.000000 styledlogger-0.1.2/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:12:33.586098 styledlogger-0.1.2/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:12:33.000000 styledlogger-0.1.2/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.1.1/LICENSE` & `styledlogger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/PKG-INFO` & `styledlogger-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
```

### Comparing `styledlogger-0.1.1/README.md` & `styledlogger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/setup.py` & `styledlogger-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/styledlogger/classes/callback.py` & `styledlogger-0.1.2/styledlogger/classes/callback.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/styledlogger/classes/printcolors.py` & `styledlogger-0.1.2/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/styledlogger/classes/printtypes.py` & `styledlogger-0.1.2/styledlogger/classes/printtypes.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/styledlogger/classes/styleconfig.py` & `styledlogger-0.1.2/styledlogger/classes/styleconfig.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.1/styledlogger/logger.py` & `styledlogger-0.1.2/styledlogger/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from colorama import (
     just_fix_windows_console,
 )
 
 from .classes.styleconfig import StyleConfig
 from .classes.printtypes import PrintType, Debug, Info, Warn, Error, Fatal, System
-from .classes.callback import Callback
+from .classes.callback import Callback as LoggerCallback
 
 just_fix_windows_console()
 
 
 class Logger:
     """
     The main object for logging.
@@ -28,22 +28,34 @@
 
     def set_level(self, level):
         """
         Set the log level. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
         """
         self.level = level
 
-    def add_callback(self, name: str, activation_level, callback: callable):
+    # Create a decorator, which takes in a name, and adds the decorated function to the logger's callbacks
+    def callback(self, name: str, level: int = 1):
         """
-        Add a callback to the logger. The callback will be called with the message as the first argument.
+        Decorator to add a callback to the logger.
+
+        :param name: The name of the callback
+        :param level: The level which the callback will be activated on. Higher levels than the specified level will be activated as well.
+
+        The decorated function should take these parameters:
+        :param name: The name of the logger which called the callback
+        :param level: The level which called the callback
+        :param message: The message which the logger was called with
         """
-        self.callbacks.append(
-            Callback(name=name, activation_level=activation_level, callback=callback)
-        )
-    
+
+        def decorator_function(original_func):
+            self.callbacks.append(LoggerCallback(name, level, original_func))
+            return original_func
+
+        return decorator_function
+
     def remove_callback(self, name: str):
         """
         Remove a callback from the logger.
         """
         for callback in self.callbacks:
             if callback.name == name:
                 self.callbacks.remove(callback)
@@ -87,20 +99,22 @@
 
     def system(self, message):
         """
         Log a system message
         """
         self._log(message, System)
 
-    def _log(self, message, print_type: PrintType):
-
+    def _process_callbacks(self, print_type, message):
         for callback in self.callbacks:
             if callback.activation_level <= print_type.level:
                 callback.run_callback(level=print_type.level, message=message)
 
+    def _log(self, message, print_type: PrintType):
+        self._process_callbacks(print_type, message)
+
         if self.is_muted:
             return
 
         if self.file_path:
             with open(self.file_path, "a+", encoding="utf-8") as file:
                 file.write(
                     self.style_config.style_text_uncolored(
```

### Comparing `styledlogger-0.1.1/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.1.2/styledlogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
```

