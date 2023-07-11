# Comparing `tmp/tcompress-0.0.5.tar.gz` & `tmp/tcompress-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcompress-0.0.5.tar", last modified: Tue Jun 20 06:56:23 2023, max compression
+gzip compressed data, was "tcompress-0.0.6.tar", last modified: Tue Jul 11 00:44:49 2023, max compression
```

## Comparing `tcompress-0.0.5.tar` & `tcompress-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:56:23.604054 tcompress-0.0.5/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.5/LICENSE
--rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:56:23.604146 tcompress-0.0.5/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:08:04.000000 tcompress-0.0.5/README.md
--rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.5/pyproject.toml
--rw-r--r--   0 talalzeini   (501) staff       (20)      650 2023-06-20 06:56:23.604494 tcompress-0.0.5/setup.cfg
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:56:23.600376 tcompress-0.0.5/src/
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:56:23.601267 tcompress-0.0.5/src/tcompress/
--rw-r--r--   0 talalzeini   (501) staff       (20)      233 2023-06-20 06:56:11.000000 tcompress-0.0.5/src/tcompress/__init__.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:56:23.603814 tcompress-0.0.5/src/tcompress/functions/
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1924 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/functions/image.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      982 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/functions/main.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1504 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/functions/manage.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      498 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/functions/random.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      447 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/functions/time.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      500 2023-06-20 06:13:44.000000 tcompress-0.0.5/src/tcompress/installer.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:56:23.602406 tcompress-0.0.5/src/tcompress.egg-info/
--rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:56:23.000000 tcompress-0.0.5/src/tcompress.egg-info/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      408 2023-06-20 06:56:23.000000 tcompress-0.0.5/src/tcompress.egg-info/SOURCES.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-06-20 06:56:23.000000 tcompress-0.0.5/src/tcompress.egg-info/dependency_links.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-06-20 06:56:23.000000 tcompress-0.0.5/src/tcompress.egg-info/top_level.txt
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 00:44:49.311762 tcompress-0.0.6/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.6/LICENSE
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 00:44:49.311837 tcompress-0.0.6/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.0.6/README.md
+-rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.6/pyproject.toml
+-rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 00:44:49.312106 tcompress-0.0.6/setup.cfg
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 00:44:49.308585 tcompress-0.0.6/src/
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 00:44:49.310845 tcompress-0.0.6/src/tcompress/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-07-03 04:17:52.000000 tcompress-0.0.6/src/tcompress/__init__.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.0.6/src/tcompress/image.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.0.6/src/tcompress/main.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1499 2023-07-03 04:09:16.000000 tcompress-0.0.6/src/tcompress/manage.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.0.6/src/tcompress/random.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.0.6/src/tcompress/time.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 00:44:49.311650 tcompress-0.0.6/src/tcompress.egg-info/
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 00:44:49.000000 tcompress-0.0.6/src/tcompress.egg-info/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 00:44:49.000000 tcompress-0.0.6/src/tcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 00:44:49.000000 tcompress-0.0.6/src/tcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 00:44:49.000000 tcompress-0.0.6/src/tcompress.egg-info/top_level.txt
```

### Comparing `tcompress-0.0.5/setup.cfg` & `tcompress-0.0.6/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tcompress
-version = 0.0.5
+version = 0.0.6
 author = Talal El Zeini
 author_email = talalelzeini@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/talalzeini/compress
 project_urls = 
@@ -13,15 +13,15 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
-packages = tcompress, tcompress.functions
+packages = tcompress
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `tcompress-0.0.5/src/tcompress/functions/main.py` & `tcompress-0.0.6/src/tcompress/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import subprocess, platform, string
-from datetime import datetime
-from time import sleep
+import subprocess, platform
 
 def has_duplicates(lst):
     if len(lst) == len(set(lst)):
         return False
     else:
         return True
```

### Comparing `tcompress-0.0.5/src/tcompress/functions/manage.py` & `tcompress-0.0.6/src/tcompress/manage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
-import shutil 
+from os import path, listdir, remove
+from shutil import rmtree
 
 def read_lines(file_path):
     with open(file_path) as f:
             lines = f.readlines()
     return lines
 
 def count_lines(file_path):
@@ -12,15 +12,15 @@
 def count_folders(folder_path):
     return len(list_directories(folder_path))
 
 def count_files(folder_path):
     return len(list_files(folder_path))
 
 def get_file_info(file_path):
-    split_path = os.path.splitext(file_path)
+    split_path = path.splitext(file_path)
     file_name = file_path.split("/")[-1]
     file_extension = split_path[1]
     file_location = file_path.split("/" + file_name)[0]
     return [file_name, file_extension, file_location]
 
 def get_file_name(file_path):
     return get_file_info(file_path)[0]
@@ -28,32 +28,32 @@
 def get_file_extension(file_path):
     return get_file_info(file_path)[1]
 
 def get_file_location(file_path):
     return get_file_info(file_path)[2]
 
 def is_file(path):
-    return os.path.isfile(path)
+    return path.isfile(path)
           
 def is_folder(path):
-    return os.path.isdir(path)
+    return path.isdir(path)
 
 def is_existing(path):
-    return os.path.exists(path) 
+    return path.exists(path) 
 
 def list_directories(folder_path):
     return [
-        d for d in (os.path.join(folder_path, d1) for d1 in os.listdir(folder_path))
-        if os.path.isdir(d)
+        d for d in (path.join(folder_path, d1) for d1 in listdir(folder_path))
+        if path.isdir(d)
     ]
 
 def list_files(folder_path):
-    return [f for f in os.listdir(folder_path) if os.path.isfile(os.path.join(folder_path, f)) if f[0] != "."]
+    return [f for f in listdir(folder_path) if path.isfile(path.join(folder_path, f)) if f[0] != "."]
 
 def is_empty(folder_path):
-    return len(os.listdir(folder_path)) == 0
+    return len(listdir(folder_path)) == 0
 
 def delete_file(file_path):
-    os.remove(file_path)
+    remove(file_path)
 
 def delete_folder(folder_path):
-    shutil.rmtree(folder_path)
+    rmtree(folder_path)
```

