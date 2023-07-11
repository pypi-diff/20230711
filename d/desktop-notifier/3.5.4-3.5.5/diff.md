# Comparing `tmp/desktop-notifier-3.5.4.tar.gz` & `tmp/desktop-notifier-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.4.tar", last modified: Mon Jul  3 18:47:52 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.5.tar", last modified: Mon Jul 10 20:35:23 2023, max compression
```

## Comparing `desktop-notifier-3.5.4.tar` & `desktop-notifier-3.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.294218 desktop-notifier-3.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:23.210376 desktop-notifier-3.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-10 20:35:10.000000 desktop-notifier-3.5.5/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:23.214377 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-10 20:35:23.000000 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-10 20:35:23.000000 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:35:23.000000 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-10 20:35:23.000000 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 20:35:23.000000 desktop-notifier-3.5.5/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.4/LICENSE` & `desktop-notifier-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/PKG-INFO` & `desktop-notifier-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.4
+Version: 3.5.5
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.4/README.md` & `desktop-notifier-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/pyproject.toml` & `desktop-notifier-3.5.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.4"
+version = "3.5.5"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
```

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/base.py` & `desktop-notifier-3.5.5/src/desktop_notifier/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,22 @@
     Callable,
     Any,
     Deque,
     List,
     Sequence,
 )
 
-from importlib_resources import path as resource_path
+from importlib_resources import files, as_file
 
 
 logger = logging.getLogger(__name__)
 
-PYTHON_ICON_PATH = resource_path("desktop_notifier.resources", "python.png").__enter__()
+PYTHON_ICON_PATH = as_file(
+    files("desktop_notifier.resources").joinpath("python.png")
+).__enter__()
 
 
 class AuthorisationError(Exception):
     """Raised when we are not authorised to send notifications"""
 
 
 class Urgency(Enum):
```

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.5/src/desktop_notifier/dbus.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.5/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.5/src/desktop_notifier/macos.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.5/src/desktop_notifier/macos_legacy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.5/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/main.py` & `desktop-notifier-3.5.5/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/resources/python.png` & `desktop-notifier-3.5.5/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.5/src/desktop_notifier/winrt.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.5/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.4
+Version: 3.5.5
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.4/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.5/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

