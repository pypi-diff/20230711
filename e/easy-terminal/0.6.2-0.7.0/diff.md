# Comparing `tmp/easy-terminal-0.6.2.tar.gz` & `tmp/easy-terminal-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-terminal-0.6.2.tar", last modified: Tue Jul 11 10:00:58 2023, max compression
+gzip compressed data, was "easy-terminal-0.7.0.tar", last modified: Tue Jul 11 10:24:26 2023, max compression
```

## Comparing `easy-terminal-0.6.2.tar` & `easy-terminal-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.375617 easy-terminal-0.6.2/
--rw-rw-rw-   0        0        0     1064 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     2334 2023-07-11 10:00:58.375617 easy-terminal-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.367983 easy-terminal-0.6.2/easy_terminal/
--rw-rw-rw-   0        0        0       38 2023-02-14 21:06:57.000000 easy-terminal-0.6.2/easy_terminal/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-07-11 10:00:40.000000 easy-terminal-0.6.2/easy_terminal/terminal.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:00:58.374620 easy-terminal-0.6.2/easy_terminal.egg-info/
--rw-rw-rw-   0        0        0     2334 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 10:00:58.000000 easy-terminal-0.6.2/easy_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 10:00:58.376613 easy-terminal-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-07-11 10:00:49.000000 easy-terminal-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:24:26.047345 easy-terminal-0.7.0/
+-rw-rw-rw-   0        0        0     1064 2023-02-14 21:06:57.000000 easy-terminal-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2334 2023-07-11 10:24:26.047345 easy-terminal-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1749 2023-02-14 21:06:57.000000 easy-terminal-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:24:26.039777 easy-terminal-0.7.0/easy_terminal/
+-rw-rw-rw-   0        0        0       47 2023-07-11 10:23:48.000000 easy-terminal-0.7.0/easy_terminal/__init__.py
+-rw-rw-rw-   0        0        0     6362 2023-07-11 10:23:38.000000 easy-terminal-0.7.0/easy_terminal/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:24:26.046269 easy-terminal-0.7.0/easy_terminal.egg-info/
+-rw-rw-rw-   0        0        0     2334 2023-07-11 10:24:25.000000 easy-terminal-0.7.0/easy_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-11 10:24:25.000000 easy-terminal-0.7.0/easy_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:24:25.000000 easy-terminal-0.7.0/easy_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 10:24:25.000000 easy-terminal-0.7.0/easy_terminal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 10:24:25.000000 easy-terminal-0.7.0/easy_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:24:26.048337 easy-terminal-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-07-11 10:24:16.000000 easy-terminal-0.7.0/setup.py
```

### Comparing `easy-terminal-0.6.2/LICENSE` & `easy-terminal-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.6.2/PKG-INFO` & `easy-terminal-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.6.2
+Version: 0.7.0
 Summary: A tool that help using python function into terminal
 Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,terminal,cmd
```

### Comparing `easy-terminal-0.6.2/README.md` & `easy-terminal-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `easy-terminal-0.6.2/easy_terminal/terminal.py` & `easy-terminal-0.7.0/easy_terminal/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,74 +52,72 @@
         if not base:
             return
 
         return [base, mid, method]
 
     def _inputs(self):
         while self.run:
-            command = input("> ")
-
-            if not command:
-                continue
-
-            is_class = self.analyse_input(command)
-            command = Parameters(command)
+            self._trigger(input("> "))
+            time.sleep(.1)
 
-            if is_class:
-                event_type = str(is_class[0][0]).split(is_class[0][1])[1]
+    def _trigger(self, command: str = None):
+        if not command:
+            return
 
-                if " " in event_type:
-                    event_type = event_type.split(" ")[0]
+        is_class = self.analyse_input(command)
+        command = Parameters(command)
 
-                event_type = event_type.replace("'>", "")
+        if is_class:
+            event_type = str(is_class[0][0]).split(is_class[0][1])[1]
 
-                print(event_type)
+            if " " in event_type:
+                event_type = event_type.split(" ")[0]
 
-                sync = self.sync.grab_event(is_class[-1], event_type)
-                asyn = self.asyn.grab_event(is_class[-1], event_type)
+            event_type = event_type.replace("'>", "")
 
-            else:
-                sync = self.sync.grab_event(command._event, None)
-                asyn = self.asyn.grab_event(command._event, None)
+            sync = self.sync.grab_event(is_class[-1], event_type)
+            asyn = self.asyn.grab_event(is_class[-1], event_type)
 
-            if (sync or asyn) and is_class:
-                event = getattr(is_class[0][0], is_class[1])
+        else:
+            sync = self.sync.grab_event(command._event, None)
+            asyn = self.asyn.grab_event(command._event, None)
 
-                command._parameters = command._parameters.split()
-                command._parameters.insert(0, is_class[0][0])
-                dico = self.sync.build_arguments(event, command._parameters)
+        if (sync or asyn) and is_class:
+            event = getattr(is_class[0][0], is_class[1])
 
-                if "__main__" in str(event):
-                    del(dico["self"])
+            command._parameters = command._parameters.split()
+            command._parameters.insert(0, is_class[0][0])
+            dico = self.sync.build_arguments(event, command._parameters)
 
-                if asyn:
-                    Thread(target=self._execute_async_class, args=[event, dico]).start()
-                elif sync:
-                    Thread(target=self._execute_class, args=[event, dico]).start()
+            if "__main__" in str(event):
+                del(dico["self"])
 
-            elif asyn:
-                Thread(target=self._execute_async, args=[command]).start()
+            if asyn:
+                Thread(target=self._execute_async_class, args=[event, dico]).start()
             elif sync:
-                Thread(target=self._execute, args=[command]).start()
+                Thread(target=self._execute_class, args=[event, dico]).start()
 
-            elif self.main_function:
-                command._parameters = command._parameters.split()
-                command._parameters.insert(0, command._event)
-
-                if self.main_function == "sync":
-                    event = self.sync.get_events_type("__main")[0].event
-                    dico = self.sync.build_arguments(event, command._parameters)
-                    Thread(target=self._execute_class, args=[event, dico]).start()
-
-                elif self.main_function == "async":
-                    event = self.asyn.get_events_type("__main")[0].event
-                    dico = self.sync.build_arguments(event, command._parameters)
-                    Thread(target=self._execute_async_class, args=[event, dico]).start()
+        elif asyn:
+            Thread(target=self._execute_async, args=[command]).start()
+        elif sync:
+            Thread(target=self._execute, args=[command]).start()
+
+        elif self.main_function:
+            command._parameters = command._parameters.split()
+            command._parameters.insert(0, command._event)
 
-            time.sleep(.1)
+            if self.main_function == "sync":
+                event = self.sync.get_events_type("__main")[0].event
+                dico = self.sync.build_arguments(event, command._parameters)
+                Thread(target=self._execute_class, args=[event, dico]).start()
+
+            elif self.main_function == "async":
+                event = self.asyn.get_events_type("__main")[0].event
+                dico = self.sync.build_arguments(event, command._parameters)
+                Thread(target=self._execute_async_class, args=[event, dico]).start()
 
     def _execute_async_class(self, event: callable, parameters: dict):
         try:
             asyncio.run(event(**parameters))
         except Exception:
             asyncio.run(event())
 
@@ -180,14 +178,18 @@
     def add_main(func):
         _cmd.main(callback=func)
         return func
 
     return add_main
 
 
+def trigger(command: str = None):
+    return _cmd._trigger(command)
+
+
 if __name__ == "__main__":
 
     class A:
         def __init__(self, name="Test"):
             self.name = name
 
         @terminal()
```

### Comparing `easy-terminal-0.6.2/easy_terminal.egg-info/PKG-INFO` & `easy-terminal-0.7.0/easy_terminal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-terminal
-Version: 0.6.2
+Version: 0.7.0
 Summary: A tool that help using python function into terminal
 Home-page: https://github.com/ThePhoenix78/easy-terminal
 Download-URL: https://github.com/ThePhoenix78/easy-terminal/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,terminal,cmd
```

### Comparing `easy-terminal-0.6.2/setup.py` & `easy-terminal-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='easy-terminal',
-    version="0.6.2",
+    version="0.7.0",
     url='https://github.com/ThePhoenix78/easy-terminal',
     download_url='https://github.com/ThePhoenix78/easy-terminal/tarball/master',
     license='MIT',
     author='ThePhoenix78',
     author_email='thephoenix788@gmail.com',
     description='A tool that help using python function into terminal',
     long_description=long_description,
```

