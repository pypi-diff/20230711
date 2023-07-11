# Comparing `tmp/Req_http_vpn-3.0.0.tar.gz` & `tmp/Req_http_vpn-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Req_http_vpn-3.0.0.tar", last modified: Tue Jul 11 08:34:35 2023, max compression
+gzip compressed data, was "Req_http_vpn-3.5.0.tar", last modified: Tue Jul 11 11:20:21 2023, max compression
```

## Comparing `Req_http_vpn-3.0.0.tar` & `Req_http_vpn-3.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.730234 Req_http_vpn-3.0.0/
--rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     2021 2023-07-11 08:34:35.731234 Req_http_vpn-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-07-10 19:39:51.000000 Req_http_vpn-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.602206 Req_http_vpn-3.0.0/Req_http_vpn/
--rw-rw-rw-   0        0        0     6129 2023-07-11 08:17:58.000000 Req_http_vpn-3.0.0/Req_http_vpn/Req_class.py
--rw-rw-rw-   0        0        0      995 2023-07-11 08:18:04.000000 Req_http_vpn-3.0.0/Req_http_vpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.717236 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       81 2023-07-11 08:34:35.787248 Req_http_vpn-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-07-11 08:34:23.000000 Req_http_vpn-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.826705 Req_http_vpn-3.5.0/
+-rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-3.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2076 2023-07-11 11:20:20.828705 Req_http_vpn-3.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2023-07-10 19:39:51.000000 Req_http_vpn-3.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.443610 Req_http_vpn-3.5.0/Req_http_vpn/
+-rw-rw-rw-   0        0        0     6129 2023-07-11 11:12:45.000000 Req_http_vpn-3.5.0/Req_http_vpn/Req_class.py
+-rw-rw-rw-   0        0        0      995 2023-07-11 08:18:04.000000 Req_http_vpn-3.5.0/Req_http_vpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.820703 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/
+-rw-rw-rw-   0        0        0     2076 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-11 11:20:20.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-07-11 11:20:20.944733 Req_http_vpn-3.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-07-11 11:12:32.000000 Req_http_vpn-3.5.0/setup.py
```

### Comparing `Req_http_vpn-3.0.0/LICENSE` & `Req_http_vpn-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-3.0.0/PKG-INFO` & `Req_http_vpn-3.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Req_http_vpn
-Version: 3.0.0
+Version: 3.5.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
-Keywords: http
+Keywords: http,req_http_vpn,vpn,https,request,requests,data,been,host
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  ____                       _      _    _
 |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
 | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
 |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
```

### Comparing `Req_http_vpn-3.0.0/README.md` & `Req_http_vpn-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-3.0.0/Req_http_vpn/Req_class.py` & `Req_http_vpn-3.5.0/Req_http_vpn/Req_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Req_Vpn_print = '0'
 
 from typing import overload
 from requests import post, head
 import os
 from ColorTER import *
 
-__version__ = ['3.0.0']
+__version__ = ['3.5.0']
 
 class Requests_filter:
     """
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
     ### How to create an object from this class:
     ```python
@@ -120,15 +120,15 @@
                 'UrlBox': f'{self.url}',
                 'ContentTypeBox': f'{Content_type}',
                 'ContentDataBox': f'{Data}',
                 'HeadersBox': f'{Headers}',
                 'RefererBox': f'{Referer}',
                 'AgentList': f'{UserAgent}',
                 'VersionsList': 'HTTP/1.1',
-                'MethodList': 'PorT',
+                'MethodList': 'POST',
             }
             data = post('https://www.httpdebugger.com/Tools/ViewHttpHeaders.aspx', data=datas, timeout=Timeout, stream=Stream)
             return dict(
                 headers= data.headers,
                 content= data.content.decode('utf-8'),
                 status_code= data.status_code
             )
@@ -149,15 +149,15 @@
                 'UrlBox': f'{self.url}',
                 'ContentTypeBox': f'{Content_type}',
                 'ContentDataBox': f'{Data}',
                 'HeadersBox': f'{Headers}',
                 'RefererBox': f'{Referer}',
                 'AgentList': f'{UserAgent}',
                 'VersionsList': 'HTTP/1.1',
-                'MethodList': 'PorT',
+                'MethodList': 'HEAD',
             }
             data = head('https://www.httpdebugger.com/Tools/ViewHttpHeaders.aspx', timeout=Timeout, data=datas)
             return dict(
                 headers= data.headers,
                 content= data.content.decode('utf-8'),
                 status_code= data.status_code
             )
```

### Comparing `Req_http_vpn-3.0.0/Req_http_vpn/__init__.py` & `Req_http_vpn-3.5.0/Req_http_vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-3.0.0/Req_http_vpn.egg-info/PKG-INFO` & `Req_http_vpn-3.5.0/Req_http_vpn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Req-http-vpn
-Version: 3.0.0
+Version: 3.5.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
-Keywords: http
+Keywords: http,req_http_vpn,vpn,https,request,requests,data,been,host
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  ____                       _      _    _
 |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
 | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
 |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
```

