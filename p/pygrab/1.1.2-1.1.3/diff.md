# Comparing `tmp/pygrab-1.1.2.tar.gz` & `tmp/pygrab-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.1.2.tar", last modified: Sun Jul  9 21:00:17 2023, max compression
+gzip compressed data, was "pygrab-1.1.3.tar", last modified: Tue Jul 11 01:45:42 2023, max compression
```

## Comparing `pygrab-1.1.2.tar` & `pygrab-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.717000 pygrab-1.1.2/
--rw-rw-rw-   0        0        0      183 2023-07-09 21:00:17.709000 pygrab-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.652000 pygrab-1.1.2/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.2/pygrab/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.2/pygrab/proxylist.py
--rw-rw-rw-   0        0        0    15789 2023-07-09 20:58:03.000000 pygrab-1.1.2/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.701000 pygrab-1.1.2/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 21:00:17.715000 pygrab-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-09 20:58:15.000000 pygrab-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.476000 pygrab-1.1.3/
+-rw-rw-rw-   0        0        0      183 2023-07-11 01:45:42.468000 pygrab-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.405000 pygrab-1.1.3/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.3/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.3/pygrab/proxylist.py
+-rw-rw-rw-   0        0        0    16578 2023-07-11 01:42:55.000000 pygrab-1.1.3/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.461000 pygrab-1.1.3/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:45:42.474000 pygrab-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-11 01:43:23.000000 pygrab-1.1.3/setup.py
```

### Comparing `pygrab-1.1.2/pygrab/proxylist.py` & `pygrab-1.1.3/pygrab/proxylist.py`

 * *Files identical despite different names*

### Comparing `pygrab-1.1.2/pygrab/pygrab.py` & `pygrab-1.1.3/pygrab/pygrab.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .proxylist import ProxyList
 import requests as _requests
 from pyppeteer import launch as _launch
 import asyncio as _asyncio
 import time as _time
 
 
-
 def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs): 
     """
     Gets the content at the specified URL.
 
     Parameters:
         url (str): The URL to get.
         use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
@@ -85,59 +84,66 @@
                     return session.get(url, *args, **kwargs, proxies=proxies)
                 except Exception as err:
                     raise Exception(f'{err}\n\nThere seems to have been an error with the proxy IP. Please note that free proxies may not be reliable.')
 
             return session.get(url, *args, **kwargs)
     raise Exception(f"Invalid url: {url}")
     
-def get_async(urls, use_proxy=False, retries=5, enable_js=False, time_rest=0, *args, **kwargs) -> list:
+def get_async(urls, use_proxy=False, retries=5, enable_js=False, thread_limit=800, time_rest=0, *args, **kwargs) -> list:
     """
     Gets multiple URLs asynchronously.
 
     This function sends HTTP requests to a list of URLs in separate threads, allowing for concurrent HTTP requests.
     The function returns a list of responses from the grabbed URLs.
 
     Args:
         urls (list): A list of URLs to grab.
         use_proxy (bool, optional): If True, uses a proxy for the HTTP requests. Defaults to False.
         retries (int, optional): The number of times to retry the HTTP request in case of failure. Defaults to 5.
+        thread_limit (int, optional): The maximum number of threads that will be spawned. 
         time_rest (int, optional): The time in seconds to wait between starting each thread. Defaults to 0.
         *args: Variable length argument list to pass to the get function.
         **kwargs: Arbitrary keyword arguments to pass to the get function.
 
     Returns:
         list: A list of responses from the grabbed URLs.
     
     Raises:
         TypeError: If any of the arguments are not of the desired data type.
     """
-    if not (isinstance(urls, list)):
-        raise TypeError("Argument 'urls' must be a list")
+    if (isinstance(urls, (str, int, float, bool))):
+        raise TypeError("Argument 'urls' must be an iterable object")
     elif not (isinstance(use_proxy, bool)):
         raise TypeError("Argument 'use_proxy' must be a bool")
     elif not (isinstance(retries, int)):
         raise TypeError("Argument 'retries' must be a int")
     elif not (isinstance(enable_js, bool)):
         raise TypeError("Argument 'enable_js' must be a bool")
     elif not (isinstance(time_rest, int) or isinstance(time_rest, float)):
         raise TypeError("Argument 'time_rest' must be a int or float")
 
     import threading as _threading # only import if async functionality is needed
     if type(urls) == str:
         return [get(urls, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)]
 
+
     result = []
-    threads = []
-    for url in urls:
-        threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
-        threads[-1].start()
-        _time.sleep(time_rest)
-    
-    for thread in threads:
-        thread.join()
+    thread_counter = 0
+
+    while thread_counter < len(urls):
+        sub_urls = urls[thread_counter:thread_counter+thread_limit]
+        threads = []
+        for url in sub_urls:
+            threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
+            threads[-1].start()
+            _time.sleep(time_rest)
+        
+        for thread in threads:
+            thread.join()
+        thread_counter += thread_limit
         
     return result
 
 def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8'):
     """
     Reads the contens of a file and returns it to the user.
 
@@ -213,39 +219,40 @@
 
     if response.status_code == 200:
         with open(local_filename, 'wb') as f:
             f.write(response.content)
     else:
         raise Exception(f"Error fetching url. Status code - {response.status_code}")
 
-def download_async(urls:list, local_filename:list=None, use_proxy=False, retries=5, time_rest=0) -> None:
+def download_async(urls:list, local_filename:list=None, use_proxy=False, retries=5, thread_limit=500, time_rest=0) -> None:
     """
     Executes multiple file downloads asynchronously from a list of given URLs and saves them locally.
 
     This function uses threading to download multiple files simultaneously. Each file is saved with a filename from the list of local filenames, if provided. If no local filename is provided, the function uses the filename from the corresponding URL.
 
     Parameters:
         urls (list of str): The URLs of the files to be downloaded. Each URL must include a file extension.
         local_filename (list of str, optional): A list of names to be used when saving the files locally. If none is provided, the function uses the filename from each corresponding URL. Each filename must include a file extension if provided. Must be of same length as 'urls' if provided.
         use_proxy (bool, optional): If set to True, the function will use a proxy server for the downloads. Defaults to False.
         retries (int, optional): The number of retry attempts for the downloads in case of failure. Defaults to 5.
+        thread_limit (int, optional): The maximum number of threads that will be spawned. 
         time_rest (int, optional): The amount of time to rest between the start of each download thread. Defaults to 0 seconds.
 
     Returns:
         None
 
     Raises:
         TypeError: If any of the arguments are not of the desired data type.
         ValueError: If 'local_filename' is specified but does not match the length of 'urls' or if a URL does not contain a file extension.
         ValueError: If a 'local_filename' is specified but does not contain a file extension.
     """
-    if not (isinstance(urls, list)):
-        raise TypeError("Argument 'urls' must be a list")
-    elif not (isinstance(local_filename, list) or local_filename is None):
-        raise TypeError("Argument 'local_filename' must be a list")
+    if (isinstance(urls, (str, int, float, bool))):
+        raise TypeError("Argument 'urls' must be an iterable object")
+    elif (isinstance(local_filename, (str, int, float, bool)) or local_filename is None):
+        raise TypeError("Argument 'local_filename' must be an iterable object")
     elif not (isinstance(use_proxy, bool)):
         raise TypeError("Argument 'use_proxy' must be a bool")
     elif not (isinstance(retries, int)):
         raise TypeError("Argument 'retries' must be a int")
     elif not (isinstance(time_rest, int) or isinstance(time_rest, float)):
         raise TypeError("Argument 'time_rest' must be a int or float")
 
@@ -254,24 +261,29 @@
         if len(urls) != len(local_filename):
             raise ValueError("Lists 'url' and 'name' must be of equal length.")
     else:
         local_filename = [None for _ in range(len(urls))]
 
     # only import if async functionality is needed
     import threading as _threading
-    import time as _time
 
-    threads = []
-    for url, name in zip(urls, local_filename):
-        threads.append(_threading.Thread(target=download, args=[url, name, use_proxy, retries]))
-        threads[-1].start()
-        _time.sleep(time_rest)
-    
-    for thread in threads:
-        thread.join()
+    thread_counter = 0
+    while (thread_counter < len(urls)):
+        threads = []
+        sub_urls = urls[thread_counter:thread_counter+thread_limit]
+        sub_local_filename= local_filename[thread_counter:thread_counter+thread_limit]
+
+        for url, name in zip(sub_urls, sub_local_filename):
+            threads.append(_threading.Thread(target=download, args=[url, name, use_proxy, retries]))
+            threads[-1].start()
+            _time.sleep(time_rest)
+        
+        for thread in threads:
+            thread.join()
+        thread_counter += thread_limit
     
 
 def head(url, **kwargs):
     return _requests.head(url, **kwargs)
 
 def post(url:str, data=None, json=None, **kwargs):
     local_file_starts = ['./', 'C:', '/']
```

