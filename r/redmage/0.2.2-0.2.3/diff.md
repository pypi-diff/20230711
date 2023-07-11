# Comparing `tmp/redmage-0.2.2.tar.gz` & `tmp/redmage-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.2.2.tar", max compression
+gzip compressed data, was "redmage-0.2.3.tar", max compression
```

## Comparing `redmage-0.2.2.tar` & `redmage-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.2/LICENSE
--rw-r--r--   0        0        0    15783 2023-07-11 01:23:41.893511 redmage-0.2.2/README.md
--rw-r--r--   0        0        0      660 2023-07-11 01:13:54.453551 redmage-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.2/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.2/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.2/redmage/convertors.py
--rw-r--r--   0        0        0     8245 2023-07-11 01:06:21.337049 redmage-0.2.2/redmage/core.py
--rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.2/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.2/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.2/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.2/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.2/redmage/triggers.py
--rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.2.2/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.2/redmage/utils.py
--rw-r--r--   0        0        0    16484 1970-01-01 00:00:00.000000 redmage-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.3/LICENSE
+-rw-r--r--   0        0        0    15783 2023-07-11 01:23:41.893511 redmage-0.2.3/README.md
+-rw-r--r--   0        0        0      660 2023-07-11 04:05:48.216558 redmage-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.3/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-07-11 04:05:32.672334 redmage-0.2.3/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.3/redmage/convertors.py
+-rw-r--r--   0        0        0     8267 2023-07-11 04:03:53.117794 redmage-0.2.3/redmage/core.py
+-rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.2.3/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.3/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.3/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.3/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.3/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.2.3/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.3/redmage/utils.py
+-rw-r--r--   0        0        0    16484 1970-01-01 00:00:00.000000 redmage-0.2.3/PKG-INFO
```

### Comparing `redmage-0.2.2/LICENSE` & `redmage-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/README.md` & `redmage-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/pyproject.toml` & `redmage-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.2.2"
+version = "0.2.3"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.2.2/redmage/components.py` & `redmage-0.2.3/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/convertors.py` & `redmage-0.2.3/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/core.py` & `redmage-0.2.3/redmage/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             self.create_routes()
             if self.middleware:
                 self._starlette = Starlette(
                     debug=self.debug,
                     routes=self.routes,
                     middleware=self.middleware,
                 )
-            self._starlette = Starlette(debug=self.debug, routes=self.routes)
+            else:
+                self._starlette = Starlette(debug=self.debug, routes=self.routes)
         return self._starlette
 
     def create_routes(self) -> None:
         for cls, routes in self.components:
             if routes:
                 self._register_routes(cls, routes)
             self._register_targets(cls)
```

### Comparing `redmage-0.2.2/redmage/elements.py` & `redmage-0.2.3/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/targets.py` & `redmage-0.2.3/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/triggers.py` & `redmage-0.2.3/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/types.py` & `redmage-0.2.3/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/redmage/utils.py` & `redmage-0.2.3/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.2.2/PKG-INFO` & `redmage-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.2.2
+Version: 0.2.3
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

