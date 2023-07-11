# Comparing `tmp/to_tmx-1.0.2.tar.gz` & `tmp/to_tmx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alexskrn/Documents/NLP/to_tmx/dist/tmp8tsv29ex/to_tmx-1.0.2.tar", last modified: Tue Jul 11 17:42:26 2023, max compression
+gzip compressed data, was "/Users/alexskrn/Documents/NLP/to_tmx/dist/tmpko0i0e12/to_tmx-1.0.3.tar", last modified: Tue Jul 11 17:52:10 2023, max compression
```

## Comparing `to_tmx-1.0.2.tar` & `to_tmx-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/
--rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:42:26.000000 to_tmx-1.0.2/PKG-INFO
--rw-r--r--   0 alexskrn   (502) staff       (20)       65 2020-07-10 16:28:04.000000 to_tmx-1.0.2/requirements.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)      135 2023-07-11 17:13:12.000000 to_tmx-1.0.2/MANIFEST.in
-drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/
--rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/PKG-INFO
--rw-r--r--   0 alexskrn   (502) staff       (20)      342 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/SOURCES.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)      183 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/entry_points.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)       64 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/requires.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)        7 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/top_level.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)        1 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/dependency_links.txt
--rw-r--r--   0 alexskrn   (502) staff       (20)     1625 2023-07-11 17:23:08.000000 to_tmx-1.0.2/setup.py
-drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx/
--rw-r--r--   0 alexskrn   (502) staff       (20)     2524 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/tmx_batch_tradosizer.py
--rw-r--r--   0 alexskrn   (502) staff       (20)     4638 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/to_tmx.py
--rw-r--r--   0 alexskrn   (502) staff       (20)     3890 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/tmx_tradosizer.py
--rw-r--r--   0 alexskrn   (502) staff       (20)        0 2020-07-10 16:28:04.000000 to_tmx-1.0.2/to_tmx/__init__.py
--rw-r--r--   0 alexskrn   (502) staff       (20)     1499 2020-07-10 16:28:04.000000 to_tmx-1.0.2/to_tmx/sent_tok.py
--rw-r--r--   0 alexskrn   (502) staff       (20)       38 2023-07-11 17:42:26.000000 to_tmx-1.0.2/setup.cfg
--rw-r--r--   0 alexskrn   (502) staff       (20)     1065 2023-07-11 17:13:12.000000 to_tmx-1.0.2/LICENSE.txt
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:52:10.000000 to_tmx-1.0.3/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:52:10.000000 to_tmx-1.0.3/PKG-INFO
+-rw-r--r--   0 alexskrn   (502) staff       (20)       44 2023-07-11 17:48:26.000000 to_tmx-1.0.3/requirements.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)      135 2023-07-11 17:13:12.000000 to_tmx-1.0.3/MANIFEST.in
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/PKG-INFO
+-rw-r--r--   0 alexskrn   (502) staff       (20)      342 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/SOURCES.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)      183 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/entry_points.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)       43 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/requires.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)        7 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/top_level.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)        1 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx.egg-info/dependency_links.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1625 2023-07-11 17:50:46.000000 to_tmx-1.0.3/setup.py
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:52:10.000000 to_tmx-1.0.3/to_tmx/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     2524 2023-07-11 17:13:12.000000 to_tmx-1.0.3/to_tmx/tmx_batch_tradosizer.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4638 2023-07-11 17:13:12.000000 to_tmx-1.0.3/to_tmx/to_tmx.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     3890 2023-07-11 17:13:12.000000 to_tmx-1.0.3/to_tmx/tmx_tradosizer.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)        0 2020-07-10 16:28:04.000000 to_tmx-1.0.3/to_tmx/__init__.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1499 2020-07-10 16:28:04.000000 to_tmx-1.0.3/to_tmx/sent_tok.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)       38 2023-07-11 17:52:10.000000 to_tmx-1.0.3/setup.cfg
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1065 2023-07-11 17:13:12.000000 to_tmx-1.0.3/LICENSE.txt
```

### Comparing `to_tmx-1.0.2/PKG-INFO` & `to_tmx-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to_tmx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Txt-to-tmx file converter.
 Home-page: https://github.com/AlexSkrn/to_tmx
 Author: AlexSkrn
 Author-email: alex.g.skrn@gmail.com
 License: MIT
 Keywords: tmx converter
 Platform: UNKNOWN
```

### Comparing `to_tmx-1.0.2/to_tmx.egg-info/PKG-INFO` & `to_tmx-1.0.3/to_tmx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-tmx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Txt-to-tmx file converter.
 Home-page: https://github.com/AlexSkrn/to_tmx
 Author: AlexSkrn
 Author-email: alex.g.skrn@gmail.com
 License: MIT
 Keywords: tmx converter
 Platform: UNKNOWN
```

### Comparing `to_tmx-1.0.2/setup.py` & `to_tmx-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 
 setuptools.setup(
     name=NAME,
-    version='1.0.2',
+    version='1.0.3',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `to_tmx-1.0.2/to_tmx/tmx_batch_tradosizer.py` & `to_tmx-1.0.3/to_tmx/tmx_batch_tradosizer.py`

 * *Files identical despite different names*

### Comparing `to_tmx-1.0.2/to_tmx/to_tmx.py` & `to_tmx-1.0.3/to_tmx/to_tmx.py`

 * *Files identical despite different names*

### Comparing `to_tmx-1.0.2/to_tmx/tmx_tradosizer.py` & `to_tmx-1.0.3/to_tmx/tmx_tradosizer.py`

 * *Files identical despite different names*

### Comparing `to_tmx-1.0.2/to_tmx/sent_tok.py` & `to_tmx-1.0.3/to_tmx/sent_tok.py`

 * *Files identical despite different names*

### Comparing `to_tmx-1.0.2/LICENSE.txt` & `to_tmx-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

