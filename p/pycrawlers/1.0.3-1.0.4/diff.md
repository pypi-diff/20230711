# Comparing `tmp/pycrawlers-1.0.3.tar.gz` & `tmp/pycrawlers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-1.0.3.tar", last modified: Thu Jul  6 03:26:42 2023, max compression
+gzip compressed data, was "pycrawlers-1.0.4.tar", last modified: Tue Jul 11 09:00:33 2023, max compression
```

## Comparing `pycrawlers-1.0.3.tar` & `pycrawlers-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.496952 pycrawlers-1.0.3/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.3/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 03:26:42.496826 pycrawlers-1.0.3/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     2556 2023-07-05 06:09:58.000000 pycrawlers-1.0.3/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.493244 pycrawlers-1.0.3/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.3/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.3/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.493432 pycrawlers-1.0.3/pycrawlers/
--rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.3/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.494521 pycrawlers-1.0.3/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.3/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.3/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     5433 2023-07-06 02:49:38.000000 pycrawlers-1.0.3/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.494940 pycrawlers-1.0.3/pycrawlers/huggingfaces/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.3/pycrawlers/huggingfaces/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     5132 2023-07-06 02:16:23.000000 pycrawlers-1.0.3/pycrawlers/huggingfaces/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.496374 pycrawlers-1.0.3/pycrawlers/websites/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.3/pycrawlers/websites/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.3/pycrawlers/websites/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.3/pycrawlers/websites/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.3/pycrawlers/websites/get_websites.py
--rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.3/pycrawlers/websites/url_filters.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 03:26:42.494037 pycrawlers-1.0.3/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 03:26:42.000000 pycrawlers-1.0.3/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-06 03:26:42.000000 pycrawlers-1.0.3/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-06 03:26:42.000000 pycrawlers-1.0.3/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-06 03:26:42.000000 pycrawlers-1.0.3/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-06 03:26:42.000000 pycrawlers-1.0.3/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-06 03:26:42.497002 pycrawlers-1.0.3/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-06 02:49:38.000000 pycrawlers-1.0.3/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.931628 pycrawlers-1.0.4/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.4/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-11 09:00:33.931505 pycrawlers-1.0.4/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2556 2023-07-05 06:09:58.000000 pycrawlers-1.0.4/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.928296 pycrawlers-1.0.4/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.4/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.4/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.928497 pycrawlers-1.0.4/pycrawlers/
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.4/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.929569 pycrawlers-1.0.4/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.4/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.4/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     5528 2023-07-11 08:39:06.000000 pycrawlers-1.0.4/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.929963 pycrawlers-1.0.4/pycrawlers/huggingfaces/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.4/pycrawlers/huggingfaces/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     5481 2023-07-11 08:43:52.000000 pycrawlers-1.0.4/pycrawlers/huggingfaces/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.931062 pycrawlers-1.0.4/pycrawlers/websites/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.4/pycrawlers/websites/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.4/pycrawlers/websites/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.4/pycrawlers/websites/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.4/pycrawlers/websites/get_websites.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.4/pycrawlers/websites/url_filters.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-11 09:00:33.929067 pycrawlers-1.0.4/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-11 09:00:33.000000 pycrawlers-1.0.4/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-11 09:00:33.000000 pycrawlers-1.0.4/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-11 09:00:33.000000 pycrawlers-1.0.4/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-11 09:00:33.000000 pycrawlers-1.0.4/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-11 09:00:33.000000 pycrawlers-1.0.4/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-11 09:00:33.931665 pycrawlers-1.0.4/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-11 09:00:10.000000 pycrawlers-1.0.4/setup.py
```

### Comparing `pycrawlers-1.0.3/LICENSE` & `pycrawlers-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/PKG-INFO` & `pycrawlers-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-1.0.3/README.md` & `pycrawlers-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/other/dw_hg.py` & `pycrawlers-1.0.4/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers/common/default_data.py` & `pycrawlers-1.0.4/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers/common/tools.py` & `pycrawlers-1.0.4/pycrawlers/common/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 import random
 from pymongo import MongoClient
 from pytz import timezone
 import json
 from pycrawlers.common.default_data import default_headers
 
 
-def get_session():
-    """使用requests Session，使抓取数据的时候可以重试"""
+def get_session(max_retries: int = 3):
+    """
+    使用requests Session，使抓取数据的时候可以重试
+    # 默认设置重试次数为3次
+    """
     session = requests.Session()
-    session.mount('http://', HTTPAdapter(max_retries=3))  # 设置重试次数为3次
-    session.mount('https://', HTTPAdapter(max_retries=3))
+    session.mount('http://', HTTPAdapter(max_retries=max_retries))
+    session.mount('https://', HTTPAdapter(max_retries=max_retries))
     return session
 
 
-requests_session = get_session()
-
-
 class DealException(object):
     """处理异常返回的装饰器"""
     def __call__(self, func):
         @wraps(func)
         def wrapped_function(*args, **kwargs):
             try:
                 response = func(*args, **kwargs)
@@ -37,18 +37,20 @@
                 return response
             except requests.RequestException as e:
                 print(e)
         return wrapped_function
 
 
 # 下载数据
-def download(url: str, fname: str, headers: dict, read_timeout: int = 15, file_size=None):
+def download(url: str, fname: str, headers: dict, read_timeout: int = 15, file_size=None, max_retries: int = 3):
     if 'Range' in headers:
         del headers['Range']
 
+    requests_session = get_session(max_retries)
+
     @DealException()
     def get_data():
         return requests_session.get(url, headers=headers, stream=True, timeout=(read_timeout, 5))
     resp_ = get_data()
     total_ = int(resp_.headers.get('content-length', 0))
     if file_size < total_:
         file_op = 'wb'
```

### Comparing `pycrawlers-1.0.3/pycrawlers/huggingfaces/download.py` & `pycrawlers-1.0.4/pycrawlers/huggingfaces/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 获取hugging face 模型
 """
 import random
 import os
 import time
 from lxml import etree
 from pycrawlers.common.default_data import headers
-from pycrawlers.common.tools import requests_session
+from pycrawlers.common.tools import get_session
 from pycrawlers.common.tools import DealException
 from pycrawlers.common.tools import download
 from pycrawlers.common.tools import juedge_path
 from pycrawlers.common.tools import juedge_url
 
 
 class HuggingFace(object):
     def __init__(self, base_url: str = None):
         self.base_url = base_url if base_url else 'https://huggingface.co'
         self.tag = True if base_url else False
         self.html_data = None
+        self.requests_session = get_session()
 
-    def get_data(self, url: str, file_save_path: str = None):
+    def get_data(self, url: str, file_save_path: str = None, max_retries: int = 3):
         """
         获取单个数据
         :param url: 例：'htt://huggingface.co/albert-base-v2/tree/main'
         :param file_save_path: None or './albert-base-v2'
+        :param max_retries: request 最大重试次数
         :return:
         """
         juedge_url(url)
         _url = url.split('/')
         if not self.tag:
             self.get_base_url(_url)
         response = self.crawl_html(url)
@@ -40,45 +42,46 @@
             # print(self.html_data)
             file_names = self.get_file_names()
             file_urls = self.get_file_urls()
             # print(file_urls)
             # print(file_names)
             files_path = juedge_path(file_save_path) if file_save_path else juedge_path('./' + _url[-3] + '/')
             print(f"{'🔴' * 10}{' ' * 5}Start downloading: {_url[-3]}{' ' * 5}{'🔴' * 10}")
-            self.get_files(file_names, file_urls, files_path)
+            self.get_files(file_names, file_urls, files_path, max_retries)
             print(f"{'🟢' * 10}{' ' * 5}Download completed{' ' * 5}{'🟢' * 10}")
 
-    def get_batch_data(self, urls: list, file_save_paths: list = None, count_info=True):
+    def get_batch_data(self, urls: list, file_save_paths: list = None, count_info=True, max_retries: int = 3):
         """
         批量获取数据
         :param urls: ['https://huggingface.co/albert-base-v2/tree/main',
                       'https://huggingface.co/dmis-lab/biosyn-sapbert-bc5cdr-disease/tree/main']
         :param file_save_paths:['./model_1/albert-base-v2', './model_2/']
         :param count_info: 是否生成程序执行的统计信息
+        :param max_retries: request 最大重试次数
         :return:
         """
         success_urls = []
         fail_urls = []
         if file_save_paths:
             if len(urls) == len(file_save_paths):
                 for u, f in zip(urls, file_save_paths):
-                    success_urls, fail_urls = self.fault_tolerant(u, success_urls, fail_urls, f)
+                    success_urls, fail_urls = self.fault_tolerant(u, success_urls, fail_urls, f, max_retries)
             else:
                 raise ValueError('The number of urls and paths is inconsistent')
         else:
             for url in urls:
-                success_urls, fail_urls = self.fault_tolerant(url, success_urls, fail_urls)
+                success_urls, fail_urls = self.fault_tolerant(url, success_urls, fail_urls, max_retries=max_retries)
         if count_info:
             if success_urls or fail_urls:
                 self.count_info(success_urls, fail_urls)
 
-    def fault_tolerant(self, url: str, success_urls: list, fail_urls: list, path: str = None):
+    def fault_tolerant(self, url: str, success_urls: list, fail_urls: list, path: str = None, max_retries: int = 3):
         """容错处理"""
         try:
-            self.get_data(url, path)
+            self.get_data(url, path, max_retries)
             success_urls.append(url)
             time.sleep(0.5)
         except Exception as e:
             print(e)
             fail_urls.append(url)
         return success_urls, fail_urls
 
@@ -87,15 +90,15 @@
         if len(_url) > 5:
             if 'http' in _url[0] and _url[1] == '':
                 self.base_url = _url[0] + '//' + _url[2]
 
     @DealException()
     def crawl_html(self, url):
         """获取html"""
-        return requests_session.get(url, headers=headers, timeout=1)
+        return self.requests_session.get(url, headers=headers, timeout=1)
 
     def get_file_names(self):
         """获取文件名"""
         xpath = f'//div[@data-target="ViewerIndexTreeList"]/ul/li//a[1]/span[1]/text()'
         return self.html_data.xpath(xpath)
 
     def get_file_urls(self):
@@ -104,20 +107,21 @@
         return self.html_data.xpath(xpath)
 
     @staticmethod
     def generate_file_path(_url: list):
         """生成路径"""
         return juedge_path('./' + _url[-3] + '/')
 
-    def get_files(self, file_names, file_urls, files_path):
+    def get_files(self, file_names, file_urls, files_path, max_retries):
         for name, part_url in zip(file_names, file_urls):
             if name in part_url:
                 url = self.base_url + part_url
                 save_file_path = files_path + name
-                download(url, save_file_path, headers, read_timeout=60, file_size=self.get_file_size(save_file_path))
+                download(url, save_file_path, headers,
+                         read_timeout=60, file_size=self.get_file_size(save_file_path), max_retries=max_retries)
                 time.sleep(random.random())
 
     @staticmethod
     def count_info(success_urls, fail_urls):
         print(f'程序执行统计：')
         print(f'a. 成功{str(len(success_urls))}个')
         print(f'b. 失败{str(len(fail_urls))}个')
```

### Comparing `pycrawlers-1.0.3/pycrawlers/websites/get_web_page.py` & `pycrawlers-1.0.4/pycrawlers/websites/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers/websites/get_web_page_id.py` & `pycrawlers-1.0.4/pycrawlers/websites/get_web_page_id.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers/websites/get_websites.py` & `pycrawlers-1.0.4/pycrawlers/websites/get_websites.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers/websites/url_filters.py` & `pycrawlers-1.0.4/pycrawlers/websites/url_filters.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-1.0.4/pycrawlers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-1.0.3/pycrawlers.egg-info/SOURCES.txt` & `pycrawlers-1.0.4/pycrawlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.3/setup.py` & `pycrawlers-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='1.0.3',
+    version='1.0.4',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

