# Comparing `tmp/rongdavbaaddins-0.1.0.4.tar.gz` & `tmp/rongdavbaaddins-0.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.1.0.4.tar", last modified: Mon Jul 10 09:44:55 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.1.0.5.tar", last modified: Tue Jul 11 06:26:35 2023, max compression
```

## Comparing `rongdavbaaddins-0.1.0.4.tar` & `rongdavbaaddins-0.1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:44:55.776013 rongdavbaaddins-0.1.0.4/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      417 2023-07-10 09:44:55.776013 rongdavbaaddins-0.1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 09:44:55.764010 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-07-10 09:44:55.767010 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0  1878442 2023-07-10 09:41:32.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-07-10 09:44:55.769009 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0    59392 2023-07-10 07:42:50.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.pyd
--rw-rw-rw-   0        0        0    54784 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      448 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   144896 2023-07-10 09:42:04.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/rongdavbaaddins.pyd
--rw-rw-rw-   0        0        0    66560 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    29163 2023-07-10 09:41:33.000000 rongdavbaaddins-0.1.0.4/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-07-10 09:44:55.775010 rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      417 2023-07-10 09:44:55.000000 rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-07-10 09:44:55.000000 rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:44:55.000000 rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-10 09:44:55.000000 rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-10 09:44:55.777009 rongdavbaaddins-0.1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-07-10 09:43:31.000000 rongdavbaaddins-0.1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:35.734688 rongdavbaaddins-0.1.0.5/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-07-11 06:26:35.734688 rongdavbaaddins-0.1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:35.689686 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:35.704686 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0  1878442 2023-07-10 09:41:32.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:35.712690 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0    59392 2023-07-10 07:42:50.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.pyd
+-rw-rw-rw-   0        0        0    54784 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      448 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   144896 2023-07-11 06:24:29.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/rongdavbaaddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-07-10 07:25:31.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    29163 2023-07-10 09:41:33.000000 rongdavbaaddins-0.1.0.5/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:35.730687 rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-07-11 06:26:35.000000 rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      781 2023-07-11 06:26:35.000000 rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 06:26:35.000000 rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 06:26:35.000000 rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-11 06:26:35.736692 rongdavbaaddins-0.1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-07-11 06:26:23.000000 rongdavbaaddins-0.1.0.5/setup.py
```

### Comparing `rongdavbaaddins-0.1.0.4/LICENSE.txt` & `rongdavbaaddins-0.1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/rongdaVbaAddins/RDaddins.xlam` & `rongdavbaaddins-0.1.0.5/rongdaVbaAddins/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.1.0.5/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.1.0.5/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.1.0.5/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.1.0.4/setup.py` & `rongdavbaaddins-0.1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.4"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.5"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

