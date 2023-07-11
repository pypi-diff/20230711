# Comparing `tmp/Req_http_vpn-2.0.0.tar.gz` & `tmp/Req_http_vpn-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Req_http_vpn-2.0.0.tar", last modified: Mon Jul 10 21:29:02 2023, max compression
+gzip compressed data, was "Req_http_vpn-3.0.0.tar", last modified: Tue Jul 11 08:34:35 2023, max compression
```

## Comparing `Req_http_vpn-2.0.0.tar` & `Req_http_vpn-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.498884 Req_http_vpn-2.0.0/
--rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2297 2023-07-10 21:29:02.500913 Req_http_vpn-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-07-10 21:14:54.000000 Req_http_vpn-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.323853 Req_http_vpn-2.0.0/Req_http_vpn/
--rw-rw-rw-   0        0        0     7101 2023-07-10 21:11:58.000000 Req_http_vpn-2.0.0/Req_http_vpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.493878 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/
--rw-rw-rw-   0        0        0     2297 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-10 21:29:02.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       81 2023-07-10 21:29:02.556895 Req_http_vpn-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-07-10 21:27:34.000000 Req_http_vpn-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.730234 Req_http_vpn-3.0.0/
+-rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2021 2023-07-11 08:34:35.731234 Req_http_vpn-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2023-07-10 19:39:51.000000 Req_http_vpn-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.602206 Req_http_vpn-3.0.0/Req_http_vpn/
+-rw-rw-rw-   0        0        0     6129 2023-07-11 08:17:58.000000 Req_http_vpn-3.0.0/Req_http_vpn/Req_class.py
+-rw-rw-rw-   0        0        0      995 2023-07-11 08:18:04.000000 Req_http_vpn-3.0.0/Req_http_vpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:35.717236 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/
+-rw-rw-rw-   0        0        0     2021 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 08:34:35.000000 Req_http_vpn-3.0.0/Req_http_vpn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-07-11 08:34:35.787248 Req_http_vpn-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-07-11 08:34:23.000000 Req_http_vpn-3.0.0/setup.py
```

### Comparing `Req_http_vpn-2.0.0/LICENSE` & `Req_http_vpn-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-2.0.0/PKG-INFO` & `Req_http_vpn-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: Req_http_vpn
-Version: 2.0.0
+Version: 3.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ____                       _      _    _
-# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-#                  |_||_____|                 |_|    |_____|       |_|
+ ____                       _      _    _
+|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+                 |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -42,26 +42,12 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
-
-    ```python
-   from Req_http_vpn import *
-   import os
-
-   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
-
-   app = Requests_filter(Url=f'https://youtube.com')
-
-   app = app.filter_req_GET()
-
-   print(app.get('content'))
-    ```
-
     `The author and developer of this light and simple library:` ÙŽ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

### Comparing `Req_http_vpn-2.0.0/README.md` & `Req_http_vpn-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# ____                       _      _    _
-# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-#                  |_||_____|                 |_|    |_____|       |_|
+ ____                       _      _    _
+|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+                 |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -30,26 +30,12 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
-
-    ```python
-   from Req_http_vpn import *
-   import os
-
-   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
-
-   app = Requests_filter(Url=f'https://youtube.com')
-
-   app = app.filter_req_GET()
-
-   print(app.get('content'))
-    ```
-
     `The author and developer of this light and simple library:` َ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

### Comparing `Req_http_vpn-2.0.0/Req_http_vpn.egg-info/PKG-INFO` & `Req_http_vpn-3.0.0/Req_http_vpn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: Req-http-vpn
-Version: 2.0.0
+Version: 3.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ____                       _      _    _
-# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-#                  |_||_____|                 |_|    |_____|       |_|
+ ____                       _      _    _
+|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+                 |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -42,26 +42,12 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
-
-    ```python
-   from Req_http_vpn import *
-   import os
-
-   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
-
-   app = Requests_filter(Url=f'https://youtube.com')
-
-   app = app.filter_req_GET()
-
-   print(app.get('content'))
-    ```
-
     `The author and developer of this light and simple library:` ÙŽ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

### Comparing `Req_http_vpn-2.0.0/setup.py` & `Req_http_vpn-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-import setuptools, os, sys, re
+
+import setuptools, os
 
 with open('README.md', "r") as f:
     long_description = f.read()
     
-print('Thank you for installing and using our library (:')
+print('Thank you for installing version 3 of this library ❤')
     
 def find_packages(path='.'):
     ret = []
     for root, dirs, files in os.walk(path):
         if '__init__.py' in files:
             package_name = root.replace('/', '.').lstrip('.\\')
             ret.append(package_name)
     return ret
 
 setuptools.setup(
     name=f"Req_http_vpn",
-    version=f"2.0.0",
+    version=f"3.0.0",
     author=f"Amin Rngbr",
     author_email=f"rngbramin@gmail.com",
     description=f"A simple and optimized library for sending HTTP requests to closed or filtered sites (:",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='LICENSE',
     url=f"https://github.com/aminrngbr1122",
     keywords=f"http",
     packages=find_packages(),
-    install_requires=['colorter', 'requests',  'MusicBGX'],
+    install_requires=['colorter', 'requests'],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

