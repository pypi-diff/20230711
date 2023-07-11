# Comparing `tmp/pydantic-collections-0.4.0.tar.gz` & `tmp/pydantic-collections-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydantic-collections-0.4.0.tar", last modified: Sun Oct 16 12:09:24 2022, max compression
+gzip compressed data, was "dist/pydantic-collections-0.4.1.tar", last modified: Tue Jul 11 05:04:41 2023, max compression
```

## Comparing `pydantic-collections-0.4.0.tar` & `pydantic-collections-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 pydantic-collections-0.4.0/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 pydantic-collections-0.4.0/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     3576 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     3183 2021-10-30 06:37:45.000000 pydantic-collections-0.4.0/README.md
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections/
--rw-rw-r--   0 roman     (1000) roman     (1000)      192 2022-10-16 09:06:07.000000 pydantic-collections-0.4.0/pydantic_collections/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     7006 2022-10-16 09:08:32.000000 pydantic-collections-0.4.0/pydantic_collections/_base_collection_model.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     3576 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      356 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       16 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       21 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/pydantic_collections.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      158 2021-10-22 13:36:03.000000 pydantic-collections-0.4.0/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2022-10-16 12:09:24.000000 pydantic-collections-0.4.0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1173 2021-10-23 13:09:28.000000 pydantic-collections-0.4.0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 pydantic-collections-0.4.1/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 pydantic-collections-0.4.1/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3577 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3184 2023-07-11 04:54:51.000000 pydantic-collections-0.4.1/README.md
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      192 2023-07-11 04:53:14.000000 pydantic-collections-0.4.1/pydantic_collections/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     7006 2022-10-16 09:08:32.000000 pydantic-collections-0.4.1/pydantic_collections/_base_collection_model.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3577 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      356 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       21 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       21 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      158 2021-10-22 13:36:03.000000 pydantic-collections-0.4.1/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1178 2023-07-11 04:54:51.000000 pydantic-collections-0.4.1/setup.py
```

### Comparing `pydantic-collections-0.4.0/LICENSE.txt` & `pydantic-collections-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydantic-collections-0.4.0/PKG-INFO` & `pydantic-collections-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-collections
-Version: 0.4.0
+Version: 0.4.1
 Summary: Collections of pydantic models
 Home-page: https://github.com/romis2012/pydantic-collections
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: python pydantic validation parsing serialization models
 Platform: UNKNOWN
@@ -19,16 +19,16 @@
 
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
-- Python >= 3.7
-- pydantic >= 1.8.2
+- Python>=3.7
+- pydantic>=1.8.2,<2.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
```

### Comparing `pydantic-collections-0.4.0/README.md` & `pydantic-collections-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
-- Python >= 3.7
-- pydantic >= 1.8.2
+- Python>=3.7
+- pydantic>=1.8.2,<2.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
```

### Comparing `pydantic-collections-0.4.0/pydantic_collections/_base_collection_model.py` & `pydantic-collections-0.4.1/pydantic_collections/_base_collection_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-collections-0.4.0/pydantic_collections.egg-info/PKG-INFO` & `pydantic-collections-0.4.1/pydantic_collections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-collections
-Version: 0.4.0
+Version: 0.4.1
 Summary: Collections of pydantic models
 Home-page: https://github.com/romis2012/pydantic-collections
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: python pydantic validation parsing serialization models
 Platform: UNKNOWN
@@ -19,16 +19,16 @@
 
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
-- Python >= 3.7
-- pydantic >= 1.8.2
+- Python>=3.7
+- pydantic>=1.8.2,<2.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
```

### Comparing `pydantic-collections-0.4.0/setup.py` & `pydantic-collections-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     license='Apache 2',
     url='https://github.com/romis2012/pydantic-collections',
     description='Collections of pydantic models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['pydantic_collections'],
     keywords='python pydantic validation parsing serialization models',
-    install_requires=['pydantic>=1.8.2']
+    install_requires=['pydantic>=1.8.2,<2.0']
 )
```

