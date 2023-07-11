# Comparing `tmp/scribelex-1.0.8.tar.gz` & `tmp/scribelex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribelex-1.0.8.tar", last modified: Tue Jul 11 20:55:45 2023, max compression
+gzip compressed data, was "scribelex-1.0.9.tar", last modified: Tue Jul 11 20:57:46 2023, max compression
```

## Comparing `scribelex-1.0.8.tar` & `scribelex-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.170624 scribelex-1.0.8/
--rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1596 2023-07-11 20:55:45.169618 scribelex-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-07-08 21:29:07.000000 scribelex-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.158306 scribelex-1.0.8/scribelex/
--rw-rw-rw-   0        0        0       44 2023-07-11 20:35:48.000000 scribelex-1.0.8/scribelex/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-07-11 19:12:33.000000 scribelex-1.0.8/scribelex/base.py
--rw-rw-rw-   0        0        0     1486 2023-07-11 20:35:12.000000 scribelex-1.0.8/scribelex/common.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.169618 scribelex-1.0.8/scribelex.egg-info/
--rw-rw-rw-   0        0        0     1596 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 20:55:45.170624 scribelex-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1252 2023-07-11 20:55:40.000000 scribelex-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:57:46.923666 scribelex-1.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1596 2023-07-11 20:57:46.923666 scribelex-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-07-08 21:29:07.000000 scribelex-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:57:46.914667 scribelex-1.0.9/scribelex/
+-rw-rw-rw-   0        0        0       44 2023-07-11 20:35:48.000000 scribelex-1.0.9/scribelex/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-07-11 19:12:33.000000 scribelex-1.0.9/scribelex/base.py
+-rw-rw-rw-   0        0        0     1487 2023-07-11 20:57:24.000000 scribelex-1.0.9/scribelex/common.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:57:46.922666 scribelex-1.0.9/scribelex.egg-info/
+-rw-rw-rw-   0        0        0     1596 2023-07-11 20:57:46.000000 scribelex-1.0.9/scribelex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-11 20:57:46.000000 scribelex-1.0.9/scribelex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:57:46.000000 scribelex-1.0.9/scribelex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-11 20:57:46.000000 scribelex-1.0.9/scribelex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:57:46.923666 scribelex-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-07-11 20:57:44.000000 scribelex-1.0.9/setup.py
```

### Comparing `scribelex-1.0.8/LICENSE` & `scribelex-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.8/PKG-INFO` & `scribelex-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scribelex-1.0.8/README.md` & `scribelex-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.8/scribelex/base.py` & `scribelex-1.0.9/scribelex/base.py`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.8/scribelex/common.py` & `scribelex-1.0.9/scribelex/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from base import filt, shift, one_or_more, fmap, seq, atom, one_of, zero_or_more, right
+from .base import filt, shift, one_or_more, fmap, seq, atom, one_of, zero_or_more, right
 import string as python_string
 
 # Цифра
 digit = filt(str.isdigit)(shift)
 
 # Цифры
 digits = one_or_more(digit)
```

### Comparing `scribelex-1.0.8/scribelex.egg-info/PKG-INFO` & `scribelex-1.0.9/scribelex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scribelex-1.0.8/setup.py` & `scribelex-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scribelex",
-    version="1.0.8",
+    version="1.0.9",
     author="UncleDrema",
     author_email="missl.wipiece@gmail.com",
     description="Scribelex is a lightweight Python library for building parser combinators.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
     url="https://github.com/UncleDrema/scribelex",
```

