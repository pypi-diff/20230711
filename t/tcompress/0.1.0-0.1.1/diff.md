# Comparing `tmp/tcompress-0.1.0.tar.gz` & `tmp/tcompress-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcompress-0.1.0.tar", last modified: Tue Jul 11 01:27:14 2023, max compression
+gzip compressed data, was "tcompress-0.1.1.tar", last modified: Tue Jul 11 02:32:32 2023, max compression
```

## Comparing `tcompress-0.1.0.tar` & `tcompress-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.045592 tcompress-0.1.0/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.1.0/LICENSE
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:27:14.045676 tcompress-0.1.0/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      554 2023-07-03 03:43:08.000000 tcompress-0.1.0/README.md
--rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.1.0/pyproject.toml
--rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 01:27:14.045959 tcompress-0.1.0/setup.cfg
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.042214 tcompress-0.1.0/src/
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.044533 tcompress-0.1.0/src/tcompress/
--rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.1.0/src/tcompress/__init__.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.1.0/src/tcompress/image.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.1.0/src/tcompress/main.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1541 2023-07-11 01:26:20.000000 tcompress-0.1.0/src/tcompress/manage.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.1.0/src/tcompress/random.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.1.0/src/tcompress/time.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 01:27:14.045415 tcompress-0.1.0/src/tcompress.egg-info/
--rw-r--r--   0 talalzeini   (501) staff       (20)     1054 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/SOURCES.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/dependency_links.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 01:27:14.000000 tcompress-0.1.0/src/tcompress.egg-info/top_level.txt
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 02:32:32.894482 tcompress-0.1.1/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.1.1/LICENSE
+-rw-r--r--   0 talalzeini   (501) staff       (20)     3080 2023-07-11 02:32:32.894547 tcompress-0.1.1/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)     2580 2023-07-11 02:31:49.000000 tcompress-0.1.1/README.md
+-rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.1.1/pyproject.toml
+-rw-r--r--   0 talalzeini   (501) staff       (20)      629 2023-07-11 02:32:32.894814 tcompress-0.1.1/setup.cfg
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 02:32:32.891325 tcompress-0.1.1/src/
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 02:32:32.893628 tcompress-0.1.1/src/tcompress/
+-rw-r--r--   0 talalzeini   (501) staff       (20)      149 2023-07-11 01:00:16.000000 tcompress-0.1.1/src/tcompress/__init__.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     3586 2023-07-03 04:07:49.000000 tcompress-0.1.1/src/tcompress/image.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      921 2023-07-03 03:58:14.000000 tcompress-0.1.1/src/tcompress/main.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1541 2023-07-11 01:26:20.000000 tcompress-0.1.1/src/tcompress/manage.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1350 2023-07-03 04:06:56.000000 tcompress-0.1.1/src/tcompress/random.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1321 2023-07-03 03:37:37.000000 tcompress-0.1.1/src/tcompress/time.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-07-11 02:32:32.894355 tcompress-0.1.1/src/tcompress.egg-info/
+-rw-r--r--   0 talalzeini   (501) staff       (20)     3080 2023-07-11 02:32:32.000000 tcompress-0.1.1/src/tcompress.egg-info/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      331 2023-07-11 02:32:32.000000 tcompress-0.1.1/src/tcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-07-11 02:32:32.000000 tcompress-0.1.1/src/tcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-07-11 02:32:32.000000 tcompress-0.1.1/src/tcompress.egg-info/top_level.txt
```

### Comparing `tcompress-0.1.0/setup.cfg` & `tcompress-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tcompress
-version = 0.1.0
+version = 0.1.1
 author = Talal El Zeini
 author_email = talalelzeini@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/talalzeini/compress
 project_urls =
```

### Comparing `tcompress-0.1.0/src/tcompress/image.py` & `tcompress-0.1.1/src/tcompress/image.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.1.0/src/tcompress/main.py` & `tcompress-0.1.1/src/tcompress/main.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.1.0/src/tcompress/manage.py` & `tcompress-0.1.1/src/tcompress/manage.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.1.0/src/tcompress/random.py` & `tcompress-0.1.1/src/tcompress/random.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.1.0/src/tcompress/time.py` & `tcompress-0.1.1/src/tcompress/time.py`

 * *Files identical despite different names*

