# Comparing `tmp/KofiPyQtHelper-0.0.2.tar.gz` & `tmp/KofiPyQtHelper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KofiPyQtHelper-0.0.2.tar", last modified: Tue Jul 11 09:31:46 2023, max compression
+gzip compressed data, was "dist/KofiPyQtHelper-0.0.3.tar", last modified: Tue Jul 11 09:40:38 2023, max compression
```

## Comparing `KofiPyQtHelper-0.0.2.tar` & `KofiPyQtHelper-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)      207 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/requires.txt
--rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/KofiPyQtHelper.egg-info/top_level.txt
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.2/README.md
--rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 09:31:46.000000 KofiPyQtHelper-0.0.2/setup.cfg
--rw-r--r--   0 kofi       (501) staff       (20)      890 2023-07-11 09:31:42.000000 KofiPyQtHelper-0.0.2/setup.py
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      207 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/requires.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/KofiPyQtHelper.egg-info/top_level.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.3/README.md
+-rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 09:40:38.000000 KofiPyQtHelper-0.0.3/setup.cfg
+-rw-r--r--   0 kofi       (501) staff       (20)      892 2023-07-11 09:39:19.000000 KofiPyQtHelper-0.0.3/setup.py
```

### Comparing `KofiPyQtHelper-0.0.2/setup.py` & `KofiPyQtHelper-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KofiPyQtHelper",
-    version="0.0.2",
+    version="0.0.3",
     author="Kofi",
     author_email="aliwkxqq@163.com",
     description="PyQt 的快速布局工具",
     long_description=long_description,
     license="BSD License",
     packages=find_packages(),
-    data_files=[("Lib/site-packages/your-module-name", ["file"])],
+    # data_files=[("Lib/site-packages/your-module-name", ["file"])],
     install_requires=[
         "Jinja2==3.1.2",
         "loguru==0.6.0",
         "matplotlib==3.5.3",
         "numpy==1.21.4",
         "pandas==1.3.4",
         "pdf2docx==0.5.6",
```

