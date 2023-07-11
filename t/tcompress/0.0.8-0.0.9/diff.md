# Comparing `tmp/tcompress-0.0.8.tar.gz` & `tmp/tcompress-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcompress-0.0.8.tar", last modified: Tue Jul 11 01:02:46 2023, max compression
+gzip compressed data, was "tcompress-0.0.9.tar", last modified: Tue Jul 11 01:23:30 2023, max compression
```

## Comparing `tcompress-0.0.8.tar` & `tcompress-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:02:46.901795 tcompress-0.0.8/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.8/LICENSE
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:02:46.901859 tcompress-0.0.8/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.0.8/README.md
--rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.8/pyproject.toml
--rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 01:02:46.902107 tcompress-0.0.8/setup.cfg
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:02:46.898674 tcompress-0.0.8/src/
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:02:46.900858 tcompress-0.0.8/src/tcompress/
--rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.0.8/src/tcompress/__init__.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.0.8/src/tcompress/image.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.0.8/src/tcompress/main.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1499 2023-07-03 04:09:16.000000 tcompress-0.0.8/src/tcompress/manage.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.0.8/src/tcompress/random.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.0.8/src/tcompress/time.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:02:46.901677 tcompress-0.0.8/src/tcompress.egg-info/
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:02:46.000000 tcompress-0.0.8/src/tcompress.egg-info/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 01:02:46.000000 tcompress-0.0.8/src/tcompress.egg-info/SOURCES.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 01:02:46.000000 tcompress-0.0.8/src/tcompress.egg-info/dependency_links.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 01:02:46.000000 tcompress-0.0.8/src/tcompress.egg-info/top_level.txt
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.357392 tcompress-0.0.9/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.9/LICENSE
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:23:30.357465 tcompress-0.0.9/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.0.9/README.md
+-rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.9/pyproject.toml
+-rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 01:23:30.357729 tcompress-0.0.9/setup.cfg
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.354092 tcompress-0.0.9/src/
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.356380 tcompress-0.0.9/src/tcompress/
+-rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.0.9/src/tcompress/__init__.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.0.9/src/tcompress/image.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.0.9/src/tcompress/main.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1499 2023-07-03 04:09:16.000000 tcompress-0.0.9/src/tcompress/manage.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.0.9/src/tcompress/random.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.0.9/src/tcompress/time.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:23:30.357277 tcompress-0.0.9/src/tcompress.egg-info/
+-rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 01:23:30.000000 tcompress-0.0.9/src/tcompress.egg-info/top_level.txt
```

### Comparing `tcompress-0.0.8/PKG-INFO` & `tcompress-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcompress
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/talalzeini/compress
 Author: Talal El Zeini
 Author-email: talalelzeini@gmail.com
 Project-URL: Bug Tracker, https://github.com/talalzeini/compress/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tcompress-0.0.8/README.md` & `tcompress-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/setup.cfg` & `tcompress-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tcompress
-version = 0.0.8
+version = 0.0.9
 author = Talal El Zeini
 author_email = talalelzeini@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/talalzeini/compress
 project_urls =
```

### Comparing `tcompress-0.0.8/src/tcompress/image.py` & `tcompress-0.0.9/src/tcompress/image.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/src/tcompress/main.py` & `tcompress-0.0.9/src/tcompress/main.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/src/tcompress/manage.py` & `tcompress-0.0.9/src/tcompress/manage.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/src/tcompress/random.py` & `tcompress-0.0.9/src/tcompress/random.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/src/tcompress/time.py` & `tcompress-0.0.9/src/tcompress/time.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.8/src/tcompress.egg-info/PKG-INFO` & `tcompress-0.0.9/src/tcompress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcompress
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/talalzeini/compress
 Author: Talal El Zeini
 Author-email: talalelzeini@gmail.com
 Project-URL: Bug Tracker, https://github.com/talalzeini/compress/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

