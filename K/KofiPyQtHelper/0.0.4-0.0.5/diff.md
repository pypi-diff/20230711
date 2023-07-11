# Comparing `tmp/KofiPyQtHelper-0.0.4.tar.gz` & `tmp/KofiPyQtHelper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KofiPyQtHelper-0.0.4.tar", last modified: Tue Jul 11 09:46:27 2023, max compression
+gzip compressed data, was "dist/KofiPyQtHelper-0.0.5.tar", last modified: Tue Jul 11 09:51:10 2023, max compression
```

## Comparing `KofiPyQtHelper-0.0.4.tar` & `KofiPyQtHelper-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)      207 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/requires.txt
--rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/KofiPyQtHelper.egg-info/top_level.txt
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.4/README.md
--rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 09:46:27.000000 KofiPyQtHelper-0.0.4/setup.cfg
--rw-r--r--   0 kofi       (501) staff       (20)      892 2023-07-11 09:46:22.000000 KofiPyQtHelper-0.0.4/setup.py
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      207 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/requires.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/KofiPyQtHelper.egg-info/top_level.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.5/README.md
+-rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 09:51:10.000000 KofiPyQtHelper-0.0.5/setup.cfg
+-rw-r--r--   0 kofi       (501) staff       (20)      892 2023-07-11 09:51:01.000000 KofiPyQtHelper-0.0.5/setup.py
```

### Comparing `KofiPyQtHelper-0.0.4/setup.py` & `KofiPyQtHelper-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KofiPyQtHelper",
-    version="0.0.4",
+    version="0.0.5",
     author="Kofi",
     author_email="aliwkxqq@163.com",
     description="PyQt 的快速布局工具",
     long_description=long_description,
     license="BSD License",
     packages=find_packages(),
     # data_files=[("Lib/site-packages/your-module-name", ["file"])],
```

