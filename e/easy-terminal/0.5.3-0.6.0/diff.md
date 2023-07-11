# Comparing `tmp/easy-terminal-0.5.3.tar.gz` & `tmp/easy-terminal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-terminal-0.5.3.tar", last modified: Wed Feb 15 00:13:58 2023, max compression
+gzip compressed data, was "easy-terminal-0.6.0.tar", last modified: Tue Jul 11 09:31:06 2023, max compression
```

## Comparing `easy-terminal-0.5.3.tar` & `easy-terminal-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 00:13:58.314874 easy-terminal-0.5.3/
--rw-rw-rw-   0        0        0     1064 2023-02-13 00:28:35.000000 easy-terminal-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     2375 2023-02-15 00:13:58.314874 easy-terminal-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-02-14 21:05:44.000000 easy-terminal-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 00:13:58.314874 easy-terminal-0.5.3/easy_terminal/
--rw-rw-rw-   0        0        0       38 2023-02-13 00:28:36.000000 easy-terminal-0.5.3/easy_terminal/__init__.py
--rw-rw-rw-   0        0        0     6038 2023-02-13 00:36:17.000000 easy-terminal-0.5.3/easy_terminal/terminal.py
-drwxrwxrwx   0        0        0        0 2023-02-15 00:13:58.314874 easy-terminal-0.5.3/easy_terminal.egg-info/
--rw-rw-rw-   0        0        0     2375 2023-02-15 00:13:58.000000 easy-terminal-0.5.3/easy_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-02-15 00:13:58.000000 easy-terminal-0.5.3/easy_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 00:13:58.000000 easy-terminal-0.5.3/easy_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-02-15 00:13:58.000000 easy-terminal-0.5.3/easy_terminal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-15 00:13:58.000000 easy-terminal-0.5.3/easy_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 00:13:58.314874 easy-terminal-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1233 2023-02-15 00:13:43.000000 easy-terminal-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:31:06.056959 easy-terminal-0.6.0/
+-rw-rw-rw-   0        0        0     1064 2023-02-14 21:06:57.000000 easy-terminal-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2334 2023-07-11 09:31:06.056959 easy-terminal-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1749 2023-02-14 21:06:57.000000 easy-terminal-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 09:31:06.046397 easy-terminal-0.6.0/easy_terminal/
+-rw-rw-rw-   0        0        0       38 2023-02-14 21:06:57.000000 easy-terminal-0.6.0/easy_terminal/__init__.py
+-rw-rw-rw-   0        0        0     6254 2023-07-11 09:30:20.000000 easy-terminal-0.6.0/easy_terminal/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:31:06.055450 easy-terminal-0.6.0/easy_terminal.egg-info/
+-rw-rw-rw-   0        0        0     2334 2023-07-11 09:31:05.000000 easy-terminal-0.6.0/easy_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-11 09:31:05.000000 easy-terminal-0.6.0/easy_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:31:05.000000 easy-terminal-0.6.0/easy_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 09:31:05.000000 easy-terminal-0.6.0/easy_terminal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 09:31:05.000000 easy-terminal-0.6.0/easy_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:31:06.057949 easy-terminal-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-07-11 09:30:43.000000 easy-terminal-0.6.0/setup.py
```

### Comparing `easy-terminal-0.5.3/LICENSE` & `easy-terminal-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.5.3/PKG-INFO` & `easy-terminal-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.5.3
-Summary: A tool that help convert function into terminal command (sync and async)
-Home-page: https://github.com/ThePhoenix78/easy_terminal
+Version: 0.6.0
+Summary: A tool that help using python function into terminal
+Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
-Keywords: wrapper,event,terminal,cmd,command,command-line
+Keywords: wrapper,event,terminal,cmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # easy-terminal
```

### Comparing `easy-terminal-0.5.3/README.md` & `easy-terminal-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.5.3/easy_terminal/terminal.py` & `easy-terminal-0.6.0/easy_terminal/terminal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from threading import Thread
 from easy_events import Events, AsyncEvents, Parameters
-import asyncio, time, gc
+import asyncio, time, gc, copy
 
 
 class Debug():
     def __init__(self):
         self.sync = Events(first_parameter_object=False)
         self.asyn = AsyncEvents(first_parameter_object=False)
         self.run = True
@@ -16,16 +16,23 @@
             if isinstance(elem, dict) and f"__main__.{object}" in str(elem):
                 return elem.get(object)
 
     def get_object(self, object: str):
         for elem in gc.get_objects():
             if isinstance(elem, dict) and object in str(elem):
                 val = elem.get(object)
-                if "__main__." in str(val):
-                    return val
+                if not val:
+                    continue
+
+                if "<class __main__." in str(val):
+                    return val, "__main__."
+
+                elif "<class " in str(val):
+                    return val, str(val)[8:str(val).index(".", 1)+1]
+
 
     def analyse_input(self, command: str):
         result = []
         base = None
         method = None
         mid = None
 
@@ -54,32 +61,33 @@
             if not command:
                 continue
 
             is_class = self.analyse_input(command)
             command = Parameters(command)
 
             if is_class:
-                event_type = str(is_class[0]).split("__main__.")[1]
+                event_type = str(is_class[0][0]).split(is_class[0][1])[1]
 
                 if " " in event_type:
                     event_type = event_type.split(" ")[0]
+
                 event_type = event_type.replace("'>", "")
 
                 sync = self.sync.grab_event(is_class[-1], event_type)
                 asyn = self.asyn.grab_event(is_class[-1], event_type)
 
             else:
                 sync = self.sync.grab_event(command._event, None)
                 asyn = self.asyn.grab_event(command._event, None)
 
             if (sync or asyn) and is_class:
-                event = getattr(is_class[0], is_class[1])
+                event = getattr(is_class[0][0], is_class[1])
 
                 command._parameters = command._parameters.split()
-                command._parameters.insert(0, is_class[0])
+                command._parameters.insert(0, is_class[0][0])
                 dico = self.sync.build_arguments(event, command._parameters)
 
                 if "__main__" in str(event):
                     del(dico["self"])
 
                 if asyn:
                     Thread(target=self._execute_async_class, args=[event, dico]).start()
@@ -110,15 +118,15 @@
     def _execute_async_class(self, event: callable, parameters: dict):
         asyncio.run(event(**parameters))
 
     def _execute_class(self, event: callable, parameters: dict):
         event(**parameters)
 
     def _execute_async(self, command):
-        asyncio.run(self.asyn.trigger_run(command, None))
+        asyncio.run(self.asyn.trigger(command, None))
 
     def _execute(self, command):
         self.sync.trigger(command, None)
 
     def stop(self):
         self.run = False
```

### Comparing `easy-terminal-0.5.3/easy_terminal.egg-info/PKG-INFO` & `easy-terminal-0.6.0/easy_terminal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.5.3
-Summary: A tool that help convert function into terminal command (sync and async)
-Home-page: https://github.com/ThePhoenix78/easy_terminal
+Version: 0.6.0
+Summary: A tool that help using python function into terminal
+Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
-Keywords: wrapper,event,terminal,cmd,command,command-line
+Keywords: wrapper,event,terminal,cmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # easy-terminal
```

### Comparing `easy-terminal-0.5.3/setup.py` & `easy-terminal-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='easy-terminal',
-    version="0.5.3",
-    url='https://github.com/ThePhoenix78/easy_terminal',
+    version="0.6.0",
+    url='https://github.com/ThePhoenix78/easy-terminal',
     download_url='https://github.com/ThePhoenix78/easy-terminal/tarball/master',
     license='MIT',
     author='ThePhoenix78',
     author_email='thephoenix788@gmail.com',
-    description='A tool that help convert function into terminal command (sync and async)',
+    description='A tool that help using python function into terminal',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=[
         "wrapper",
         "event",
         "terminal",
-        "cmd",
-        "command",
-        "command-line"
+        "cmd"
     ],
     install_requires=[
-        "easy-events>=2.3.0"
+        "easy-events>=2.9.0"
     ],
     setup_requires=[
         'wheel'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

