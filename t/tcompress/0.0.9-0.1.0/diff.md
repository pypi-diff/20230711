# Comparing `tmp/tcompress-0.0.9.tar.gz` & `tmp/tcompress-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcompress-0.0.9.tar", last modified: Tue Jul 11 01:23:30 2023, max compression
+gzip compressed data, was "tcompress-0.1.0.tar", last modified: Tue Jul 11 01:27:14 2023, max compression
```

## Comparing `tcompress-0.0.9.tar` & `tcompress-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.357392 tcompress-0.0.9/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.9/LICENSE
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:23:30.357465 tcompress-0.0.9/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.0.9/README.md
--rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.9/pyproject.toml
--rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 01:23:30.357729 tcompress-0.0.9/setup.cfg
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.354092 tcompress-0.0.9/src/
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.356380 tcompress-0.0.9/src/tcompress/
--rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.0.9/src/tcompress/__init__.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.0.9/src/tcompress/image.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.0.9/src/tcompress/main.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1499 2023-07-03 04:09:16.000000 tcompress-0.0.9/src/tcompress/manage.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.0.9/src/tcompress/random.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.0.9/src/tcompress/time.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.357277 tcompress-0.0.9/src/tcompress.egg-info/
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/SOURCES.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/dependency_links.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/top_level.txt
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.045592 tcompress-0.1.0/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.1.0/LICENSE
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:27:14.045676 tcompress-0.1.0/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.1.0/README.md
+-rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.1.0/pyproject.toml
+-rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 01:27:14.045959 tcompress-0.1.0/setup.cfg
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.042214 tcompress-0.1.0/src/
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.044533 tcompress-0.1.0/src/tcompress/
+-rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.1.0/src/tcompress/__init__.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.1.0/src/tcompress/image.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.1.0/src/tcompress/main.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1541 2023-07-11 01:26:20.000000 tcompress-0.1.0/src/tcompress/manage.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.1.0/src/tcompress/random.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.1.0/src/tcompress/time.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.045415 tcompress-0.1.0/src/tcompress.egg-info/
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/top_level.txt
```

### Comparing `tcompress-0.0.9/PKG-INFO` & `tcompress-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcompress
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/talalzeini/compress
 Author: Talal El Zeini
 Author-email: talalelzeini@gmail.com
 Project-URL: Bug Tracker, https://github.com/talalzeini/compress/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tcompress-0.0.9/README.md` & `tcompress-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.9/setup.cfg` & `tcompress-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tcompress
-version = 0.0.9
+version = 0.1.0
 author = Talal El Zeini
 author_email = talalelzeini@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/talalzeini/compress
 project_urls =
```

### Comparing `tcompress-0.0.9/src/tcompress/image.py` & `tcompress-0.1.0/src/tcompress/image.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.9/src/tcompress/main.py` & `tcompress-0.1.0/src/tcompress/main.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.9/src/tcompress/manage.py` & `tcompress-0.1.0/src/tcompress/manage.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 def get_file_extension(file_path):
     return get_file_info(file_path)[1]
 
 def get_file_location(file_path):
     return get_file_info(file_path)[2]
 
-def is_file(path):
-    return path.isfile(path)
+def is_file(path_string):
+    return path.isfile(path_string)
           
-def is_folder(path):
-    return path.isdir(path)
+def is_folder(path_string):
+    return path.isdir(path_string)
 
-def is_existing(path):
-    return path.exists(path) 
+def is_existing(path_string):
+    return path.exists(path_string) 
 
 def list_directories(folder_path):
     return [
         d for d in (path.join(folder_path, d1) for d1 in listdir(folder_path))
         if path.isdir(d)
     ]
```

### Comparing `tcompress-0.0.9/src/tcompress/random.py` & `tcompress-0.1.0/src/tcompress/random.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.9/src/tcompress/time.py` & `tcompress-0.1.0/src/tcompress/time.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.9/src/tcompress.egg-info/PKG-INFO` & `tcompress-0.1.0/src/tcompress.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcompress
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/talalzeini/compress
 Author: Talal El Zeini
 Author-email: talalelzeini@gmail.com
 Project-URL: Bug Tracker, https://github.com/talalzeini/compress/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

