# Comparing `tmp/redmage-0.2.1.tar.gz` & `tmp/redmage-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.2.1.tar", max compression
+gzip compressed data, was "redmage-0.2.2.tar", max compression
```

## Comparing `redmage-0.2.1.tar` & `redmage-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.1/LICENSE
--rw-r--r--   0        0        0    14693 2023-07-11 00:43:29.450794 redmage-0.2.1/README.md
--rw-r--r--   0        0        0      660 2023-07-11 00:51:16.382615 redmage-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.1/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.1/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.1/redmage/convertors.py
--rw-r--r--   0        0        0     7766 2023-07-11 00:48:25.487066 redmage-0.2.1/redmage/core.py
--rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.1/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.1/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.1/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.1/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.1/redmage/triggers.py
--rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.2.1/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.1/redmage/utils.py
--rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.2/LICENSE
+-rw-r--r--   0        0        0    15783 2023-07-11 01:23:41.893511 redmage-0.2.2/README.md
+-rw-r--r--   0        0        0      660 2023-07-11 01:13:54.453551 redmage-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.2/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.2/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.2/redmage/convertors.py
+-rw-r--r--   0        0        0     8245 2023-07-11 01:06:21.337049 redmage-0.2.2/redmage/core.py
+-rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.2/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.2/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.2/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.2/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.2/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.2.2/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.2/redmage/utils.py
+-rw-r--r--   0        0        0    16484 1970-01-01 00:00:00.000000 redmage-0.2.2/PKG-INFO
```

### Comparing `redmage-0.2.1/LICENSE` & `redmage-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/README.md` & `redmage-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 
 At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
 
 ```
 uvicorn <module>:<filename>:app.starlette
 ```
 
+### Application Options
+
+You can pass the following keyword arguments to the Redmage constructor which  work as proxies to the underlying Starlette app.
+
+* debug
+* middleware
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
@@ -140,14 +146,15 @@
 | keyword     | htmx attribute                       | type           | default             | documentation | notes                              |
 |-------------|--------------------------------------|----------------|---------------------|---------------|------------------------------------|
 | trigger     | hx-trigger                           | str or Trigger | None                |               | See Trigger section below          |
 | swap        | hx-swap                              | str            | HTMXSwap.OUTER_HTML |               | redmage.types.HTMXSwap enum        |
 | swap_oob    | hx-swap-oob                          | bool           | False               |               |                                    |
 | confirm     | hx-confirm                           | bool           | False               |               |                                    |
 | boost       | hx-boost                             | bool           | False               |               |                                    |
+| on          | hx-on                                | str            | None                |               |                                    |
 | indicator   | N/A                                  | bool           | False               |               |                                    |
 | target      | hx-target, hx-\<method\>             | Target         | None                |               | See Target section below           |
 | click       | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | submit      | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | change      | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | mouse_over  | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | mouse_enter | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
@@ -231,14 +238,43 @@
     @Target.post
     def set_count(self, count: int):
         self.count = count
 ```
 
 When the button is clicked an HTTP POST request is issued to our application. The **set_count** method is ran, updating the component state, and the component is re-rendered and swapped into the DOM.
 
+By default, if the target method returns **None** then **self** is rendered. We could also explicitly return self, another component, or a tuple of components (this can be useful in conjunction with out of bounds swaps).
+
+### Options
+
+A target method can also return a dictionary of options to alter the response. It supports the following keys:
+
+* headers (dict[str: str])
+
+```
+from redmage import Target
+
+
+class ClickComponent(Component):
+
+    def __init__(self):
+        self.count = 0
+
+    def render(self):
+        return Button(
+            self.count,
+            target=self.set_count(self.count + 1)
+        )
+
+    @Target.post
+    def set_count(self, count: int):
+        self.count = count
+        return self {"headers": {"HX-Location": "/changeup"}}
+```
+
 ### Target method arguments
 
 All of the arguments of a render method, except **self**, require type hints so that Redmage can build a route. Positional or keyword (and keyword only) arguments are added to the route as path arguments or query parameters respectively.
 
 If the request has a body, the first argument must be a [positional only argument](https://peps.python.org/pep-0570/). It's type must be a class that de-serializes the body by passing the fields as keyword arguments to it's constructor, like a dataclass.
 
 ```
```

### Comparing `redmage-0.2.1/pyproject.toml` & `redmage-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.2.1"
+version = "0.2.2"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.2.1/redmage/components.py` & `redmage-0.2.2/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/redmage/convertors.py` & `redmage-0.2.2/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/redmage/core.py` & `redmage-0.2.2/redmage/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,23 @@
                 )
             else:
                 components = fn(
                     instance,
                     **{**comp_params, **comp_query_params},
                 )
             if isinstance(components, tuple):
+                # if the last element in the tuple is a dict
+                # then it's an options dict which can contain headers
+                if isinstance(components[-1], dict):
+                    options = components[-1]
+                    headers = options.get("headers", {})
+                    components = components[:-1]
+                    return HTMLResponse(
+                        "\n".join([str(c) for c in components]), headers=headers
+                    )
                 return HTMLResponse("\n".join([str(c) for c in components]))
             elif components:
                 return HTMLResponse(str(components))
             return HTMLResponse(str(instance))
 
         return route_function
```

### Comparing `redmage-0.2.1/redmage/elements.py` & `redmage-0.2.2/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/redmage/targets.py` & `redmage-0.2.2/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/redmage/triggers.py` & `redmage-0.2.2/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/redmage/utils.py` & `redmage-0.2.2/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.1/PKG-INFO` & `redmage-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.2.1
+Version: 0.2.2
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -87,14 +87,20 @@
 
 At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
 
 ```
 uvicorn <module>:<filename>:app.starlette
 ```
 
+### Application Options
+
+You can pass the following keyword arguments to the Redmage constructor which  work as proxies to the underlying Starlette app.
+
+* debug
+* middleware
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
@@ -159,14 +165,15 @@
 | keyword     | htmx attribute                       | type           | default             | documentation | notes                              |
 |-------------|--------------------------------------|----------------|---------------------|---------------|------------------------------------|
 | trigger     | hx-trigger                           | str or Trigger | None                |               | See Trigger section below          |
 | swap        | hx-swap                              | str            | HTMXSwap.OUTER_HTML |               | redmage.types.HTMXSwap enum        |
 | swap_oob    | hx-swap-oob                          | bool           | False               |               |                                    |
 | confirm     | hx-confirm                           | bool           | False               |               |                                    |
 | boost       | hx-boost                             | bool           | False               |               |                                    |
+| on          | hx-on                                | str            | None                |               |                                    |
 | indicator   | N/A                                  | bool           | False               |               |                                    |
 | target      | hx-target, hx-\<method\>             | Target         | None                |               | See Target section below           |
 | click       | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | submit      | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | change      | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | mouse_over  | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
 | mouse_enter | hx-target, hx-\<method\>, hx-trigger | Target         | None                |               | See Trigger keywords section below |
@@ -250,14 +257,43 @@
     @Target.post
     def set_count(self, count: int):
         self.count = count
 ```
 
 When the button is clicked an HTTP POST request is issued to our application. The **set_count** method is ran, updating the component state, and the component is re-rendered and swapped into the DOM.
 
+By default, if the target method returns **None** then **self** is rendered. We could also explicitly return self, another component, or a tuple of components (this can be useful in conjunction with out of bounds swaps).
+
+### Options
+
+A target method can also return a dictionary of options to alter the response. It supports the following keys:
+
+* headers (dict[str: str])
+
+```
+from redmage import Target
+
+
+class ClickComponent(Component):
+
+    def __init__(self):
+        self.count = 0
+
+    def render(self):
+        return Button(
+            self.count,
+            target=self.set_count(self.count + 1)
+        )
+
+    @Target.post
+    def set_count(self, count: int):
+        self.count = count
+        return self {"headers": {"HX-Location": "/changeup"}}
+```
+
 ### Target method arguments
 
 All of the arguments of a render method, except **self**, require type hints so that Redmage can build a route. Positional or keyword (and keyword only) arguments are added to the route as path arguments or query parameters respectively.
 
 If the request has a body, the first argument must be a [positional only argument](https://peps.python.org/pep-0570/). It's type must be a class that de-serializes the body by passing the fields as keyword arguments to it's constructor, like a dataclass.
 
 ```
```

