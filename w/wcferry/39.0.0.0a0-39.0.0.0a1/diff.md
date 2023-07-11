# Comparing `tmp/wcferry-39.0.0.0a0.tar.gz` & `tmp/wcferry-39.0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcferry-39.0.0.0a0.tar", last modified: Tue Jul 11 08:38:47 2023, max compression
+gzip compressed data, was "wcferry-39.0.0.0a1.tar", last modified: Tue Jul 11 08:45:04 2023, max compression
```

## Comparing `wcferry-39.0.0.0a0.tar` & `wcferry-39.0.0.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:38:47.687813 wcferry-39.0.0.0a0/
--rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-39.0.0.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     5676 2023-07-11 08:38:47.686807 wcferry-39.0.0.0a0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-11 08:38:47.687813 wcferry-39.0.0.0a0/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-39.0.0.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:38:47.674801 wcferry-39.0.0.0a0/wcferry/
--rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-39.0.0.0a0/wcferry/__init__.py
--rw-rw-rw-   0        0        0    19873 2023-07-11 08:25:24.000000 wcferry-39.0.0.0a0/wcferry/client.py
--rw-rw-rw-   0        0        0   634880 2023-07-01 22:32:25.000000 wcferry-39.0.0.0a0/wcferry/spy.dll
--rw-rw-rw-   0        0        0  1163776 2023-07-01 22:35:24.000000 wcferry-39.0.0.0a0/wcferry/spy_debug.dll
--rwxrwxrwx   0        0        0   162816 2023-07-01 22:32:39.000000 wcferry-39.0.0.0a0/wcferry/wcf.exe
--rw-rw-rw-   0        0        0     7362 2023-07-10 00:15:30.000000 wcferry-39.0.0.0a0/wcferry/wcf_pb2.py
--rw-rw-rw-   0        0        0     2055 2023-05-10 03:43:35.000000 wcferry-39.0.0.0a0/wcferry/wxmsg.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:38:47.683802 wcferry-39.0.0.0a0/wcferry.egg-info/
--rw-rw-rw-   0        0        0     5676 2023-07-11 08:38:47.000000 wcferry-39.0.0.0a0/wcferry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-11 08:38:47.000000 wcferry-39.0.0.0a0/wcferry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:38:47.000000 wcferry-39.0.0.0a0/wcferry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-11 08:38:47.000000 wcferry-39.0.0.0a0/wcferry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 08:38:47.000000 wcferry-39.0.0.0a0/wcferry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 08:45:04.520367 wcferry-39.0.0.0a1/
+-rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-39.0.0.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5678 2023-07-11 08:45:04.519369 wcferry-39.0.0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:45:04.520367 wcferry-39.0.0.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-39.0.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:45:04.507369 wcferry-39.0.0.0a1/wcferry/
+-rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-39.0.0.0a1/wcferry/__init__.py
+-rw-rw-rw-   0        0        0    19873 2023-07-11 08:44:57.000000 wcferry-39.0.0.0a1/wcferry/client.py
+-rw-rw-rw-   0        0        0   634880 2023-07-01 22:32:25.000000 wcferry-39.0.0.0a1/wcferry/spy.dll
+-rw-rw-rw-   0        0        0  1163776 2023-07-01 22:35:24.000000 wcferry-39.0.0.0a1/wcferry/spy_debug.dll
+-rwxrwxrwx   0        0        0   162816 2023-07-01 22:32:39.000000 wcferry-39.0.0.0a1/wcferry/wcf.exe
+-rw-rw-rw-   0        0        0     7362 2023-07-10 00:15:30.000000 wcferry-39.0.0.0a1/wcferry/wcf_pb2.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 03:43:35.000000 wcferry-39.0.0.0a1/wcferry/wxmsg.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:45:04.517365 wcferry-39.0.0.0a1/wcferry.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-07-11 08:45:04.000000 wcferry-39.0.0.0a1/wcferry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-11 08:45:04.000000 wcferry-39.0.0.0a1/wcferry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:45:04.000000 wcferry-39.0.0.0a1/wcferry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-11 08:45:04.000000 wcferry-39.0.0.0a1/wcferry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 08:45:04.000000 wcferry-39.0.0.0a1/wcferry.egg-info/top_level.txt
```

### Comparing `wcferry-39.0.0.0a0/PKG-INFO` & `wcferry-39.0.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 39.0.0.0a0
+Version: 39.0.0.0a1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 
 # WeChatFerry Python 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
 
 |[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/XTJ9H-FsCPCscixAts8i_A)|
 |:-:|:-:|:-:|
+
 🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
 
 ## 快速开始
 ```sh
 pip install --upgrade wcferry
 ```
```

### Comparing `wcferry-39.0.0.0a0/setup.py` & `wcferry-39.0.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry/client.py` & `wcferry-39.0.0.0a1/wcferry/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-__version__ = "39.0.0.0a0"
+__version__ = "39.0.0.0a1"
 
 import atexit
 import base64
 import logging
 import os
 import re
 import sys
```

### Comparing `wcferry-39.0.0.0a0/wcferry/spy.dll` & `wcferry-39.0.0.0a1/wcferry/spy.dll`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry/spy_debug.dll` & `wcferry-39.0.0.0a1/wcferry/spy_debug.dll`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry/wcf.exe` & `wcferry-39.0.0.0a1/wcferry/wcf.exe`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry/wcf_pb2.py` & `wcferry-39.0.0.0a1/wcferry/wcf_pb2.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry/wxmsg.py` & `wcferry-39.0.0.0a1/wcferry/wxmsg.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a0/wcferry.egg-info/PKG-INFO` & `wcferry-39.0.0.0a1/wcferry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 39.0.0.0a0
+Version: 39.0.0.0a1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 
 # WeChatFerry Python 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
 
 |[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/XTJ9H-FsCPCscixAts8i_A)|
 |:-:|:-:|:-:|
+
 🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
 
 ## 快速开始
 ```sh
 pip install --upgrade wcferry
 ```
```

