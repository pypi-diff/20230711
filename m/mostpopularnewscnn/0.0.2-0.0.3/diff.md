# Comparing `tmp/mostpopularnewscnn-0.0.2.tar.gz` & `tmp/mostpopularnewscnn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostpopularnewscnn-0.0.2.tar", last modified: Mon Jul 10 13:44:20 2023, max compression
+gzip compressed data, was "mostpopularnewscnn-0.0.3.tar", last modified: Tue Jul 11 15:17:01 2023, max compression
```

## Comparing `mostpopularnewscnn-0.0.2.tar` & `mostpopularnewscnn-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.621883 mostpopularnewscnn-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-01 14:10:17.000000 mostpopularnewscnn-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1127 2023-07-10 13:44:20.620883 mostpopularnewscnn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-08 13:50:59.000000 mostpopularnewscnn-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.607884 mostpopularnewscnn-0.0.2/mostpopularnewscnn/
--rw-rw-rw-   0        0        0     2199 2023-07-10 13:29:11.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.618884 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/
--rw-rw-rw-   0        0        0     1127 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-07-10 13:41:31.000000 mostpopularnewscnn-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 13:44:20.622883 mostpopularnewscnn-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 15:17:01.969418 mostpopularnewscnn-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-01 14:10:17.000000 mostpopularnewscnn-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1274 2023-07-11 15:17:01.965419 mostpopularnewscnn-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-07-11 15:05:40.000000 mostpopularnewscnn-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 15:17:01.927419 mostpopularnewscnn-0.0.3/mostpopularnewscnn/
+-rw-rw-rw-   0        0        0     3420 2023-07-11 15:09:38.000000 mostpopularnewscnn-0.0.3/mostpopularnewscnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:17:01.958418 mostpopularnewscnn-0.0.3/mostpopularnewscnn.egg-info/
+-rw-rw-rw-   0        0        0     1274 2023-07-11 15:17:01.000000 mostpopularnewscnn-0.0.3/mostpopularnewscnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-11 15:17:01.000000 mostpopularnewscnn-0.0.3/mostpopularnewscnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:17:01.000000 mostpopularnewscnn-0.0.3/mostpopularnewscnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 15:17:01.000000 mostpopularnewscnn-0.0.3/mostpopularnewscnn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-07-11 15:16:03.000000 mostpopularnewscnn-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 15:17:01.970422 mostpopularnewscnn-0.0.3/setup.cfg
```

### Comparing `mostpopularnewscnn-0.0.2/LICENSE` & `mostpopularnewscnn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mostpopularnewscnn-0.0.2/pyproject.toml` & `mostpopularnewscnn-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.31.0", "beautifulsoup4>= 4.12.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mostpopularnewscnn"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Tri Prasetyo Kusumo Aji", email="ajikprasetyo22@gmail.com" },
 ]
 description = "This package will get the most popular news in CNN Indonesia"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

