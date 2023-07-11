# Comparing `tmp/phanos-0.0.5.tar.gz` & `tmp/phanos-0.0.6.tar.gz`

## Comparing `phanos-0.0.5.tar` & `phanos-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.5/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.5/Pipfile.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.5/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/log.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/metrics.py
--rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/publisher.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/tree.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.5/test/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.5/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.5/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.5/test/run_tests.py
--rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.5/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.5/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.5/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.5/LICENSE
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.5/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.6/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.6/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/log.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15975 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/publisher.py
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/tree.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.6/test/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.6/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.6/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.6/test/run_tests.py
+-rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.6/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.6/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.6/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.6/PKG-INFO
```

### Comparing `phanos-0.0.5/Pipfile.lock` & `phanos-0.0.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/deactivate/bin/Activate.ps1` & `phanos-0.0.6/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/deactivate/bin/activate` & `phanos-0.0.6/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/deactivate/bin/activate.csh` & `phanos-0.0.6/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/deactivate/bin/activate.fish` & `phanos-0.0.6/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/src/phanos/log.py` & `phanos-0.0.6/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/src/phanos/metrics.py` & `phanos-0.0.6/src/phanos/metrics.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/src/phanos/publisher.py` & `phanos-0.0.6/src/phanos/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,23 +356,23 @@
 
     def add_handler(self, handler: BaseHandler) -> None:
         """Add handler to profiler
 
         :param handler: handler instance
         """
         self._handlers[handler.handler_name] = handler
-        self.debug("handler {handler.handler_name} added to phanos profiler")
+        self.debug(f"handler {handler.handler_name} added to phanos profiler")
 
     def delete_handler(self, handler_name: str) -> None:
         """Delete handler from profiler
 
         :param handler_name: name of handler:
         """
         _ = self._handlers.pop(handler_name, None)
-        self.debug("handler {handler_name} deleted")
+        self.debug(f"handler {handler_name} deleted")
 
     def delete_handlers(self) -> None:
         """delete all handlers"""
         self._handlers.clear()
         self.debug(f"all handlers deleted")
 
     def profile(self, func: typing.Callable) -> typing.Callable:
```

### Comparing `phanos-0.0.5/src/phanos/tree.py` & `phanos-0.0.6/src/phanos/tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,19 +44,47 @@
         """
         child.parent = self
         if self.method is None:  # equivalent of 'self.context != ""' -> i am root
             child.context = (
                 self.get_method_class(child.method) + ":" + child.context
             )  # child.method cannot be None
         else:
-            child.context = self.context + "." + child.context
+            between = self._get_methods_between()
+            if between != "":
+                child.context = self.context + "." + between + "." + child.context
+            else:
+                child.context = self.context + "." + child.context
         self.children.append(child)
         self.debug(f"node {self.context} added child: {child.context}")
         return child
 
+    def _get_methods_between(self) -> str:
+        methods_between = []
+        split_context = self.context.split(".")
+        if len(split_context) == 1:
+            starting_method = self.context.split(":")[-1]
+        else:
+            starting_method = split_context[-1]
+        between = ""
+        if inspect.stack():
+            for item in inspect.stack():
+                if item.function == starting_method:
+                    break
+                if item.function not in [
+                    "<module>",
+                    "inner",
+                    "add_child",
+                    "_get_methods_between",
+                ]:
+                    methods_between.append(item.function)
+            methods_between.reverse()
+            between = ".".join(f"{method}" for method in methods_between)
+
+        return between
+
     def delete_child(self) -> None:
         """Delete first child of node"""
         child = self.children.pop(0)
         child.parent = None
         self.debug(f"node {self.context} deleted child: {child.context}")
 
     def clear_tree(self) -> None:
```

### Comparing `phanos-0.0.5/test/dummy_api.py` & `phanos-0.0.6/test/dummy_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         sleep(0.2)
 
     @phanos_profiler.profile
     def second_access(self):
         self.first_access()
         sleep(0.3)
 
+    def third_access(self):
+        self.second_access()
+
 
 @ns.route("/one")
 class DummyResource(Resource):
     access = DummyDbAccess()
 
     @phanos_profiler.profile
     def get(self):
@@ -51,7 +54,18 @@
 
 app = Flask("TEST")
 api = Api(
     app,
     prefix="/api",
 )
 api.add_namespace(ns)
+
+if __name__ == "__main__":
+    from src.phanos import phanos_profiler
+    from src.phanos.publisher import LoggerHandler
+
+    phanos_profiler.config()
+    handler = LoggerHandler("asd")
+    phanos_profiler.add_handler(handler)
+    print("starting profle")
+    resource = DummyResource()
+    res = resource.get()
```

### Comparing `phanos-0.0.5/test/run_tests.py` & `phanos-0.0.6/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/test/test_metric.py` & `phanos-0.0.6/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/test/testing_data.py` & `phanos-0.0.6/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/.gitignore` & `phanos-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/LICENSE` & `phanos-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/README.md` & `phanos-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.0.5/pyproject.toml` & `phanos-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
```

### Comparing `phanos-0.0.5/PKG-INFO` & `phanos-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

