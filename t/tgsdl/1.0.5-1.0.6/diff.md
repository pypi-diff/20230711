# Comparing `tmp/tgsdl-1.0.5.tar.gz` & `tmp/tgsdl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgsdl-1.0.5.tar", last modified: Sun Jun 18 16:37:33 2023, max compression
+gzip compressed data, was "tgsdl-1.0.6.tar", last modified: Tue Jul 11 18:24:48 2023, max compression
```

## Comparing `tgsdl-1.0.5.tar` & `tgsdl-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 16:37:25.000000 tgsdl-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 16:37:25.000000 tgsdl-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 16:37:33.582695 tgsdl-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-18 16:37:25.000000 tgsdl-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:37:33.582695 tgsdl-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-18 16:37:25.000000 tgsdl-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/tgsdl/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:37:25.000000 tgsdl-1.0.5/tgsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-18 16:37:25.000000 tgsdl-1.0.5/tgsdl/tgsdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/tgsdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:24:48.292718 tgsdl-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 18:24:38.000000 tgsdl-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 18:24:38.000000 tgsdl-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 18:24:48.292718 tgsdl-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 18:24:38.000000 tgsdl-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:24:48.292718 tgsdl-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 18:24:38.000000 tgsdl-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:24:48.292718 tgsdl-1.0.6/tgsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 18:24:38.000000 tgsdl-1.0.6/tgsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-11 18:24:38.000000 tgsdl-1.0.6/tgsdl/tgsdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:24:48.292718 tgsdl-1.0.6/tgsdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 18:24:48.000000 tgsdl-1.0.6/tgsdl.egg-info/top_level.txt
```

### Comparing `tgsdl-1.0.5/LICENSE` & `tgsdl-1.0.6/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Bevlill
+Copyright (c) 2023 OneFinalHug
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tgsdl-1.0.5/PKG-INFO` & `tgsdl-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.5
+Version: 1.0.6
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
 Author: Bevlill
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tgsdl-1.0.5/README.md` & `tgsdl-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tgsdl-1.0.5/setup.py` & `tgsdl-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 readme_path = os.path.join(current_dir, 'README.md')
 
 setup(
     name='tgsdl',
-    version='1.0.5',
+    version='1.0.6',
     description='Telegram Sticker Pack Downloader Library',
     author='Bevlill',
     author_email='voidlillis@gmail.com',
     url='https://github.com/lillisfeb/TGSDL/',
     long_description = open(readme_path).read(),
     long_description_content_type='text/markdown',
     keywords=['telegram', 'bot', 'sticker', 'download', 'stickerpack'],
```

### Comparing `tgsdl-1.0.5/tgsdl/tgsdl.py` & `tgsdl-1.0.6/tgsdl/tgsdl.py`

 * *Files identical despite different names*

### Comparing `tgsdl-1.0.5/tgsdl.egg-info/PKG-INFO` & `tgsdl-1.0.6/tgsdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.5
+Version: 1.0.6
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
 Author: Bevlill
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
```

