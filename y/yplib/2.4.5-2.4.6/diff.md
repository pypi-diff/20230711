# Comparing `tmp/yplib-2.4.5.tar.gz` & `tmp/yplib-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.5.tar", last modified: Tue Jul 11 01:49:15 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.6.tar", last modified: Tue Jul 11 06:31:23 2023, max compression
```

## Comparing `yplib-2.4.5.tar` & `yplib-2.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.616605 yplib-2.4.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-11 01:49:15.616104 yplib-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 01:49:15.616605 yplib-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-11 01:48:58.000000 yplib-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.610450 yplib-2.4.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.5/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.5/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    32960 2023-07-11 01:48:35.000000 yplib-2.4.5/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.615104 yplib-2.4.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.328307 yplib-2.4.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-11 06:31:23.327700 yplib-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 06:31:23.328307 yplib-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-11 06:31:03.000000 yplib-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.316658 yplib-2.4.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.6/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32950 2023-07-11 06:30:56.000000 yplib-2.4.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.326877 yplib-2.4.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.5/LICENSE` & `yplib-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/setup.py` & `yplib-2.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.5",
+  version="2.4.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.5/yplib/__init__.py` & `yplib-2.4.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/chart.py` & `yplib-2.4.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/chart_html.py` & `yplib-2.4.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/db.py` & `yplib-2.4.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/file.py` & `yplib-2.4.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/http_util.py` & `yplib-2.4.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/index.py` & `yplib-2.4.6/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 def is_linux():
     return not is_win()
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
-    l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
-         a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
+    l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ' '.join(list(map(lambda x: json.dumps(x) if can_use_json(x) else str(x), l)))
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + d if time_prefix else d
     print(lo)
     return lo
 
 
 # 记录日志, 如果是对象会转化为 json
```

### Comparing `yplib-2.4.5/yplib/mail.py` & `yplib-2.4.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/mail_html.py` & `yplib-2.4.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.5/yplib/markdown.py` & `yplib-2.4.6/yplib/markdown.py`

 * *Files identical despite different names*

