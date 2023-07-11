# Comparing `tmp/cohost-0.3.0.tar.gz` & `tmp/cohost-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohost-0.3.0.tar", last modified: Wed Jul  5 01:29:26 2023, max compression
+gzip compressed data, was "cohost-0.3.1.tar", last modified: Tue Jul 11 04:08:09 2023, max compression
```

## Comparing `cohost-0.3.0.tar` & `cohost-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.798351 cohost-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 01:29:17.000000 cohost-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 01:29:26.798351 cohost-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-05 01:29:17.000000 cohost-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.794351 cohost-0.3.0/cohost/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.798351 cohost-0.3.0/cohost/models/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.794351 cohost-0.3.0/cohost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-05 01:29:17.000000 cohost-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:29:26.798351 cohost-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 04:07:59.000000 cohost-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-11 04:08:09.369651 cohost-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-11 04:07:59.000000 cohost-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 04:07:59.000000 cohost-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:08:09.369651 cohost-0.3.1/setup.cfg
```

### Comparing `cohost-0.3.0/LICENSE` & `cohost-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/PKG-INFO` & `cohost-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.3.0/README.md` & `cohost-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost/models/block.py` & `cohost-0.3.1/cohost/models/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         elif (self.filename.lower().endswith('.jpg')
               or self.filename.lower().endswith('.jpeg')):
             content_type = 'image/jpeg'
         elif self.filename.lower().endswith('.png'):
             content_type = 'image/png'
         elif self.filename.lower().endswith('.svg'):
             content_type = 'image/svg+xml'
+        elif self.filename.lower().endswith('.gif'):
+            content_type = 'image/gif'
         self.content_type = content_type
         with open(self.filepath, 'rb') as f:
             content_length = len(f.read())
         self.content_length = content_length
         self.attachment_id = attachment_id
         self.alt_text = alt_text
```

### Comparing `cohost-0.3.0/cohost/models/notification.py` & `cohost-0.3.1/cohost/models/notification.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost/models/post.py` & `cohost-0.3.1/cohost/models/post.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost/models/project.py` & `cohost-0.3.1/cohost/models/project.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost/models/user.py` & `cohost-0.3.1/cohost/models/user.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost/network.py` & `cohost-0.3.1/cohost/network.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.0/cohost.egg-info/PKG-INFO` & `cohost-0.3.1/cohost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.3.0/pyproject.toml` & `cohost-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cohost"
-version = "0.3.0"
+version = "0.3.1"
 description = "Unofficial Python API wrapper for Cohost.org - the fourth website!"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = [ "cohost.org", "cohost", "api" ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

