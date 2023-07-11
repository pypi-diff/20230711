# Comparing `tmp/yplib-2.4.2.tar.gz` & `tmp/yplib-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.2.tar", last modified: Mon Jul 10 08:52:52 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.3.tar", last modified: Tue Jul 11 00:31:56 2023, max compression
```

## Comparing `yplib-2.4.2.tar` & `yplib-2.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.302780 yplib-2.4.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 08:52:52.302220 yplib-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 08:52:52.302780 yplib-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 08:52:42.000000 yplib-2.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.298720 yplib-2.4.2/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.2/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.2/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.2/yplib/http_util.py
--rw-rw-rw-   0        0        0    32901 2023-07-10 08:52:07.000000 yplib-2.4.2/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.2/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.2/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.2/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.2/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.301163 yplib-2.4.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.833812 yplib-2.4.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-11 00:31:56.833144 yplib-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 00:31:56.833869 yplib-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-11 00:31:23.000000 yplib-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.829162 yplib-2.4.3/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.3/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.3/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32701 2023-07-11 00:29:24.000000 yplib-2.4.3/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.3/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.3/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.3/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.3/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 00:31:56.832197 yplib-2.4.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 00:31:56.000000 yplib-2.4.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.2/LICENSE` & `yplib-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/setup.py` & `yplib-2.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.2",
+  version="2.4.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.2/yplib/__init__.py` & `yplib-2.4.3/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/chart.py` & `yplib-2.4.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/chart_html.py` & `yplib-2.4.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/db.py` & `yplib-2.4.3/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/file.py` & `yplib-2.4.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/http_util.py` & `yplib-2.4.3/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/index.py` & `yplib-2.4.3/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,15 @@
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
-    d = ''
-    for one in l:
-        if can_use_json(one):
-            o = json.dumps(one)
-        else:
-            o = str(one)
-        if o != '':
-            if len(d):
-                d += ' '
-            d += o
+    d = ' '.join(list(map(lambda x: json.dumps(x) if can_use_json(x) else str(x), l)))
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + d if time_prefix else d
     print(lo)
     return lo
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_print(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
@@ -79,38 +70,29 @@
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
 def to_hump_one(s):
     if s is None or s == '':
         return s
-    s = str(s).lower()
-    s1 = s.split('_')
-    r = ""
-    for w in s1:
-        r += w.capitalize()
+    r = ''.join(list(map(lambda x: x.capitalize(), str(s).lower().split('_'))))
     return r[0].lower() + r[1:]
 
 
 def to_hump(s):
     if s is None or s == '':
         return s
     if isinstance(s, list) or isinstance(s, tuple) or isinstance(s, set):
-        rr = []
-        for ss in s:
-            rr.append(to_hump_one(ss))
-        return rr
+        return list(map(lambda x: to_hump_one(x), s))
     return to_hump_one(s)
 
 
-def to_hump_more(a1, a2, a3, a4, a5):
-    l = [a1, a2, a3, a4, a5]
-    r = []
-    for a in l:
-        r.append(to_hump(a))
+def to_hump_more(a1=None, a2=None, a3=None, a4=None, a5=None):
+    r = list(map(lambda x: to_hump(x), [a1, a2, a3, a4, a5]))
+    r = list(filter(lambda x: x is not None, r))
     if not len(r):
         return None
     if len(r) == 1:
         return r[0]
     if len(r) == 2:
         return r[0], r[1]
     if len(r) == 3:
@@ -122,39 +104,28 @@
 
 
 # 将驼峰命名转成下划线命名
 # 例如 : userId -> user_id
 def to_underline_one(s):
     if s == '' or s is None:
         return s
-    r = ''
-    for c in str(s):
-        if c.isupper():
-            r += '_' + c.lower()
-        else:
-            r += c
-    return r
+    return ''.join(list(map(lambda x: '_' + str(x).lower() if x.isupper() else x, str(s))))
 
 
 def to_underline(s):
     if s == '' or s is None:
         return s
     if isinstance(s, list) or isinstance(s, tuple) or isinstance(s, set):
-        rr = []
-        for ss in s:
-            rr.append(to_underline_one(ss))
-        return rr
+        return list(map(lambda x: to_underline_one(x), s))
     return to_underline_one(s)
 
 
-def to_underline_more(a1, a2, a3, a4, a5):
-    l = [a1, a2, a3, a4, a5]
-    r = []
-    for a in l:
-        r.append(to_underline(a))
+def to_underline_more(a1=None, a2=None, a3=None, a4=None, a5=None):
+    r = list(map(lambda x: to_underline(x), [a1, a2, a3, a4, a5]))
+    r = list(filter(lambda x: x is not None, r))
     if not len(r):
         return None
     if len(r) == 1:
         return r[0]
     if len(r) == 2:
         return r[0], r[1]
     if len(r) == 3:
@@ -255,15 +226,15 @@
 def to_int(s):
     if isinstance(s, int):
         return s
     if s is None or s == '':
         return 0
     if isinstance(s, float):
         return int(s)
-    s = re.sub(r'\D', "", str(s))
+    s = re.sub(r'\D', '', str(s))
     # s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
     # @see https://www.runoob.com/python3/python3-reg-expressions.html
     return 0 if s == '' else int(s)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 float
 def to_float(s):
@@ -567,15 +538,15 @@
         data_list.append(row_data)
     return data_list
 
 
 # 将一个文件中以空行作为分隔符,
 # 组成一个 list(list) 数据
 # 多行空行,自动合并到一行空行
-def to_list_from_txt_with_blank_row(file_name='a.txt'):
+def to_list_from_txt_with_blank_line(file_name='a.txt'):
     return to_list_from_txt(file_name, sep_line='')
 
 
 # 将 list 切分成 list(list)
 # 组成一个 list(list) 数据
 # 多行空行,自动合并到一行空行
 def to_list_list(data_list=[], count=10):
```

### Comparing `yplib-2.4.2/yplib/mail.py` & `yplib-2.4.3/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/mail_html.py` & `yplib-2.4.3/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.2/yplib/markdown.py` & `yplib-2.4.3/yplib/markdown.py`

 * *Files identical despite different names*

