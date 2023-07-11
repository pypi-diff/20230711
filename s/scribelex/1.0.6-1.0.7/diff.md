# Comparing `tmp/scribelex-1.0.6.tar.gz` & `tmp/scribelex-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribelex-1.0.6.tar", last modified: Tue Jul 11 20:19:06 2023, max compression
+gzip compressed data, was "scribelex-1.0.7.tar", last modified: Tue Jul 11 20:41:21 2023, max compression
```

## Comparing `scribelex-1.0.6.tar` & `scribelex-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:19:06.673139 scribelex-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 20:19:01.000000 scribelex-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:19:06.673139 scribelex-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 20:19:01.000000 scribelex-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:19:06.673139 scribelex-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 20:19:01.000000 scribelex-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:19:06.669139 scribelex-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:19:06.673139 scribelex-1.0.6/src/scribelex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:19:06.000000 scribelex-1.0.6/src/scribelex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 20:19:06.000000 scribelex-1.0.6/src/scribelex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:19:06.000000 scribelex-1.0.6/src/scribelex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:19:06.000000 scribelex-1.0.6/src/scribelex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:41:21.418811 scribelex-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 20:41:17.000000 scribelex-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:41:21.418811 scribelex-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 20:41:17.000000 scribelex-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:41:21.418811 scribelex-1.0.7/scribelex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:41:21.418811 scribelex-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-11 20:41:17.000000 scribelex-1.0.7/setup.py
```

### Comparing `scribelex-1.0.6/LICENSE` & `scribelex-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.6/PKG-INFO` & `scribelex-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.6
+Version: 1.0.7
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scribelex-1.0.6/README.md` & `scribelex-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.6/setup.py` & `scribelex-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scribelex",
-    version="1.0.6",
+    version="1.0.7",
     author="UncleDrema",
     author_email="missl.wipiece@gmail.com",
     description="Scribelex is a lightweight Python library for building parser combinators.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
     url="https://github.com/UncleDrema/scribelex",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
+    packages=find_packages("scribelex"),
+    package_dir={"scribelex": "scribelex"},
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `scribelex-1.0.6/src/scribelex.egg-info/PKG-INFO` & `scribelex-1.0.7/scribelex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.6
+Version: 1.0.7
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

