# Comparing `tmp/almost_unique_id-0.0.2.tar.gz` & `tmp/almost_unique_id-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almost_unique_id-0.0.2.tar", last modified: Fri Nov 18 22:09:52 2022, max compression
+gzip compressed data, was "almost_unique_id-0.0.3.tar", last modified: Tue Jul 11 20:16:39 2023, max compression
```

## Comparing `almost_unique_id-0.0.2.tar` & `almost_unique_id-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2022-11-18 22:09:52.299419 almost_unique_id-0.0.2/
--rw-r--r--   0 avi        (501) staff       (20)     1074 2022-11-18 22:02:18.000000 almost_unique_id-0.0.2/LICENSE.md
--rw-r--r--   0 avi        (501) staff       (20)     1816 2022-11-18 22:09:52.299308 almost_unique_id-0.0.2/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     1583 2022-11-18 21:57:03.000000 almost_unique_id-0.0.2/README.md
--rw-r--r--   0 avi        (501) staff       (20)    14904 2022-09-06 17:53:16.000000 almost_unique_id-0.0.2/adjectives.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2022-11-18 22:09:52.299160 almost_unique_id-0.0.2/almost_unique_id.egg-info/
--rw-r--r--   0 avi        (501) staff       (20)     1816 2022-11-18 22:09:52.000000 almost_unique_id-0.0.2/almost_unique_id.egg-info/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)      232 2022-11-18 22:09:52.000000 almost_unique_id-0.0.2/almost_unique_id.egg-info/SOURCES.txt
--rw-r--r--   0 avi        (501) staff       (20)        1 2022-11-18 22:09:52.000000 almost_unique_id-0.0.2/almost_unique_id.egg-info/dependency_links.txt
--rw-r--r--   0 avi        (501) staff       (20)       34 2022-11-18 22:09:52.000000 almost_unique_id-0.0.2/almost_unique_id.egg-info/top_level.txt
--rw-r--r--   0 avi        (501) staff       (20)      313 2022-11-18 21:50:31.000000 almost_unique_id-0.0.2/almost_unique_id.py
--rw-r--r--   0 avi        (501) staff       (20)   188283 2022-09-06 17:53:16.000000 almost_unique_id-0.0.2/names.py
--rw-r--r--   0 avi        (501) staff       (20)       38 2022-11-18 22:09:52.299459 almost_unique_id-0.0.2/setup.cfg
--rw-r--r--   0 avi        (501) staff       (20)      719 2022-11-18 22:09:47.000000 almost_unique_id-0.0.2/setup.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-07-11 20:16:39.151121 almost_unique_id-0.0.3/
+-rw-r--r--   0 avi        (501) staff       (20)     1074 2022-11-18 22:02:18.000000 almost_unique_id-0.0.3/LICENSE.md
+-rw-r--r--   0 avi        (501) staff       (20)     1912 2023-07-11 20:16:39.150977 almost_unique_id-0.0.3/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     1679 2022-11-18 22:15:17.000000 almost_unique_id-0.0.3/README.md
+-rw-r--r--   0 avi        (501) staff       (20)    14904 2022-09-06 17:53:16.000000 almost_unique_id-0.0.3/adjectives.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-07-11 20:16:39.150813 almost_unique_id-0.0.3/almost_unique_id.egg-info/
+-rw-r--r--   0 avi        (501) staff       (20)     1912 2023-07-11 20:16:39.000000 almost_unique_id-0.0.3/almost_unique_id.egg-info/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)      232 2023-07-11 20:16:39.000000 almost_unique_id-0.0.3/almost_unique_id.egg-info/SOURCES.txt
+-rw-r--r--   0 avi        (501) staff       (20)        1 2023-07-11 20:16:39.000000 almost_unique_id-0.0.3/almost_unique_id.egg-info/dependency_links.txt
+-rw-r--r--   0 avi        (501) staff       (20)       34 2023-07-11 20:16:39.000000 almost_unique_id-0.0.3/almost_unique_id.egg-info/top_level.txt
+-rw-r--r--   0 avi        (501) staff       (20)      317 2023-07-11 20:15:15.000000 almost_unique_id-0.0.3/almost_unique_id.py
+-rw-r--r--   0 avi        (501) staff       (20)   188283 2022-09-06 17:53:16.000000 almost_unique_id-0.0.3/names.py
+-rw-r--r--   0 avi        (501) staff       (20)       38 2023-07-11 20:16:39.151167 almost_unique_id-0.0.3/setup.cfg
+-rw-r--r--   0 avi        (501) staff       (20)      719 2023-07-11 20:15:38.000000 almost_unique_id-0.0.3/setup.py
```

### Comparing `almost_unique_id-0.0.2/LICENSE.md` & `almost_unique_id-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `almost_unique_id-0.0.2/PKG-INFO` & `almost_unique_id-0.0.3/almost_unique_id.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: almost_unique_id
-Version: 0.0.2
+Name: almost-unique-id
+Version: 0.0.3
 Summary: Almost Unique IDs
 Author: Avi Schwarzschild
 License: MIT
 Keywords: run ids
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,16 +12,23 @@
 # almost-unique-id
 Get almost unique ID names. This package randomly selects an `adjective-Name` pair from 24,567,933 unique pairs. 
 
 These IDs serve much the same pupose as generating a random hex string, that is to get random names for things that are (extrememly) unlikely to overlap. This project was developed alongside several scientific research projects where many trial of an experiment needed to be named distictly. We find that Enlglish languane keys are easier to discuss and remember than some number of digits/letters that might be unpronounceable. 
 
 Feel free to use this for any such application. If you have a use for this that you think is worth mentioning in the README, feel free to open a PR and add it so the description.
 
-## Installation  
-To install this package, git clone it and install with pip as follows.
+## Installation
+
+This package is installable with pip:
+
+```
+$ pip install almost-unique-id
+```
+
+Or, you can install it from source by git cloning it and installing with pip as follows.
 
 ```
 $ git clone https://github.com/aks2203/almost-unique-id.git
 $ cd almost-unique-id
 $ pip install -e .
 ```
```

### Comparing `almost_unique_id-0.0.2/README.md` & `almost_unique_id-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # almost-unique-id
 Get almost unique ID names. This package randomly selects an `adjective-Name` pair from 24,567,933 unique pairs. 
 
 These IDs serve much the same pupose as generating a random hex string, that is to get random names for things that are (extrememly) unlikely to overlap. This project was developed alongside several scientific research projects where many trial of an experiment needed to be named distictly. We find that Enlglish languane keys are easier to discuss and remember than some number of digits/letters that might be unpronounceable. 
 
 Feel free to use this for any such application. If you have a use for this that you think is worth mentioning in the README, feel free to open a PR and add it so the description.
 
-## Installation  
-To install this package, git clone it and install with pip as follows.
+## Installation
+
+This package is installable with pip:
+
+```
+$ pip install almost-unique-id
+```
+
+Or, you can install it from source by git cloning it and installing with pip as follows.
 
 ```
 $ git clone https://github.com/aks2203/almost-unique-id.git
 $ cd almost-unique-id
 $ pip install -e .
 ```
```

### Comparing `almost_unique_id-0.0.2/adjectives.py` & `almost_unique_id-0.0.3/adjectives.py`

 * *Files identical despite different names*

### Comparing `almost_unique_id-0.0.2/almost_unique_id.egg-info/PKG-INFO` & `almost_unique_id-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: almost-unique-id
-Version: 0.0.2
+Name: almost_unique_id
+Version: 0.0.3
 Summary: Almost Unique IDs
 Author: Avi Schwarzschild
 License: MIT
 Keywords: run ids
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,16 +12,23 @@
 # almost-unique-id
 Get almost unique ID names. This package randomly selects an `adjective-Name` pair from 24,567,933 unique pairs. 
 
 These IDs serve much the same pupose as generating a random hex string, that is to get random names for things that are (extrememly) unlikely to overlap. This project was developed alongside several scientific research projects where many trial of an experiment needed to be named distictly. We find that Enlglish languane keys are easier to discuss and remember than some number of digits/letters that might be unpronounceable. 
 
 Feel free to use this for any such application. If you have a use for this that you think is worth mentioning in the README, feel free to open a PR and add it so the description.
 
-## Installation  
-To install this package, git clone it and install with pip as follows.
+## Installation
+
+This package is installable with pip:
+
+```
+$ pip install almost-unique-id
+```
+
+Or, you can install it from source by git cloning it and installing with pip as follows.
 
 ```
 $ git clone https://github.com/aks2203/almost-unique-id.git
 $ cd almost-unique-id
 $ pip install -e .
 ```
```

### Comparing `almost_unique_id-0.0.2/names.py` & `almost_unique_id-0.0.3/names.py`

 * *Files identical despite different names*

### Comparing `almost_unique_id-0.0.2/setup.py` & `almost_unique_id-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 sys.path.insert(0, path.join(here, "almost-unique-id"))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name="almost_unique_id",
-      version="v0.0.2",
+      version="v0.0.3",
       description="Almost Unique IDs",
       author="Avi Schwarzschild",
       keywords=["run ids"],
       long_description=long_description,
       long_description_content_type="text/markdown",
       py_modules=["almost_unique_id", "adjectives", "names"],
       python_requires=">=3.7",
```

