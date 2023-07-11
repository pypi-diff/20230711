# Comparing `tmp/easy-terminal-0.6.1.tar.gz` & `tmp/easy-terminal-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-terminal-0.6.1.tar", last modified: Tue Jul 11 09:59:37 2023, max compression
+gzip compressed data, was "easy-terminal-0.6.2.tar", last modified: Tue Jul 11 10:00:58 2023, max compression
```

## Comparing `easy-terminal-0.6.1.tar` & `easy-terminal-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:59:37.961326 easy-terminal-0.6.1/
--rw-rw-rw-   0        0        0     1064 2023-02-14 21:06:57.000000 easy-terminal-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     2334 2023-07-11 09:59:37.959802 easy-terminal-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-02-14 21:06:57.000000 easy-terminal-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 09:59:37.952825 easy-terminal-0.6.1/easy_terminal/
--rw-rw-rw-   0        0        0       38 2023-02-14 21:06:57.000000 easy-terminal-0.6.1/easy_terminal/__init__.py
--rw-rw-rw-   0        0        0     6466 2023-07-11 09:57:43.000000 easy-terminal-0.6.1/easy_terminal/terminal.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:59:37.958806 easy-terminal-0.6.1/easy_terminal.egg-info/
--rw-rw-rw-   0        0        0     2334 2023-07-11 09:59:37.000000 easy-terminal-0.6.1/easy_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-11 09:59:37.000000 easy-terminal-0.6.1/easy_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:59:37.000000 easy-terminal-0.6.1/easy_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-11 09:59:37.000000 easy-terminal-0.6.1/easy_terminal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 09:59:37.000000 easy-terminal-0.6.1/easy_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 09:59:37.961326 easy-terminal-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-07-11 09:59:32.000000 easy-terminal-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.375617 easy-terminal-0.6.2/
+-rw-rw-rw-   0        0        0     1064 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     2334 2023-07-11 10:00:58.375617 easy-terminal-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1749 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.367983 easy-terminal-0.6.2/easy_terminal/
+-rw-rw-rw-   0        0        0       38 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/easy_terminal/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-07-11 10:00:40.000000 easy-terminal-0.6.2/easy_terminal/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.374620 easy-terminal-0.6.2/easy_terminal.egg-info/
+-rw-rw-rw-   0        0        0     2334 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:00:58.376613 easy-terminal-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-07-11 10:00:49.000000 easy-terminal-0.6.2/setup.py
```

### Comparing `easy-terminal-0.6.1/LICENSE` & `easy-terminal-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.6.1/PKG-INFO` & `easy-terminal-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool that help using python function into terminal
 Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,terminal,cmd
```

### Comparing `easy-terminal-0.6.1/README.md` & `easy-terminal-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.6.1/easy_terminal/terminal.py` & `easy-terminal-0.6.2/easy_terminal/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from threading import Thread
 from easy_events import Events, AsyncEvents, Parameters
 import asyncio, time, gc, copy
 
-print("DEBUG")
 
 class Debug():
     def __init__(self):
         self.sync = Events(first_parameter_object=False)
         self.asyn = AsyncEvents(first_parameter_object=False)
         self.run = True
         self.main_function = None
@@ -119,15 +118,15 @@
             time.sleep(.1)
 
     def _execute_async_class(self, event: callable, parameters: dict):
         try:
             asyncio.run(event(**parameters))
         except Exception:
             asyncio.run(event())
-            
+
     def _execute_class(self, event: callable, parameters: dict):
         try:
             event(**parameters)
         except Exception:
             event()
 
     def _execute_async(self, command):
```

### Comparing `easy-terminal-0.6.1/easy_terminal.egg-info/PKG-INFO` & `easy-terminal-0.6.2/easy_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool that help using python function into terminal
 Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,terminal,cmd
```

### Comparing `easy-terminal-0.6.1/setup.py` & `easy-terminal-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='easy-terminal',
-    version="0.6.1",
+    version="0.6.2",
     url='https://github.com/ThePhoenix78/easy-terminal',
     download_url='https://github.com/ThePhoenix78/easy-terminal/tarball/master',
     license='MIT',
     author='ThePhoenix78',
     author_email='thephoenix788@gmail.com',
     description='A tool that help using python function into terminal',
     long_description=long_description,
```

