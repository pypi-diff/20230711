# Comparing `tmp/lime_nda-0.0.8.tar.gz` & `tmp/lime_nda-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime_nda-0.0.8.tar", last modified: Tue Jul 11 12:03:29 2023, max compression
+gzip compressed data, was "lime_nda-0.0.9.tar", last modified: Tue Jul 11 12:46:16 2023, max compression
```

## Comparing `lime_nda-0.0.8.tar` & `lime_nda-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:03:29.070570 lime_nda-0.0.8/
--rw-rw-rw-   0        0        0    35823 2023-07-11 10:38:49.000000 lime_nda-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1805 2023-07-11 12:03:29.068498 lime_nda-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-11 10:38:49.000000 lime_nda-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 12:03:29.034165 lime_nda-0.0.8/lime_nda/
--rw-rw-rw-   0        0        0      266 2023-07-11 10:38:49.000000 lime_nda-0.0.8/lime_nda/__init__.py
--rw-rw-rw-   0        0        0    17960 2023-07-11 11:52:38.000000 lime_nda-0.0.8/lime_nda/nda_functions.py
--rw-rw-rw-   0        0        0    13742 2023-07-11 10:38:49.000000 lime_nda-0.0.8/lime_nda/nda_version_8_0.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:03:29.065929 lime_nda-0.0.8/lime_nda.egg-info/
--rw-rw-rw-   0        0        0     1805 2023-07-11 12:03:28.000000 lime_nda-0.0.8/lime_nda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-11 12:03:28.000000 lime_nda-0.0.8/lime_nda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:03:28.000000 lime_nda-0.0.8/lime_nda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 12:03:28.000000 lime_nda-0.0.8/lime_nda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      665 2023-07-11 11:57:49.000000 lime_nda-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 12:03:29.072517 lime_nda-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 12:46:16.036322 lime_nda-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 10:38:49.000000 lime_nda-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1805 2023-07-11 12:46:16.034636 lime_nda-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-11 10:38:49.000000 lime_nda-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 12:46:15.981416 lime_nda-0.0.9/lime_nda/
+-rw-rw-rw-   0        0        0      266 2023-07-11 10:38:49.000000 lime_nda-0.0.9/lime_nda/__init__.py
+-rw-rw-rw-   0        0        0    17960 2023-07-11 12:44:29.000000 lime_nda-0.0.9/lime_nda/nda_functions.py
+-rw-rw-rw-   0        0        0    13742 2023-07-11 10:38:49.000000 lime_nda-0.0.9/lime_nda/nda_version_8_0.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:46:16.028648 lime_nda-0.0.9/lime_nda.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      665 2023-07-11 12:45:17.000000 lime_nda-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:46:16.037341 lime_nda-0.0.9/setup.cfg
```

### Comparing `lime_nda-0.0.8/LICENSE` & `lime_nda-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.8/PKG-INFO` & `lime_nda-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime_nda
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime CellTesting <vividhgarg@outlook.com>
 Project-URL: Homepage, https://github.com/vividh-garg/NDA
 Project-URL: Bug Tracker, https://github.com/vividh-garg/NDA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lime_nda-0.0.8/README.md` & `lime_nda-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.8/lime_nda/nda_functions.py` & `lime_nda-0.0.9/lime_nda/nda_functions.py`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.8/lime_nda/nda_version_8_0.py` & `lime_nda-0.0.9/lime_nda/nda_version_8_0.py`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.8/lime_nda.egg-info/PKG-INFO` & `lime_nda-0.0.9/lime_nda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-nda
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime CellTesting <vividhgarg@outlook.com>
 Project-URL: Homepage, https://github.com/vividh-garg/NDA
 Project-URL: Bug Tracker, https://github.com/vividh-garg/NDA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lime_nda-0.0.8/pyproject.toml` & `lime_nda-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lime_nda"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Lime CellTesting", email="vividhgarg@outlook.com" },
 ]
 description = 'Python Package for working with NDA files, specifically for people at Lime.AI' 
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

