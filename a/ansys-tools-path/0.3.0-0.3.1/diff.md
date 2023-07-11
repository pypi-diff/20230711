# Comparing `tmp/ansys_tools_path-0.3.0.tar.gz` & `tmp/ansys_tools_path-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.3.0.tar` & `ansys_tools_path-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1089 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/LICENSE
--rw-r--r--   0        0        0     4692 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/README.rst
--rw-r--r--   0        0        0     1914 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      905 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      677 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    30449 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0        0 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/py.typed
--rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 ansys_tools_path-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-11 07:22:03.030136 ansys_tools_path-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4692 2023-07-11 07:22:03.030136 ansys_tools_path-0.3.1/README.rst
+-rw-r--r--   0        0        0     1914 2023-07-11 07:22:03.034136 ansys_tools_path-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1383 2023-07-11 07:22:03.034136 ansys_tools_path-0.3.1/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      677 2023-07-11 07:22:03.034136 ansys_tools_path-0.3.1/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    30458 2023-07-11 07:22:03.034136 ansys_tools_path-0.3.1/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:22:03.034136 ansys_tools_path-0.3.1/src/ansys/tools/path/py.typed
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 ansys_tools_path-0.3.1/PKG-INFO
```

### Comparing `ansys_tools_path-0.3.0/LICENSE` & `ansys_tools_path-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.3.0/README.rst` & `ansys_tools_path-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.3.0/pyproject.toml` & `ansys_tools_path-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -31,15 +31,15 @@
 ]
 
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
-    "pyfakefs==5.2.2",
+    "pyfakefs==5.2.3",
 ]
 
 doc = [
     "Sphinx==7.0.1",
     "numpydoc==1.5.0",
     "ansys-sphinx-theme==0.9.9",
     "sphinx-copybutton==0.5.2",
```

### Comparing `ansys_tools_path-0.3.0/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.3.1/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.3.0/src/ansys/tools/path/path.py` & `ansys_tools_path-0.3.1/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         ver_str = path[-3:]
         if is_float(ver_str):
             ansys_paths[int(ver_str)] = path
 
     # Testing for ANSYS STUDENT version
     paths = glob(os.path.join(base_path, "ANSYS*", "v*"))
     if not paths:
-        return {}
+        return ansys_paths
 
     for path in paths:
         ver_str = path[-3:]
         if is_float(ver_str):
             ansys_paths[-int(ver_str)] = path
 
     return ansys_paths
```

### Comparing `ansys_tools_path-0.3.0/PKG-INFO` & `ansys_tools_path-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: twine==4.0.2 ; extra == "build"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
-Requires-Dist: pyfakefs==5.2.2 ; extra == "tests"
+Requires-Dist: pyfakefs==5.2.3 ; extra == "tests"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
 Project-URL: Source, https://github.com/ansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: tests
```

