# Comparing `tmp/yplib-2.4.4.tar.gz` & `tmp/yplib-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.4.tar", last modified: Tue Jul 11 01:18:31 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.5.tar", last modified: Tue Jul 11 01:49:15 2023, max compression
```

## Comparing `yplib-2.4.4.tar` & `yplib-2.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-11 01:18:31.113425 yplib-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 01:18:31.113425 yplib-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-11 01:17:42.000000 yplib-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.4/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.4/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    32701 2023-07-11 00:29:24.000000 yplib-2.4.4/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.4/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.4/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.4/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:18:31.113425 yplib-2.4.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 01:18:30.000000 yplib-2.4.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.616605 yplib-2.4.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-11 01:49:15.616104 yplib-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:49:15.616605 yplib-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-11 01:48:58.000000 yplib-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.610450 yplib-2.4.5/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.5/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.5/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32960 2023-07-11 01:48:35.000000 yplib-2.4.5/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.5/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.5/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.5/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:49:15.615104 yplib-2.4.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 01:49:15.000000 yplib-2.4.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.4/LICENSE` & `yplib-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/setup.py` & `yplib-2.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.4",
+  version="2.4.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.4/yplib/__init__.py` & `yplib-2.4.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/chart.py` & `yplib-2.4.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/chart_html.py` & `yplib-2.4.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/db.py` & `yplib-2.4.5/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/file.py` & `yplib-2.4.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/http_util.py` & `yplib-2.4.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/index.py` & `yplib-2.4.5/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,23 +233,29 @@
     s = re.sub(r'\D', '', str(s))
     # s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
     # @see https://www.runoob.com/python3/python3-reg-expressions.html
     return 0 if s == '' else int(s)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 float
-def to_float(s):
+# precision , 小数部位的长度 , 多余的部分 直接去掉
+def to_float(s, precision=None):
     if isinstance(s, float):
         return s
     if s is None or s == '':
         return 0.0
     # s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
     # @see https://www.runoob.com/python3/python3-reg-expressions.html
     s = re.sub('[^0-9.]', '', str(s))
-    return 0.0 if s == '' else float(s)
+    if s == '':
+        return 0.0
+    if precision is None:
+        return float(s)
+    s1 = s.split('.')
+    return float(s1[0] + '.' + s1[1][0:len(s1[1]) if len(s1[1]) < int(precision) else int(precision)])
 
 
 # 将字符串 s 转化成 datetime
 def to_datetime(s=None, r_str=False):
     if s is None or s == '':
         return str(datetime.today()) if r_str else datetime.today()
     s = str(s)
```

### Comparing `yplib-2.4.4/yplib/mail.py` & `yplib-2.4.5/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/mail_html.py` & `yplib-2.4.5/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.4/yplib/markdown.py` & `yplib-2.4.5/yplib/markdown.py`

 * *Files identical despite different names*

