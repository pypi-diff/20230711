# Comparing `tmp/redmage-0.2.3.tar.gz` & `tmp/redmage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.2.3.tar", max compression
+gzip compressed data, was "redmage-0.3.0.tar", max compression
```

## Comparing `redmage-0.2.3.tar` & `redmage-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.3/LICENSE
--rw-r--r--   0        0        0    15783 2023-07-11 01:23:41.893511 redmage-0.2.3/README.md
--rw-r--r--   0        0        0      660 2023-07-11 04:05:48.216558 redmage-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.3/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-07-11 04:05:32.672334 redmage-0.2.3/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.3/redmage/convertors.py
--rw-r--r--   0        0        0     8267 2023-07-11 04:03:53.117794 redmage-0.2.3/redmage/core.py
--rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.3/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.3/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.3/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.3/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.3/redmage/triggers.py
--rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.2.3/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.3/redmage/utils.py
--rw-r--r--   0        0        0    16484 1970-01-01 00:00:00.000000 redmage-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.3.0/LICENSE
+-rw-r--r--   0        0        0    15237 2023-07-11 04:23:19.514090 redmage-0.3.0/README.md
+-rw-r--r--   0        0        0      660 2023-07-11 04:17:59.610235 redmage-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.3.0/redmage/__init__.py
+-rw-r--r--   0        0        0     6844 2023-07-11 04:20:48.549197 redmage-0.3.0/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.3.0/redmage/convertors.py
+-rw-r--r--   0        0        0     7832 2023-07-11 04:19:56.895119 redmage-0.3.0/redmage/core.py
+-rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.3.0/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.3.0/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.3.0/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.3.0/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.3.0/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.3.0/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.3.0/redmage/utils.py
+-rw-r--r--   0        0        0    15938 1970-01-01 00:00:00.000000 redmage-0.3.0/PKG-INFO
```

### Comparing `redmage-0.2.3/LICENSE` & `redmage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/README.md` & `redmage-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -240,41 +240,14 @@
         self.count = count
 ```
 
 When the button is clicked an HTTP POST request is issued to our application. The **set_count** method is ran, updating the component state, and the component is re-rendered and swapped into the DOM.
 
 By default, if the target method returns **None** then **self** is rendered. We could also explicitly return self, another component, or a tuple of components (this can be useful in conjunction with out of bounds swaps).
 
-### Options
-
-A target method can also return a dictionary of options to alter the response. It supports the following keys:
-
-* headers (dict[str: str])
-
-```
-from redmage import Target
-
-
-class ClickComponent(Component):
-
-    def __init__(self):
-        self.count = 0
-
-    def render(self):
-        return Button(
-            self.count,
-            target=self.set_count(self.count + 1)
-        )
-
-    @Target.post
-    def set_count(self, count: int):
-        self.count = count
-        return self {"headers": {"HX-Location": "/changeup"}}
-```
-
 ### Target method arguments
 
 All of the arguments of a render method, except **self**, require type hints so that Redmage can build a route. Positional or keyword (and keyword only) arguments are added to the route as path arguments or query parameters respectively.
 
 If the request has a body, the first argument must be a [positional only argument](https://peps.python.org/pep-0570/). It's type must be a class that de-serializes the body by passing the fields as keyword arguments to it's constructor, like a dataclass.
 
 ```
```

### Comparing `redmage-0.2.3/pyproject.toml` & `redmage-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.2.3"
+version = "0.3.0"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.2.3/redmage/components.py` & `redmage-0.3.0/redmage/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 from inspect import Parameter, signature
 from typing import Any, Dict, Optional
 from typing import OrderedDict as OrderedDictType
 from typing import Tuple
 from uuid import uuid1
 
 from starlette.convertors import CONVERTOR_TYPES as starlette_convertors
+from starlette.responses import HTMLResponse
 
 from .utils import group_signature_param_by_kind
 
 logger = logging.getLogger("redmage")
 
 
 class Component(ABC):
     app: "Redmage"  # type: ignore
     render_extensions: Dict[str, Any] = {}
 
     def __init_subclass__(cls, routes: Optional[Tuple[str]] = None, **kwargs: Any):
         super().__init_subclass__(**kwargs)
         cls.app.register_component(cls, routes=routes)
 
+    @staticmethod
+    def build_response(content: Any) -> HTMLResponse:
+        return HTMLResponse(content)
+
     @classmethod
     def set_app(cls, app: "Redmage") -> None:  # type: ignore
         cls.app = app
 
     @classmethod
     def add_render_extension(cls, **kwargs: Any) -> None:
         for key, value in kwargs.items():
```

### Comparing `redmage-0.2.3/redmage/convertors.py` & `redmage-0.3.0/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/redmage/core.py` & `redmage-0.3.0/redmage/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ) -> None:
         self.components.append((cls, routes))
 
     def _get_explicit_route_function(self, cls: ComponentClass) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
             attrs = {**request.path_params, **request.query_params}
             instance = cls(**attrs)
-            return HTMLResponse(str(instance))
+            return instance.build_response(str(instance))
 
         return route_function
 
     def _get_route_function(
         self, cls: ComponentClass, name: str, fn: Callable
     ) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
@@ -101,27 +101,18 @@
                 )
             else:
                 components = fn(
                     instance,
                     **{**comp_params, **comp_query_params},
                 )
             if isinstance(components, tuple):
-                # if the last element in the tuple is a dict
-                # then it's an options dict which can contain headers
-                if isinstance(components[-1], dict):
-                    options = components[-1]
-                    headers = options.get("headers", {})
-                    components = components[:-1]
-                    return HTMLResponse(
-                        "\n".join([str(c) for c in components]), headers=headers
-                    )
-                return HTMLResponse("\n".join([str(c) for c in components]))
+                return instance.build_response("\n".join([str(c) for c in components]))
             elif components:
-                return HTMLResponse(str(components))
-            return HTMLResponse(str(instance))
+                return instance.build_response(str(components))
+            return instance.build_response(str(instance))
 
         return route_function
 
     def _convert_value(self, key: str, value: str, fn: Callable) -> Any:
         params = signature(fn).parameters
         if key in params:
             ann = (
```

### Comparing `redmage-0.2.3/redmage/elements.py` & `redmage-0.3.0/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/redmage/targets.py` & `redmage-0.3.0/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/redmage/triggers.py` & `redmage-0.3.0/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/redmage/types.py` & `redmage-0.3.0/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/redmage/utils.py` & `redmage-0.3.0/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.3/PKG-INFO` & `redmage-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.2.3
+Version: 0.3.0
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -259,41 +259,14 @@
         self.count = count
 ```
 
 When the button is clicked an HTTP POST request is issued to our application. The **set_count** method is ran, updating the component state, and the component is re-rendered and swapped into the DOM.
 
 By default, if the target method returns **None** then **self** is rendered. We could also explicitly return self, another component, or a tuple of components (this can be useful in conjunction with out of bounds swaps).
 
-### Options
-
-A target method can also return a dictionary of options to alter the response. It supports the following keys:
-
-* headers (dict[str: str])
-
-```
-from redmage import Target
-
-
-class ClickComponent(Component):
-
-    def __init__(self):
-        self.count = 0
-
-    def render(self):
-        return Button(
-            self.count,
-            target=self.set_count(self.count + 1)
-        )
-
-    @Target.post
-    def set_count(self, count: int):
-        self.count = count
-        return self {"headers": {"HX-Location": "/changeup"}}
-```
-
 ### Target method arguments
 
 All of the arguments of a render method, except **self**, require type hints so that Redmage can build a route. Positional or keyword (and keyword only) arguments are added to the route as path arguments or query parameters respectively.
 
 If the request has a body, the first argument must be a [positional only argument](https://peps.python.org/pep-0570/). It's type must be a class that de-serializes the body by passing the fields as keyword arguments to it's constructor, like a dataclass.
 
 ```
```

