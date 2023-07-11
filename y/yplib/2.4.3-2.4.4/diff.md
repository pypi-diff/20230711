# Comparing `tmp/yplib-2.4.3.tar.gz` & `tmp/yplib-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.3.tar", last modified: Tue Jul 11 00:31:56 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.4.tar", last modified: Tue Jul 11 01:18:31 2023, max compression
```

## Comparing `yplib-2.4.3.tar` & `yplib-2.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.833812 yplib-2.4.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-11 00:31:56.833144 yplib-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 00:31:56.833869 yplib-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-11 00:31:23.000000 yplib-2.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.829162 yplib-2.4.3/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.3/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.3/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    32701 2023-07-11 00:29:24.000000 yplib-2.4.3/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.3/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.832197 yplib-2.4.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-11 01:18:31.113425 yplib-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:18:31.113425 yplib-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-11 01:17:42.000000 yplib-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.4/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.4/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32701 2023-07-11 00:29:24.000000 yplib-2.4.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.3/LICENSE` & `yplib-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/setup.py` & `yplib-2.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.3",
+  version="2.4.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.3/yplib/__init__.py` & `yplib-2.4.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/chart.py` & `yplib-2.4.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/chart_html.py` & `yplib-2.4.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/db.py` & `yplib-2.4.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/file.py` & `yplib-2.4.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/index.py` & `yplib-2.4.4/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/mail.py` & `yplib-2.4.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/mail_html.py` & `yplib-2.4.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.3/yplib/markdown.py` & `yplib-2.4.4/yplib/markdown.py`

 * *Files identical despite different names*

