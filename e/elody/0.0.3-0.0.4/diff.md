# Comparing `tmp/elody-0.0.3.tar.gz` & `tmp/elody-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.3.tar", last modified: Wed May 17 14:50:07 2023, max compression
+gzip compressed data, was "elody-0.0.4.tar", last modified: Tue Jul 11 14:03:31 2023, max compression
```

## Comparing `elody-0.0.3.tar` & `elody-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:50:07.938384 elody-0.0.3/
--rw-r--r--   0 booster   (1000) booster   (1000)    18092 2023-05-17 14:21:56.000000 elody-0.0.3/LICENSE
--rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:50:07.938384 elody-0.0.3/PKG-INFO
--rw-r--r--   0 booster   (1000) booster   (1000)     1263 2023-05-17 14:48:35.000000 elody-0.0.3/README.md
--rw-r--r--   0 booster   (1000) booster   (1000)      714 2023-05-17 14:48:35.000000 elody-0.0.3/pyproject.toml
--rw-r--r--   0 booster   (1000) booster   (1000)       38 2023-05-17 14:50:07.938384 elody-0.0.3/setup.cfg
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:50:07.938384 elody-0.0.3/src/
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:50:07.938384 elody-0.0.3/src/elody/
--rw-r--r--   0 booster   (1000) booster   (1000)       22 2023-05-17 14:21:56.000000 elody-0.0.3/src/elody/__init__.py
--rw-r--r--   0 booster   (1000) booster   (1000)     3924 2023-05-17 14:48:35.000000 elody-0.0.3/src/elody/client.py
--rw-r--r--   0 booster   (1000) booster   (1000)      209 2023-05-17 14:21:56.000000 elody-0.0.3/src/elody/exceptions.py
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:50:07.938384 elody-0.0.3/src/elody.egg-info/
--rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:50:07.000000 elody-0.0.3/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 booster   (1000) booster   (1000)      262 2023-05-17 14:50:07.000000 elody-0.0.3/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 booster   (1000) booster   (1000)        1 2023-05-17 14:50:07.000000 elody-0.0.3/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 booster   (1000) booster   (1000)       86 2023-05-17 14:50:07.000000 elody-0.0.3/src/elody.egg-info/requires.txt
--rw-r--r--   0 booster   (1000) booster   (1000)        6 2023-05-17 14:50:07.000000 elody-0.0.3/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:03:31.261202 elody-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 14:03:19.000000 elody-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-07-11 14:03:31.261202 elody-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-11 14:03:19.000000 elody-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-11 14:03:19.000000 elody-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:03:31.261202 elody-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:03:31.261202 elody-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:03:31.261202 elody-0.0.4/src/elody/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 14:03:19.000000 elody-0.0.4/src/elody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-11 14:03:19.000000 elody-0.0.4/src/elody/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 14:03:19.000000 elody-0.0.4/src/elody/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:03:31.261202 elody-0.0.4/src/elody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-07-11 14:03:31.000000 elody-0.0.4/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 14:03:31.000000 elody-0.0.4/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:03:31.000000 elody-0.0.4/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 14:03:31.000000 elody-0.0.4/src/elody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:03:31.000000 elody-0.0.4/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.3/LICENSE` & `elody-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.3/PKG-INFO` & `elody-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.3
+Version: 0.0.4
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `elody-0.0.3/README.md` & `elody-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `elody-0.0.3/pyproject.toml` & `elody-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.3"
+version = "0.0.4"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `elody-0.0.3/src/elody/client.py` & `elody-0.0.4/src/elody/client.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.3/src/elody.egg-info/PKG-INFO` & `elody-0.0.4/src/elody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.3
+Version: 0.0.4
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

