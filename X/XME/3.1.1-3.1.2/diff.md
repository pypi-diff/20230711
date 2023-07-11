# Comparing `tmp/XME-3.1.1.tar.gz` & `tmp/XME-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XME-3.1.1.tar", last modified: Tue Jul 11 09:28:53 2023, max compression
+gzip compressed data, was "XME-3.1.2.tar", last modified: Tue Jul 11 09:32:54 2023, max compression
```

## Comparing `XME-3.1.1.tar` & `XME-3.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:28:53.210240 XME-3.1.1/
--rw-rw-rw-   0        0        0     1527 2023-07-08 14:55:51.000000 XME-3.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3547 2023-07-11 09:28:53.209239 XME-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2023-07-11 09:16:04.000000 XME-3.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 09:28:53.190235 XME-3.1.1/XME/
-drwxrwxrwx   0        0        0        0 2023-07-11 09:28:53.207239 XME-3.1.1/XME/XMElib/
--rw-rw-rw-   0        0        0     1661 2023-07-08 10:05:12.000000 XME-3.1.1/XME/XMElib/ArrayOperator.py
--rw-rw-rw-   0        0        0     3640 2023-07-04 02:14:30.000000 XME-3.1.1/XME/XMElib/Executor.py
--rw-rw-rw-   0        0        0     1959 2023-07-08 15:35:32.000000 XME-3.1.1/XME/XMElib/Logputter.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:19:50.000000 XME-3.1.1/XME/XMElib/__init__.py
--rw-rw-rw-   0        0        0       75 2023-07-11 09:28:38.000000 XME-3.1.1/XME/XMElib/version_info.py
--rw-rw-rw-   0        0        0     2357 2023-07-11 09:28:06.000000 XME-3.1.1/XME/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:28:53.198237 XME-3.1.1/XME.egg-info/
--rw-rw-rw-   0        0        0     3547 2023-07-11 09:28:53.000000 XME-3.1.1/XME.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-11 09:28:53.000000 XME-3.1.1/XME.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:28:53.000000 XME-3.1.1/XME.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 09:28:53.000000 XME-3.1.1/XME.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 09:28:53.210240 XME-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-11 09:28:28.000000 XME-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:32:54.636763 XME-3.1.2/
+-rw-rw-rw-   0        0        0     1527 2023-07-08 14:55:51.000000 XME-3.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3547 2023-07-11 09:32:54.635763 XME-3.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2023-07-11 09:16:04.000000 XME-3.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 09:32:54.616759 XME-3.1.2/XME/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:32:54.633763 XME-3.1.2/XME/XMElib/
+-rw-rw-rw-   0        0        0     1661 2023-07-08 10:05:12.000000 XME-3.1.2/XME/XMElib/ArrayOperator.py
+-rw-rw-rw-   0        0        0     3640 2023-07-04 02:14:30.000000 XME-3.1.2/XME/XMElib/Executor.py
+-rw-rw-rw-   0        0        0     1959 2023-07-08 15:35:32.000000 XME-3.1.2/XME/XMElib/Logputter.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:19:50.000000 XME-3.1.2/XME/XMElib/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-07-11 09:32:21.000000 XME-3.1.2/XME/XMElib/version_info.py
+-rw-rw-rw-   0        0        0     2357 2023-07-11 09:28:06.000000 XME-3.1.2/XME/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:32:54.623760 XME-3.1.2/XME.egg-info/
+-rw-rw-rw-   0        0        0     3547 2023-07-11 09:32:54.000000 XME-3.1.2/XME.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-11 09:32:54.000000 XME-3.1.2/XME.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:32:54.000000 XME-3.1.2/XME.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 09:32:54.000000 XME-3.1.2/XME.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:32:54.636763 XME-3.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-11 09:31:56.000000 XME-3.1.2/setup.py
```

### Comparing `XME-3.1.1/LICENSE.txt` & `XME-3.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/PKG-INFO` & `XME-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XME
-Version: 3.1.1
+Version: 3.1.2
 Summary: This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 Home-page: https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine
 Author: Junxiang Huang & Weihui Li
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XME-3.1.1/README.md` & `XME-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/XME/XMElib/ArrayOperator.py` & `XME-3.1.2/XME/XMElib/ArrayOperator.py`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/XME/XMElib/Executor.py` & `XME-3.1.2/XME/XMElib/Executor.py`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/XME/XMElib/Logputter.py` & `XME-3.1.2/XME/XMElib/Logputter.py`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/XME/__init__.py` & `XME-3.1.2/XME/__init__.py`

 * *Files identical despite different names*

### Comparing `XME-3.1.1/XME.egg-info/PKG-INFO` & `XME-3.1.2/XME.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XME
-Version: 3.1.1
+Version: 3.1.2
 Summary: This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 Home-page: https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine
 Author: Junxiang Huang & Weihui Li
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XME-3.1.1/setup.py` & `XME-3.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="XME",
-    version="3.1.1",
+    version="3.1.2",
     author="Junxiang Huang & Weihui Li",
     author_email="huangjunxiang@mail.ynu.edu.cn",
     description="This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine", 
     packages=setuptools.find_packages(),
```

