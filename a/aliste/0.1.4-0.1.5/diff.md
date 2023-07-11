# Comparing `tmp/aliste-0.1.4.tar.gz` & `tmp/aliste-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliste-0.1.4.tar", last modified: Tue Jul 11 15:19:04 2023, max compression
+gzip compressed data, was "aliste-0.1.5.tar", last modified: Tue Jul 11 15:35:00 2023, max compression
```

## Comparing `aliste-0.1.4.tar` & `aliste-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 15:19:04.301647 aliste-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-07-11 08:03:48.000000 aliste-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      763 2023-07-11 15:19:04.299678 aliste-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 15:19:04.284667 aliste-0.1.4/aliste/
--rw-rw-rw-   0        0        0       26 2023-07-11 13:34:58.000000 aliste-0.1.4/aliste/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-07-11 15:18:28.000000 aliste-0.1.4/aliste/broker.py
--rw-rw-rw-   0        0        0      344 2023-07-11 13:12:35.000000 aliste-0.1.4/aliste/constants.py
--rw-rw-rw-   0        0        0     1948 2023-07-11 14:41:53.000000 aliste-0.1.4/aliste/device.py
--rw-rw-rw-   0        0        0      145 2023-07-11 11:16:10.000000 aliste-0.1.4/aliste/enums.py
--rw-rw-rw-   0        0        0      346 2023-07-11 13:20:17.000000 aliste-0.1.4/aliste/home.py
--rw-rw-rw-   0        0        0     2628 2023-07-11 15:18:00.000000 aliste-0.1.4/aliste/hub.py
--rw-rw-rw-   0        0        0      353 2023-07-11 11:01:22.000000 aliste-0.1.4/aliste/user.py
--rw-rw-rw-   0        0        0      217 2023-07-11 11:43:02.000000 aliste-0.1.4/aliste/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:19:04.299678 aliste-0.1.4/aliste.egg-info/
--rw-rw-rw-   0        0        0      763 2023-07-11 15:19:04.000000 aliste-0.1.4/aliste.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-11 15:19:04.000000 aliste-0.1.4/aliste.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 15:19:04.000000 aliste-0.1.4/aliste.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 15:19:04.000000 aliste-0.1.4/aliste.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 15:19:04.301647 aliste-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-07-11 15:19:02.000000 aliste-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:35:00.209496 aliste-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2023-07-11 08:03:48.000000 aliste-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      763 2023-07-11 15:35:00.208897 aliste-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 15:35:00.192299 aliste-0.1.5/aliste/
+-rw-rw-rw-   0        0        0       26 2023-07-11 13:34:58.000000 aliste-0.1.5/aliste/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-07-11 15:18:28.000000 aliste-0.1.5/aliste/broker.py
+-rw-rw-rw-   0        0        0      344 2023-07-11 13:12:35.000000 aliste-0.1.5/aliste/constants.py
+-rw-rw-rw-   0        0        0     1948 2023-07-11 14:41:53.000000 aliste-0.1.5/aliste/device.py
+-rw-rw-rw-   0        0        0      145 2023-07-11 11:16:10.000000 aliste-0.1.5/aliste/enums.py
+-rw-rw-rw-   0        0        0      346 2023-07-11 13:20:17.000000 aliste-0.1.5/aliste/home.py
+-rw-rw-rw-   0        0        0     2628 2023-07-11 15:18:00.000000 aliste-0.1.5/aliste/hub.py
+-rw-rw-rw-   0        0        0      353 2023-07-11 11:01:22.000000 aliste-0.1.5/aliste/user.py
+-rw-rw-rw-   0        0        0      230 2023-07-11 15:34:53.000000 aliste-0.1.5/aliste/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:35:00.206903 aliste-0.1.5/aliste.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-07-11 15:35:00.000000 aliste-0.1.5/aliste.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-11 15:35:00.000000 aliste-0.1.5/aliste.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:35:00.000000 aliste-0.1.5/aliste.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 15:35:00.000000 aliste-0.1.5/aliste.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 15:35:00.209496 aliste-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-07-11 15:34:57.000000 aliste-0.1.5/setup.py
```

### Comparing `aliste-0.1.4/LICENSE` & `aliste-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliste-0.1.4/PKG-INFO` & `aliste-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliste
-Version: 0.1.4
+Version: 0.1.5
 Summary: Aliste Smart Home SDK for Python
 Home-page: https://github.com/Kir4Kun/aliste-smart-home-sdk
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aliste-0.1.4/aliste/broker.py` & `aliste-0.1.5/aliste/broker.py`

 * *Files identical despite different names*

### Comparing `aliste-0.1.4/aliste/device.py` & `aliste-0.1.5/aliste/device.py`

 * *Files identical despite different names*

### Comparing `aliste-0.1.4/aliste/hub.py` & `aliste-0.1.5/aliste/hub.py`

 * *Files identical despite different names*

### Comparing `aliste-0.1.4/aliste.egg-info/PKG-INFO` & `aliste-0.1.5/aliste.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliste
-Version: 0.1.4
+Version: 0.1.5
 Summary: Aliste Smart Home SDK for Python
 Home-page: https://github.com/Kir4Kun/aliste-smart-home-sdk
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aliste-0.1.4/setup.py` & `aliste-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="aliste",
-    version="0.1.4",
+    version="0.1.5",
     description="Aliste Smart Home SDK for Python",
     long_description="Aliste Smart Home SDK for Python",
     long_description_content_type="text/markdown",
     url="https://github.com/Kir4Kun/aliste-smart-home-sdk",
     author="Kir4Kun",
     author_email="rkbl4ze@gmail.com",
     license="MIT",
```

