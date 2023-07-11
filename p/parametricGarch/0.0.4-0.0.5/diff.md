# Comparing `tmp/parametricGarch-0.0.4.tar.gz` & `tmp/parametricGarch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parametricGarch-0.0.4.tar", last modified: Tue Jul 11 08:42:27 2023, max compression
+gzip compressed data, was "parametricGarch-0.0.5.tar", last modified: Tue Jul 11 08:47:18 2023, max compression
```

## Comparing `parametricGarch-0.0.4.tar` & `parametricGarch-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:42:27.225355 parametricGarch-0.0.4/
--rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.4/LICENSE
--rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:42:27.225078 parametricGarch-0.0.4/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)     2190 2023-07-09 20:31:59.000000 parametricGarch-0.0.4/README.md
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:42:27.222392 parametricGarch-0.0.4/parametricGarch/
--rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.4/parametricGarch/__init__.py
--rw-r--r--   0 playerone   (501) staff       (20)    11642 2023-07-06 15:32:05.000000 parametricGarch-0.0.4/parametricGarch/parametric.py
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:42:27.224509 parametricGarch-0.0.4/parametricGarch.egg-info/
--rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:42:26.000000 parametricGarch-0.0.4/parametricGarch.egg-info/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-11 08:42:27.000000 parametricGarch-0.0.4/parametricGarch.egg-info/SOURCES.txt
--rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-11 08:42:26.000000 parametricGarch-0.0.4/parametricGarch.egg-info/dependency_links.txt
--rw-r--r--   0 playerone   (501) staff       (20)       24 2023-07-11 08:42:26.000000 parametricGarch-0.0.4/parametricGarch.egg-info/requires.txt
--rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-11 08:42:27.000000 parametricGarch-0.0.4/parametricGarch.egg-info/top_level.txt
--rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-11 08:42:27.225472 parametricGarch-0.0.4/setup.cfg
--rw-r--r--   0 playerone   (501) staff       (20)     1768 2023-07-11 08:42:05.000000 parametricGarch-0.0.4/setup.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.877014 parametricGarch-0.0.5/
+-rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.5/LICENSE
+-rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:47:18.876648 parametricGarch-0.0.5/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)     2190 2023-07-09 20:31:59.000000 parametricGarch-0.0.5/README.md
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.874008 parametricGarch-0.0.5/parametricGarch/
+-rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.5/parametricGarch/__init__.py
+-rw-r--r--   0 playerone   (501) staff       (20)    11642 2023-07-06 15:32:05.000000 parametricGarch-0.0.5/parametricGarch/parametric.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.875970 parametricGarch-0.0.5/parametricGarch.egg-info/
+-rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/SOURCES.txt
+-rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/dependency_links.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       24 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/requires.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/top_level.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-11 08:47:18.877108 parametricGarch-0.0.5/setup.cfg
+-rw-r--r--   0 playerone   (501) staff       (20)     1767 2023-07-11 08:47:13.000000 parametricGarch-0.0.5/setup.py
```

### Comparing `parametricGarch-0.0.4/LICENSE` & `parametricGarch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.4/PKG-INFO` & `parametricGarch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
```

### Comparing `parametricGarch-0.0.4/README.md` & `parametricGarch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.4/parametricGarch/parametric.py` & `parametricGarch-0.0.5/parametricGarch/parametric.py`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.4/parametricGarch.egg-info/PKG-INFO` & `parametricGarch-0.0.5/parametricGarch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
```

### Comparing `parametricGarch-0.0.4/setup.py` & `parametricGarch-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
-# Get the long description from the README file
-# with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
-#     long_description = f.read()
+#Get the long description from the README file
+with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+# with open("README.md", "r") as fh:
+#     long_description = fh.read()
 
 LONG_DESCRIPTION = long_description
 
 # This call to setup() does all the work
 setup(
     name="parametricGarch",
-    version="0.0.4",
+    version="0.0.5",
     description="Parametric Bootstrapping via the GARCH model",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/chideraani/ParametricGarch",
     author="Chidera",
     author_email="chideraani27@gmail.com",
     license="GNU",
```

