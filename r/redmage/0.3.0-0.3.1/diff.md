# Comparing `tmp/redmage-0.3.0.tar.gz` & `tmp/redmage-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.3.0.tar", max compression
+gzip compressed data, was "redmage-0.3.1.tar", max compression
```

## Comparing `redmage-0.3.0.tar` & `redmage-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.3.0/LICENSE
--rw-r--r--   0        0        0    15237 2023-07-11 04:23:19.514090 redmage-0.3.0/README.md
--rw-r--r--   0        0        0      660 2023-07-11 04:17:59.610235 redmage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.3.0/redmage/__init__.py
--rw-r--r--   0        0        0     6844 2023-07-11 04:20:48.549197 redmage-0.3.0/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.3.0/redmage/convertors.py
--rw-r--r--   0        0        0     7832 2023-07-11 04:19:56.895119 redmage-0.3.0/redmage/core.py
--rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.3.0/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.3.0/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.3.0/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.3.0/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.3.0/redmage/triggers.py
--rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.3.0/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.3.0/redmage/utils.py
--rw-r--r--   0        0        0    15938 1970-01-01 00:00:00.000000 redmage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.3.1/LICENSE
+-rw-r--r--   0        0        0    15237 2023-07-11 04:23:19.514090 redmage-0.3.1/README.md
+-rw-r--r--   0        0        0      660 2023-07-11 04:29:40.809276 redmage-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.3.1/redmage/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-11 04:29:40.810276 redmage-0.3.1/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.3.1/redmage/convertors.py
+-rw-r--r--   0        0        0     7832 2023-07-11 04:19:56.895119 redmage-0.3.1/redmage/core.py
+-rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.3.1/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.3.1/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.3.1/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.3.1/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.3.1/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.3.1/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.3.1/redmage/utils.py
+-rw-r--r--   0        0        0    15938 1970-01-01 00:00:00.000000 redmage-0.3.1/PKG-INFO
```

### Comparing `redmage-0.3.0/LICENSE` & `redmage-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/README.md` & `redmage-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/pyproject.toml` & `redmage-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.3.0"
+version = "0.3.1"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.3.0/redmage/components.py` & `redmage-0.3.1/redmage/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     app: "Redmage"  # type: ignore
     render_extensions: Dict[str, Any] = {}
 
     def __init_subclass__(cls, routes: Optional[Tuple[str]] = None, **kwargs: Any):
         super().__init_subclass__(**kwargs)
         cls.app.register_component(cls, routes=routes)
 
-    @staticmethod
-    def build_response(content: Any) -> HTMLResponse:
+    def build_response(self, content: Any) -> HTMLResponse:
         return HTMLResponse(content)
 
     @classmethod
     def set_app(cls, app: "Redmage") -> None:  # type: ignore
         cls.app = app
 
     @classmethod
```

### Comparing `redmage-0.3.0/redmage/convertors.py` & `redmage-0.3.1/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/core.py` & `redmage-0.3.1/redmage/core.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/elements.py` & `redmage-0.3.1/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/targets.py` & `redmage-0.3.1/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/triggers.py` & `redmage-0.3.1/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/types.py` & `redmage-0.3.1/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/redmage/utils.py` & `redmage-0.3.1/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.0/PKG-INFO` & `redmage-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.3.0
+Version: 0.3.1
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

