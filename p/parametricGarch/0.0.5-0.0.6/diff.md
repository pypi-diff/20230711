# Comparing `tmp/parametricGarch-0.0.5.tar.gz` & `tmp/parametricGarch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parametricGarch-0.0.5.tar", last modified: Tue Jul 11 08:47:18 2023, max compression
+gzip compressed data, was "parametricGarch-0.0.6.tar", last modified: Tue Jul 11 09:04:12 2023, max compression
```

## Comparing `parametricGarch-0.0.5.tar` & `parametricGarch-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.877014 parametricGarch-0.0.5/
--rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.5/LICENSE
--rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:47:18.876648 parametricGarch-0.0.5/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)     2190 2023-07-09 20:31:59.000000 parametricGarch-0.0.5/README.md
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.874008 parametricGarch-0.0.5/parametricGarch/
--rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.5/parametricGarch/__init__.py
--rw-r--r--   0 playerone   (501) staff       (20)    11642 2023-07-06 15:32:05.000000 parametricGarch-0.0.5/parametricGarch/parametric.py
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 08:47:18.875970 parametricGarch-0.0.5/parametricGarch.egg-info/
--rw-r--r--   0 playerone   (501) staff       (20)     3223 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/SOURCES.txt
--rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/dependency_links.txt
--rw-r--r--   0 playerone   (501) staff       (20)       24 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/requires.txt
--rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-11 08:47:18.000000 parametricGarch-0.0.5/parametricGarch.egg-info/top_level.txt
--rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-11 08:47:18.877108 parametricGarch-0.0.5/setup.cfg
--rw-r--r--   0 playerone   (501) staff       (20)     1767 2023-07-11 08:47:13.000000 parametricGarch-0.0.5/setup.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 09:04:12.501885 parametricGarch-0.0.6/
+-rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.6/LICENSE
+-rw-r--r--   0 playerone   (501) staff       (20)     3222 2023-07-11 09:04:12.501370 parametricGarch-0.0.6/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)     2189 2023-07-11 08:57:50.000000 parametricGarch-0.0.6/README.md
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 09:04:12.498082 parametricGarch-0.0.6/parametricGarch/
+-rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.6/parametricGarch/__init__.py
+-rw-r--r--   0 playerone   (501) staff       (20)    11642 2023-07-06 15:32:05.000000 parametricGarch-0.0.6/parametricGarch/parametric.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-11 09:04:12.500594 parametricGarch-0.0.6/parametricGarch.egg-info/
+-rw-r--r--   0 playerone   (501) staff       (20)     3222 2023-07-11 09:04:11.000000 parametricGarch-0.0.6/parametricGarch.egg-info/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-11 09:04:12.000000 parametricGarch-0.0.6/parametricGarch.egg-info/SOURCES.txt
+-rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-11 09:04:11.000000 parametricGarch-0.0.6/parametricGarch.egg-info/dependency_links.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       24 2023-07-11 09:04:12.000000 parametricGarch-0.0.6/parametricGarch.egg-info/requires.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-11 09:04:12.000000 parametricGarch-0.0.6/parametricGarch.egg-info/top_level.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-11 09:04:12.502055 parametricGarch-0.0.6/setup.cfg
+-rw-r--r--   0 playerone   (501) staff       (20)     1654 2023-07-11 09:04:07.000000 parametricGarch-0.0.6/setup.py
```

### Comparing `parametricGarch-0.0.5/LICENSE` & `parametricGarch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.5/PKG-INFO` & `parametricGarch-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 # ParametricGarch
 A Python library that uses parametric bootstrapping via the GARCH model to estimate volatility and Value-at-Risk (VaR) for financial assets.
 
 ### Installation
 You can install parametricGarch using pip:
 ```
-pip install parametric-garch
+pip install parametricGarch
 ```
 
 ## Dependencies
 The package dependencies are:
 - arch
 - numpy
 - pandas
```

### Comparing `parametricGarch-0.0.5/README.md` & `parametricGarch-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ParametricGarch
 A Python library that uses parametric bootstrapping via the GARCH model to estimate volatility and Value-at-Risk (VaR) for financial assets.
 
 ### Installation
 You can install parametricGarch using pip:
 ```
-pip install parametric-garch
+pip install parametricGarch
 ```
 
 ## Dependencies
 The package dependencies are:
 - arch
 - numpy
 - pandas
```

### Comparing `parametricGarch-0.0.5/parametricGarch/parametric.py` & `parametricGarch-0.0.6/parametricGarch/parametric.py`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.5/parametricGarch.egg-info/PKG-INFO` & `parametricGarch-0.0.6/parametricGarch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 # ParametricGarch
 A Python library that uses parametric bootstrapping via the GARCH model to estimate volatility and Value-at-Risk (VaR) for financial assets.
 
 ### Installation
 You can install parametricGarch using pip:
 ```
-pip install parametric-garch
+pip install parametricGarch
 ```
 
 ## Dependencies
 The package dependencies are:
 - arch
 - numpy
 - pandas
```

### Comparing `parametricGarch-0.0.5/setup.py` & `parametricGarch-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 #Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-# with open("README.md", "r") as fh:
-#     long_description = fh.read()
 
 LONG_DESCRIPTION = long_description
 
-# This call to setup() does all the work
 setup(
     name="parametricGarch",
-    version="0.0.5",
+    version="0.0.6",
     description="Parametric Bootstrapping via the GARCH model",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/chideraani/ParametricGarch",
     author="Chidera",
     author_email="chideraani27@gmail.com",
     license="GNU",
```

