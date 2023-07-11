# Comparing `tmp/cle_utilities-0.0.1.tar.gz` & `tmp/cle_utilities-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cle_utilities-0.0.1.tar", last modified: Wed Jun 28 13:14:16 2023, max compression
+gzip compressed data, was "cle_utilities-0.0.2.tar", last modified: Tue Jul 11 10:30:45 2023, max compression
```

## Comparing `cle_utilities-0.0.1.tar` & `cle_utilities-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:14:16.384503 cle_utilities-0.0.1/
--rw-rw-rw-   0        0        0     1075 2023-06-28 12:50:38.000000 cle_utilities-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      888 2023-06-28 13:14:16.383366 cle_utilities-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-06-28 13:10:31.000000 cle_utilities-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 13:14:16.341405 cle_utilities-0.0.1/cle_utilities/
--rw-rw-rw-   0        0        0        0 2023-06-28 12:44:12.000000 cle_utilities-0.0.1/cle_utilities/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-14 13:27:51.000000 cle_utilities-0.0.1/cle_utilities/cle_log.py
--rw-rw-rw-   0        0        0     1252 2023-06-13 12:47:51.000000 cle_utilities-0.0.1/cle_utilities/cleexceptionrequest.py
--rw-rw-rw-   0        0        0      790 2023-06-09 09:47:11.000000 cle_utilities-0.0.1/cle_utilities/cleheader.py
--rw-rw-rw-   0        0        0      764 2023-06-09 09:47:31.000000 cle_utilities-0.0.1/cle_utilities/clelogrequest.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:14:16.381370 cle_utilities-0.0.1/cle_utilities.egg-info/
--rw-rw-rw-   0        0        0      888 2023-06-28 13:14:16.000000 cle_utilities-0.0.1/cle_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-28 13:14:16.000000 cle_utilities-0.0.1/cle_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:14:16.000000 cle_utilities-0.0.1/cle_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-28 13:14:16.000000 cle_utilities-0.0.1/cle_utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-28 13:14:16.000000 cle_utilities-0.0.1/cle_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      705 2023-06-28 12:59:24.000000 cle_utilities-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 13:14:16.384503 cle_utilities-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:45.962834 cle_utilities-0.0.2/
+-rw-rw-rw-   0        0        0     1075 2023-06-28 12:50:38.000000 cle_utilities-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      888 2023-07-11 10:30:45.961818 cle_utilities-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-06-28 13:10:31.000000 cle_utilities-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:45.910323 cle_utilities-0.0.2/cle_utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-28 12:44:12.000000 cle_utilities-0.0.2/cle_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-06-14 13:27:51.000000 cle_utilities-0.0.2/cle_utilities/cle_log.py
+-rw-rw-rw-   0        0        0     3801 2023-07-10 12:46:13.000000 cle_utilities-0.0.2/cle_utilities/cledataclasses.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:45.958835 cle_utilities-0.0.2/cle_utilities.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-11 10:30:45.000000 cle_utilities-0.0.2/cle_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-11 10:30:45.000000 cle_utilities-0.0.2/cle_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:30:45.000000 cle_utilities-0.0.2/cle_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-11 10:30:45.000000 cle_utilities-0.0.2/cle_utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 10:30:45.000000 cle_utilities-0.0.2/cle_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2023-07-11 10:25:12.000000 cle_utilities-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:30:45.962834 cle_utilities-0.0.2/setup.cfg
```

### Comparing `cle_utilities-0.0.1/LICENSE` & `cle_utilities-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cle_utilities-0.0.1/PKG-INFO` & `cle_utilities-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cle_utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: A logging package which will help to implement the cle capabilities and design the requests to be sent to cle api.
 Author-email: Adeep Malmotra <Adeep.Malmotra@ibm.com>
 Keywords: cle,logging,automated alert,exceptions
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cle_utilities-0.0.1/cle_utilities/cle_log.py` & `cle_utilities-0.0.2/cle_utilities/cle_log.py`

 * *Files identical despite different names*

### Comparing `cle_utilities-0.0.1/cle_utilities.egg-info/PKG-INFO` & `cle_utilities-0.0.2/cle_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cle-utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: A logging package which will help to implement the cle capabilities and design the requests to be sent to cle api.
 Author-email: Adeep Malmotra <Adeep.Malmotra@ibm.com>
 Keywords: cle,logging,automated alert,exceptions
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cle_utilities-0.0.1/pyproject.toml` & `cle_utilities-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cle_utilities"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Adeep Malmotra", email="Adeep.Malmotra@ibm.com" },
 ]
 description = "A logging package which will help to implement the cle capabilities and design the requests to be sent to cle api."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["cle", "logging", "automated alert", "exceptions"]
```

