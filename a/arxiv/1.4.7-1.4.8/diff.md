# Comparing `tmp/arxiv-1.4.7.tar.gz` & `tmp/arxiv-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-1.4.7.tar", last modified: Tue Apr 18 22:04:02 2023, max compression
+gzip compressed data, was "arxiv-1.4.8.tar", last modified: Tue Jul 11 05:42:21 2023, max compression
```

## Comparing `arxiv-1.4.7.tar` & `arxiv-1.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 22:04:02.552391 arxiv-1.4.7/
--rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.7/LICENSE.txt
--rw-r--r--   0 lukas      (501) staff       (20)     8091 2023-04-18 22:04:02.552574 arxiv-1.4.7/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     7314 2023-04-18 21:41:18.000000 arxiv-1.4.7/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 22:04:02.546157 arxiv-1.4.7/arxiv/
--rw-r--r--   0 lukas      (501) staff       (20)       35 2023-04-18 21:25:11.000000 arxiv-1.4.7/arxiv/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)    26587 2023-04-17 00:44:38.000000 arxiv-1.4.7/arxiv/arxiv.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 22:04:02.548812 arxiv-1.4.7/arxiv.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     8091 2023-04-18 22:04:02.000000 arxiv-1.4.7/arxiv.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-18 22:04:02.000000 arxiv-1.4.7/arxiv.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-18 22:04:02.000000 arxiv-1.4.7/arxiv.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-18 22:04:02.000000 arxiv-1.4.7/arxiv.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-18 22:04:02.000000 arxiv-1.4.7/arxiv.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      114 2023-04-18 22:04:02.553420 arxiv-1.4.7/setup.cfg
--rw-r--r--   0 lukas      (501) staff       (20)     1164 2023-04-18 22:01:37.000000 arxiv-1.4.7/setup.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 22:04:02.551859 arxiv-1.4.7/tests/
--rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.7/tests/test_api_bugs.py
--rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.7/tests/test_client.py
--rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.7/tests/test_download.py
--rw-r--r--   0 lukas      (501) staff       (20)     4098 2023-04-18 20:55:02.000000 arxiv-1.4.7/tests/test_result.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-07-11 05:42:21.280277 arxiv-1.4.8/
+-rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.8/LICENSE.txt
+-rw-r--r--   0 lukas      (501) staff       (20)     8091 2023-07-11 05:42:21.280605 arxiv-1.4.8/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     7314 2023-04-19 00:25:45.000000 arxiv-1.4.8/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-07-11 05:42:21.271124 arxiv-1.4.8/arxiv/
+-rw-r--r--   0 lukas      (501) staff       (20)       35 2023-04-18 21:25:11.000000 arxiv-1.4.8/arxiv/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)    26563 2023-07-11 05:39:00.000000 arxiv-1.4.8/arxiv/arxiv.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-07-11 05:42:21.274633 arxiv-1.4.8/arxiv.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     8091 2023-07-11 05:42:21.000000 arxiv-1.4.8/arxiv.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      305 2023-07-11 05:42:21.000000 arxiv-1.4.8/arxiv.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-07-11 05:42:21.000000 arxiv-1.4.8/arxiv.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       11 2023-07-11 05:42:21.000000 arxiv-1.4.8/arxiv.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        6 2023-07-11 05:42:21.000000 arxiv-1.4.8/arxiv.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      114 2023-07-11 05:42:21.282204 arxiv-1.4.8/setup.cfg
+-rw-r--r--   0 lukas      (501) staff       (20)     1164 2023-07-11 05:39:00.000000 arxiv-1.4.8/setup.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-07-11 05:42:21.278917 arxiv-1.4.8/tests/
+-rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.8/tests/test_api_bugs.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.8/tests/test_client.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1626 2023-07-11 05:39:00.000000 arxiv-1.4.8/tests/test_download.py
+-rw-r--r--   0 lukas      (501) staff       (20)     4098 2023-04-18 20:55:02.000000 arxiv-1.4.8/tests/test_result.py
```

### Comparing `arxiv-1.4.7/LICENSE.txt` & `arxiv-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.7/PKG-INFO` & `arxiv-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py
+[![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.7/README.md` & `arxiv-1.4.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py
+[![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.7/arxiv/arxiv.py` & `arxiv-1.4.8/arxiv/arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,19 @@
         return self.entry_id.split('arxiv.org/abs/')[-1]
 
     def _get_default_filename(self, extension: str = "pdf") -> str:
         """
         A default `to_filename` function for the extension given.
         """
         nonempty_title = self.title if self.title else "UNTITLED"
-        # Remove disallowed characters.
-        clean_title = '_'.join(re.findall(r'\w+', nonempty_title))
-        return "{}.{}.{}".format(self.get_short_id(), clean_title, extension)
+        return '.'.join([
+            self.get_short_id().replace("/", "_"),
+            re.sub(r"[^\w]", "_", nonempty_title),
+            extension
+        ])
 
     def download_pdf(self, dirpath: str = './', filename: str = '') -> str:
         """
         Downloads the PDF for this result to the specified directory.
 
         The filename is generated by calling `to_filename(self)`.
         """
```

### Comparing `arxiv-1.4.7/arxiv.egg-info/PKG-INFO` & `arxiv-1.4.8/arxiv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py
+[![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.7/setup.py` & `arxiv-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.4.7'
+version = '1.4.8'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='arxiv',
     version=version,
```

### Comparing `arxiv-1.4.7/tests/test_api_bugs.py` & `arxiv-1.4.8/tests/test_api_bugs.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.7/tests/test_client.py` & `arxiv-1.4.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.7/tests/test_download.py` & `arxiv-1.4.8/tests/test_download.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class TestDownload(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         self.fetched_result = next(arxiv.Search(id_list=["1605.08386"]).results())
+        self.fetched_result_with_slash = next(arxiv.Search(id_list=['hep-ex/0406020v1']).results())
 
     @classmethod
     def setUp(self):
         self.temp_dir = tempfile.mkdtemp()
 
     @classmethod
     def tearDown(self):
@@ -21,14 +22,20 @@
 
     def test_download_from_query(self):
         self.fetched_result.download_pdf(dirpath=self.temp_dir)
         self.assertTrue(os.path.exists(os.path.join(
             self.temp_dir,
             '1605.08386v1.Heat_bath_random_walks_with_Markov_bases.pdf')
         ))
+        # Regression-tests https://github.com/lukasschwab/arxiv.py/issues/117.
+        self.fetched_result_with_slash.download_pdf(dirpath=self.temp_dir)
+        self.assertTrue(os.path.exists(os.path.join(
+            self.temp_dir,
+            'hep-ex_0406020v1.Sparticle_Reconstruction_at_LHC.pdf')
+        ))
 
     def test_download_tarfile_from_query(self):
         self.fetched_result.download_source(dirpath=self.temp_dir)
         self.assertTrue(os.path.exists(os.path.join(
             self.temp_dir,
             '1605.08386v1.Heat_bath_random_walks_with_Markov_bases.tar.gz'
         )))
```

### Comparing `arxiv-1.4.7/tests/test_result.py` & `arxiv-1.4.8/tests/test_result.py`

 * *Files identical despite different names*

