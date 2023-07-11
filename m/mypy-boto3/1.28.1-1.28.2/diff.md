# Comparing `tmp/mypy-boto3-1.28.1.tar.gz` & `tmp/mypy-boto3-1.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-1.28.2.tar", last modified: Tue Jul 11 06:09:51 2023, max compression
```

## Comparing `mypy-boto3-1.28.1.tar` & `mypy-boto3-1.28.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.899385 mypy-boto3-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-07 19:32:38.899385 mypy-boto3-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.887385 mypy-boto3-1.28.1/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:31:47.000000 mypy-boto3-1.28.1/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 19:31:47.000000 mypy-boto3-1.28.1/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 19:31:47.000000 mypy-boto3-1.28.1/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-07-07 19:31:47.000000 mypy-boto3-1.28.1/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105965 2023-07-07 19:31:47.000000 mypy-boto3-1.28.1/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.899385 mypy-boto3-1.28.1/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 19:32:38.000000 mypy-boto3-1.28.1/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.899385 mypy-boto3-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 19:31:45.000000 mypy-boto3-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.550497 mypy-boto3-1.28.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 06:09:51.550497 mypy-boto3-1.28.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.550497 mypy-boto3-1.28.2/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:29.000000 mypy-boto3-1.28.2/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 06:09:29.000000 mypy-boto3-1.28.2/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 06:09:29.000000 mypy-boto3-1.28.2/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-11 06:09:29.000000 mypy-boto3-1.28.2/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105965 2023-07-11 06:09:29.000000 mypy-boto3-1.28.2/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.550497 mypy-boto3-1.28.2/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 06:09:51.000000 mypy-boto3-1.28.2/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:09:51.550497 mypy-boto3-1.28.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-11 06:09:27.000000 mypy-boto3-1.28.2/setup.py
```

### Comparing `mypy-boto3-1.28.1/LICENSE` & `mypy-boto3-1.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.1/PKG-INFO` & `mypy-boto3-1.28.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.28.1
-Summary: Type annotations for boto3 1.28.1 master module generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3 1.28.2 master module generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/1.28.1/index.html)
+[boto3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/1.28.2/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.1/README.md` & `mypy-boto3-1.28.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/1.28.1/index.html)
+[boto3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/1.28.2/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.1/mypy_boto3/boto3_init_stub.py` & `mypy-boto3-1.28.2/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.1/mypy_boto3/boto3_session_stub.py` & `mypy-boto3-1.28.2/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.1/mypy_boto3/main.py` & `mypy-boto3-1.28.2/mypy_boto3/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,20 +110,18 @@
             "mypy-boto3",
         ]
         for submodule in SUBMODULES:
             if submodule.is_installed:
                 package_names.append(submodule.pypi_name)
 
         logger.info(
-            (
-                "You can now uninstall boto3-stubs with:\n\n"
-                "    python -m pip uninstall %s\n\n"
-                "If you want to use auto-typing for boto3.client/resource functions, run:\n\n"
-                "    mypy_boto3\n"
-            ),
+            "You can now uninstall boto3-stubs with:\n\n"
+            "    python -m pip uninstall %s\n\n"
+            "If you want to use auto-typing for boto3.client/resource functions, run:\n\n"
+            "    mypy_boto3\n",
             " ".join(package_names),
         )
         return
     build_package_methods(logger)
     for submodule in SUBMODULES:
         if not submodule.is_installed:
             submodule_path = ROOT_PATH / submodule.import_name
```

### Comparing `mypy-boto3-1.28.1/mypy_boto3/submodules.py` & `mypy-boto3-1.28.2/mypy_boto3/submodules.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.1/mypy_boto3.egg-info/PKG-INFO` & `mypy-boto3-1.28.2/mypy_boto3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.28.1
-Summary: Type annotations for boto3 1.28.1 master module generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3 1.28.2 master module generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/1.28.1/index.html)
+[boto3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/1.28.2/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.1/setup.py` & `mypy-boto3-1.28.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.28.1",
+    version="1.28.2",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3 1.28.1 master module generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3 1.28.2 master module generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

