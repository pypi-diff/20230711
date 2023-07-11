# Comparing `tmp/mercari-2.0.0.tar.gz` & `tmp/mercari-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercari-2.0.0.tar", last modified: Mon Jul 10 17:34:55 2023, max compression
+gzip compressed data, was "mercari-2.0.1.tar", last modified: Tue Jul 11 14:33:02 2023, max compression
```

## Comparing `mercari-2.0.0.tar` & `mercari-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.730478 mercari-2.0.0/
--rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-06-05 23:48:30.000000 mercari-2.0.0/MANIFEST.in
--rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-10 17:34:55.730363 mercari-2.0.0/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)     1665 2023-07-10 17:32:18.000000 mercari-2.0.0/README.md
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.729215 mercari-2.0.0/mercari/
--rw-r--r--   0 batmanuel   (501) staff       (20)     3750 2022-06-05 23:48:30.000000 mercari-2.0.0/mercari/DpopUtils.py
--rw-r--r--   0 batmanuel   (501) staff       (20)       95 2023-07-10 17:28:22.000000 mercari-2.0.0/mercari/__init__.py
--rw-r--r--   0 batmanuel   (501) staff       (20)     4407 2023-07-10 17:32:38.000000 mercari-2.0.0/mercari/mercari.py
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.730207 mercari-2.0.0/mercari.egg-info/
--rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)      261 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/SOURCES.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/dependency_links.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/requires.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        8 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/top_level.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-10 17:23:15.000000 mercari-2.0.0/requirements.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-07-10 17:34:55.730515 mercari-2.0.0/setup.cfg
--rw-r--r--   0 batmanuel   (501) staff       (20)      663 2023-07-10 17:28:22.000000 mercari-2.0.0/setup.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-11 14:33:02.364056 mercari-2.0.1/
+-rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-06-05 23:48:30.000000 mercari-2.0.1/MANIFEST.in
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-11 14:33:02.363927 mercari-2.0.1/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1665 2023-07-11 14:28:45.000000 mercari-2.0.1/README.md
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-11 14:33:02.362969 mercari-2.0.1/mercari/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     3750 2022-06-05 23:48:30.000000 mercari-2.0.1/mercari/DpopUtils.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)       95 2023-07-11 14:28:45.000000 mercari-2.0.1/mercari/__init__.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)     4407 2023-07-11 14:31:58.000000 mercari-2.0.1/mercari/mercari.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-11 14:33:02.363766 mercari-2.0.1/mercari.egg-info/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-11 14:33:02.000000 mercari-2.0.1/mercari.egg-info/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)      261 2023-07-11 14:33:02.000000 mercari-2.0.1/mercari.egg-info/SOURCES.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-07-11 14:33:02.000000 mercari-2.0.1/mercari.egg-info/dependency_links.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-11 14:33:02.000000 mercari-2.0.1/mercari.egg-info/requires.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        8 2023-07-11 14:33:02.000000 mercari-2.0.1/mercari.egg-info/top_level.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-10 17:23:15.000000 mercari-2.0.1/requirements.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-07-11 14:33:02.364096 mercari-2.0.1/setup.cfg
+-rw-r--r--   0 batmanuel   (501) staff       (20)      663 2023-07-11 14:32:29.000000 mercari-2.0.1/setup.py
```

### Comparing `mercari-2.0.0/PKG-INFO` & `mercari-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercari
-Version: 2.0.0
+Version: 2.0.1
 Summary: mercari api-like wrapper
 Home-page: https://github.com/marvinody/mercari/
 Author: marvinody
 Author-email: manny@sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercari-2.0.0/README.md` & `mercari-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mercari-2.0.0/mercari/DpopUtils.py` & `mercari-2.0.1/mercari/DpopUtils.py`

 * *Files identical despite different names*

### Comparing `mercari-2.0.0/mercari/mercari.py` & `mercari-2.0.1/mercari/mercari.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     # This is per page and not for the final result
     limit = 120
 
     data = {
         # this seems to be random, but we'll add a prefix for mercari to track if they wanted to
         "userId": "MERCARI_BOT_{}".format(uuid.uuid4()), 
         "pageSize": limit,
-        "pageToken": pageToPageToken(1),
+        "pageToken": pageToPageToken(0),
         # same thing as userId, courtesy of a prefix for mercari
         "searchSessionId": "MERCARI_BOT_{}".format(uuid.uuid4()),
         # this is hardcoded in their frontend currently, so leaving it
         "indexRouting": "INDEX_ROUTING_UNSPECIFIED",
         "searchCondition": {
             "keyword": keywords,
             "sort": sort,
```

### Comparing `mercari-2.0.0/mercari.egg-info/PKG-INFO` & `mercari-2.0.1/mercari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercari
-Version: 2.0.0
+Version: 2.0.1
 Summary: mercari api-like wrapper
 Home-page: https://github.com/marvinody/mercari/
 Author: marvinody
 Author-email: manny@sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercari-2.0.0/setup.py` & `mercari-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mercari',
-    version='2.0.0',
+    version='2.0.1',
     author='marvinody',
     author_email='manny@sadpanda.moe',
     description='mercari api-like wrapper',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/marvinody/mercari/',
     packages=setuptools.find_packages(),
```

