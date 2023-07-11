# Comparing `tmp/pyanalyticsgit-0.1.tar.gz` & `tmp/pyanalyticsgit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.1.tar", last modified: Mon Jul 10 23:52:51 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.2.tar", last modified: Tue Jul 11 00:11:08 2023, max compression
```

## Comparing `pyanalyticsgit-0.1.tar` & `pyanalyticsgit-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 23:52:51.865192 pyanalyticsgit-0.1/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.1/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-10 23:52:51.861192 pyanalyticsgit-0.1/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.1/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 23:52:51.861192 pyanalyticsgit-0.1/analyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 20:01:33.000000 pyanalyticsgit-0.1/analyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3889 2023-07-10 19:25:20.000000 pyanalyticsgit-0.1/analyticsgit/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4362 2023-07-10 20:34:01.000000 pyanalyticsgit-0.1/analyticsgit/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2509 2023-07-10 19:21:15.000000 pyanalyticsgit-0.1/analyticsgit/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4136 2023-07-10 20:34:01.000000 pyanalyticsgit-0.1/analyticsgit/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       82 2023-07-10 17:59:42.000000 pyanalyticsgit-0.1/analyticsgit/main.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3042 2023-07-10 20:34:01.000000 pyanalyticsgit-0.1/analyticsgit/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      267 2023-07-10 20:34:01.000000 pyanalyticsgit-0.1/analyticsgit/monitoramento.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3457 2023-07-10 20:34:01.000000 pyanalyticsgit-0.1/analyticsgit/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1132 2023-07-10 19:56:48.000000 pyanalyticsgit-0.1/analyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1134 2023-07-10 19:56:40.000000 pyanalyticsgit-0.1/analyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      838 2023-07-10 19:09:46.000000 pyanalyticsgit-0.1/analyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 23:52:51.861192 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-10 23:52:51.000000 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      523 2023-07-10 23:52:51.000000 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-10 23:52:51.000000 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-10 23:52:51.000000 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       13 2023-07-10 23:52:51.000000 pyanalyticsgit-0.1/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-10 23:52:51.865192 pyanalyticsgit-0.1/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      721 2023-07-10 23:52:34.000000 pyanalyticsgit-0.1/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.2/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.2/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.766598 pyanalyticsgit-0.2/analyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 20:01:33.000000 pyanalyticsgit-0.2/analyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3889 2023-07-10 19:25:20.000000 pyanalyticsgit-0.2/analyticsgit/automatizar.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4362 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/commit.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2509 2023-07-10 19:21:15.000000 pyanalyticsgit-0.2/analyticsgit/connect.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4136 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/issue.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       82 2023-07-10 17:59:42.000000 pyanalyticsgit-0.2/analyticsgit/main.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3042 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/milestone.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      267 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/monitoramento.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3457 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/relatorio.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1132 2023-07-10 19:56:48.000000 pyanalyticsgit-0.2/analyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1134 2023-07-10 19:56:40.000000 pyanalyticsgit-0.2/analyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      838 2023-07-10 19:09:46.000000 pyanalyticsgit-0.2/analyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.766598 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      523 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        9 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       13 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      538 2023-07-11 00:10:59.000000 pyanalyticsgit-0.2/setup.py
```

### Comparing `pyanalyticsgit-0.1/LICENSE` & `pyanalyticsgit-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/PKG-INFO` & `pyanalyticsgit-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.1
+Version: 0.2
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: Py Analytics Git
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.1/README.md` & `pyanalyticsgit-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/automatizar.py` & `pyanalyticsgit-0.2/analyticsgit/automatizar.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/commit.py` & `pyanalyticsgit-0.2/analyticsgit/commit.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/connect.py` & `pyanalyticsgit-0.2/analyticsgit/connect.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/issue.py` & `pyanalyticsgit-0.2/analyticsgit/issue.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/milestone.py` & `pyanalyticsgit-0.2/analyticsgit/milestone.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/relatorio.py` & `pyanalyticsgit-0.2/analyticsgit/relatorio.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/test_linux.py` & `pyanalyticsgit-0.2/analyticsgit/test_linux.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/test_macos.py` & `pyanalyticsgit-0.2/analyticsgit/test_macos.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/analyticsgit/test_windows.py` & `pyanalyticsgit-0.2/analyticsgit/test_windows.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.2/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.1
+Version: 0.2
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: Py Analytics Git
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.1/pyanalyticsgit.egg-info/SOURCES.txt` & `pyanalyticsgit-0.2/pyanalyticsgit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.1/setup.py` & `pyanalyticsgit-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from setuptools import setup
 from setuptools.dist import Distribution
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='pyanalyticsgit',
-    version='0.1',
+    version='0.2',
     license='MIT License',
     author='Jefferson Sena',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='jeffersonsena12144@gmail.com',
     keywords='Py Analytics Git',
     description=u'Biblioteca PyAnalyticsGit para gerar relatórios Git.',
     packages=['analyticsgit'],
-    install_requires=['matplotlib==3.7.1',
-                      'python-dotenv==1.0.0',
-                      'Requests==2.31.0',
-                      'setuptools==59.6.0',
-                      'wordcloud==1.9.2'],)
+    install_requires=['requests'],)
```

