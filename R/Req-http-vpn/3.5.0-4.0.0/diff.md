# Comparing `tmp/Req_http_vpn-3.5.0.tar.gz` & `tmp/Req_http_vpn-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Req_http_vpn-3.5.0.tar", last modified: Tue Jul 11 11:20:21 2023, max compression
+gzip compressed data, was "Req_http_vpn-4.0.0.tar", last modified: Tue Jul 11 12:37:25 2023, max compression
```

## Comparing `Req_http_vpn-3.5.0.tar` & `Req_http_vpn-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.826705 Req_http_vpn-3.5.0/
--rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-3.5.0/LICENSE
--rw-rw-rw-   0        0        0     2076 2023-07-11 11:20:20.828705 Req_http_vpn-3.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-07-10 19:39:51.000000 Req_http_vpn-3.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.443610 Req_http_vpn-3.5.0/Req_http_vpn/
--rw-rw-rw-   0        0        0     6129 2023-07-11 11:12:45.000000 Req_http_vpn-3.5.0/Req_http_vpn/Req_class.py
--rw-rw-rw-   0        0        0      995 2023-07-11 08:18:04.000000 Req_http_vpn-3.5.0/Req_http_vpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:20:20.820703 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/
--rw-rw-rw-   0        0        0     2076 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-11 11:20:20.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 11:20:19.000000 Req_http_vpn-3.5.0/Req_http_vpn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       81 2023-07-11 11:20:20.944733 Req_http_vpn-3.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-07-11 11:12:32.000000 Req_http_vpn-3.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.853776 Req_http_vpn-4.0.0/
+-rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2129 2023-07-11 12:37:25.864777 Req_http_vpn-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2023-07-11 12:36:10.000000 Req_http_vpn-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.719744 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/
+-rw-rw-rw-   0        0        0     2129 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.847776 Req_http_vpn-4.0.0/Req_http_vpng/
+-rw-rw-rw-   0        0        0     6418 2023-07-11 12:35:12.000000 Req_http_vpn-4.0.0/Req_http_vpng/Req_class.py
+-rw-rw-rw-   0        0        0     1093 2023-07-11 12:34:38.000000 Req_http_vpn-4.0.0/Req_http_vpng/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-07-11 12:37:25.954808 Req_http_vpn-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-07-11 12:35:34.000000 Req_http_vpn-4.0.0/setup.py
```

### Comparing `Req_http_vpn-3.5.0/LICENSE` & `Req_http_vpn-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-3.5.0/PKG-INFO` & `Req_http_vpn-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: Req_http_vpn
-Version: 3.5.0
+Version: 4.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
-Keywords: http,req_http_vpn,vpn,https,request,requests,data,been,host
+Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  ____                       _      _    _
 |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
 | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
 |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
 |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
                  |_||_____|                 |_|    |_____|       |_|
-
-"""
+                 
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
 
-   >>> from Req_http_vpn import *
-   >>> app = Requests_filter('Url')
-   >>> data = app.filter_req_GET()[2]
-   >>> print(data.status_code) # Print status_code
+>>>   from Req_http_vpn import *
+>>>   from os import environ
+>>>   environ['print_access_request_library_Req_http_vpn'] = '0'
+>>>   this = Requests_filter('https://instagram.com')
+>>>   this = this.filter_req_GET()
+>>>   print(this.get('status_code'))
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

### Comparing `Req_http_vpn-3.5.0/README.md` & `Req_http_vpn-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
  ____                       _      _    _
 |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
 | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
 |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
 |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
                  |_||_____|                 |_|    |_____|       |_|
-
-"""
+                 
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
 
-   >>> from Req_http_vpn import *
-   >>> app = Requests_filter('Url')
-   >>> data = app.filter_req_GET()[2]
-   >>> print(data.status_code) # Print status_code
+>>>   from Req_http_vpn import *
+>>>   from os import environ
+>>>   environ['print_access_request_library_Req_http_vpn'] = '0'
+>>>   this = Requests_filter('https://instagram.com')
+>>>   this = this.filter_req_GET()
+>>>   print(this.get('status_code'))
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

### Comparing `Req_http_vpn-3.5.0/Req_http_vpn/Req_class.py` & `Req_http_vpn-4.0.0/Req_http_vpng/Req_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Req_Vpn_print = '0'
 
 from typing import overload
 from requests import post, head
 import os
 from ColorTER import *
 
-__version__ = ['3.5.0']
+__version__ = ['4.0.0']
 
 class Requests_filter:
     """
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
     ### How to create an object from this class:
     ```python
@@ -42,38 +42,41 @@
     
     @overload
     def filter_req_GET(
         self,
         Content_type : str = 'text/html',
         Headers : str  = '',
         Timeout : float = 500.5,
+        *,
         Referer : str = 'https://google.com',
         UserAgent : str = 'Google Chrome',
         Stream : bool = False
         ) -> list or dict: ...
     
     @overload
     def filter_req_PorT(
         self,
         Data : str = 'login=...&pass=...',
         Content_type : str = 'text/html',
         Headers : str  = '',
         Timeout : float = 500.5,
+        *,
         Referer : str = 'https://google.com',
         UserAgent : str = 'Google Chrome',
         Stream : bool = False
         ) -> list or dict: ...
     
     @overload
     def filter_req_HEAD(
         self,
         Data : str = 'login=...&pass=...',
         Content_type : str = 'text/html',
         Timeout : float = 500.5,
         Headers : str  = '',
+        *,
         Referer : str = 'https://google.com',
         UserAgent : str = 'Google Chrome',
         ) -> list or dict: ...
 
     # =======================================================================================
 
     def filter_req_GET(
@@ -93,14 +96,15 @@
                 'HeadersBox': f'{Headers}',
                 'RefererBox': f'{Referer}',
                 'AgentList': f'{UserAgent}',
                 'VersionsList': 'HTTP/1.1',
                 'MethodList': 'GET',
             }
             data = post('https://www.httpdebugger.com/Tools/ViewHttpHeaders.aspx', data=datas, timeout=Timeout, stream=Stream)
+            assert data.status_code != 500, "Server error !"
             return dict(
                 headers= data.headers,
                 content= data.content.decode('utf-8'),
                 status_code= data.status_code
             )
         except Exception as e:
             return [e]
@@ -123,14 +127,15 @@
                 'HeadersBox': f'{Headers}',
                 'RefererBox': f'{Referer}',
                 'AgentList': f'{UserAgent}',
                 'VersionsList': 'HTTP/1.1',
                 'MethodList': 'POST',
             }
             data = post('https://www.httpdebugger.com/Tools/ViewHttpHeaders.aspx', data=datas, timeout=Timeout, stream=Stream)
+            assert data.status_code != 500, "Server error !"
             return dict(
                 headers= data.headers,
                 content= data.content.decode('utf-8'),
                 status_code= data.status_code
             )
         except Exception as e:
             return [e]
@@ -152,16 +157,20 @@
                 'HeadersBox': f'{Headers}',
                 'RefererBox': f'{Referer}',
                 'AgentList': f'{UserAgent}',
                 'VersionsList': 'HTTP/1.1',
                 'MethodList': 'HEAD',
             }
             data = head('https://www.httpdebugger.com/Tools/ViewHttpHeaders.aspx', timeout=Timeout, data=datas)
+            assert data.status_code != 500, "Server error !"
             return dict(
                 headers= data.headers,
                 content= data.content.decode('utf-8'),
                 status_code= data.status_code
             )
         except Exception as e:
             return [e]
         
+        def _dateTime() -> str:
+            return 0.0
+        
     # =======================================================================================
```

### Comparing `Req_http_vpn-3.5.0/Req_http_vpn/__init__.py` & `Req_http_vpn-4.0.0/Req_http_vpng/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
 
-   >>> from Req_http_vpn import *
-   >>> app = Requests_filter('Url')
-   >>> data = app.filter_req_GET()[2]
-   >>> print(data.status_code) # Print status_code
+>>>   from Req_http_vpn import *
+>>>   from os import environ
+>>>   environ['print_access_request_library_Req_http_vpn'] = '0'
+>>>   this = Requests_filter('https://instagram.com')
+>>>   this = this.filter_req_GET()
+>>>   print(this.get('status_code'))
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 """
 
 import sys
+
 sys.dont_write_bytecode = True
 
 from .Req_class import Requests_filter, Req_Vpn_print, __version__
 
-this : list = []
+this : dict = {}
```

### Comparing `Req_http_vpn-3.5.0/Req_http_vpn.egg-info/PKG-INFO` & `Req_http_vpn-4.0.0/Req_http_vpn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: Req-http-vpn
-Version: 3.5.0
+Version: 4.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
-Keywords: http,req_http_vpn,vpn,https,request,requests,data,been,host
+Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  ____                       _      _    _
 |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
 | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
 |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
 |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
                  |_||_____|                 |_|    |_____|       |_|
-
-"""
+                 
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
 
-   >>> from Req_http_vpn import *
-   >>> app = Requests_filter('Url')
-   >>> data = app.filter_req_GET()[2]
-   >>> print(data.status_code) # Print status_code
+>>>   from Req_http_vpn import *
+>>>   from os import environ
+>>>   environ['print_access_request_library_Req_http_vpn'] = '0'
+>>>   this = Requests_filter('https://instagram.com')
+>>>   this = this.filter_req_GET()
+>>>   print(this.get('status_code'))
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

