# Comparing `tmp/phonetree-1.3.0.tar.gz` & `tmp/phonetree-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonetree-1.3.0.tar", last modified: Mon Jul 10 02:11:34 2023, max compression
+gzip compressed data, was "phonetree-1.3.1.tar", last modified: Tue Jul 11 20:34:18 2023, max compression
```

## Comparing `phonetree-1.3.0.tar` & `phonetree-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.119609 phonetree-1.3.0/
--rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.3.0/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-10 02:11:34.119511 phonetree-1.3.0/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.3.0/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.118810 phonetree-1.3.0/phonetree/
--rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.3.0/phonetree/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)    11373 2023-07-10 02:11:04.000000 phonetree-1.3.0/phonetree/phonetree.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.119391 phonetree-1.3.0/phonetree.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      241 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       18 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       10 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      944 2023-07-10 01:37:54.000000 phonetree-1.3.0/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-07-10 02:11:34.119634 phonetree-1.3.0/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 20:34:18.888625 phonetree-1.3.1/
+-rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.3.1/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-11 20:34:18.888516 phonetree-1.3.1/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.3.1/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 20:34:18.887703 phonetree-1.3.1/phonetree/
+-rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.3.1/phonetree/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)    11373 2023-07-10 02:11:04.000000 phonetree-1.3.1/phonetree/phonetree.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 20:34:18.888386 phonetree-1.3.1/phonetree.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-11 20:34:18.000000 phonetree-1.3.1/phonetree.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      241 2023-07-11 20:34:18.000000 phonetree-1.3.1/phonetree.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-07-11 20:34:18.000000 phonetree-1.3.1/phonetree.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       18 2023-07-11 20:34:18.000000 phonetree-1.3.1/phonetree.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       10 2023-07-11 20:34:18.000000 phonetree-1.3.1/phonetree.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)      944 2023-07-11 20:33:58.000000 phonetree-1.3.1/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-07-11 20:34:18.888658 phonetree-1.3.1/setup.cfg
```

### Comparing `phonetree-1.3.0/LICENSE` & `phonetree-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phonetree-1.3.0/PKG-INFO` & `phonetree-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.3.0
+Version: 1.3.1
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.3.0/README.md` & `phonetree-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `phonetree-1.3.0/phonetree/phonetree.py` & `phonetree-1.3.1/phonetree/phonetree.py`

 * *Files identical despite different names*

### Comparing `phonetree-1.3.0/phonetree.egg-info/PKG-INFO` & `phonetree-1.3.1/phonetree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.3.0
+Version: 1.3.1
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.3.0/pyproject.toml` & `phonetree-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonetree"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Leandro Lima", email="leandro@lls-software.com" },
 ]
 description = "A phone-tree like menu system for text-based interfaces"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

