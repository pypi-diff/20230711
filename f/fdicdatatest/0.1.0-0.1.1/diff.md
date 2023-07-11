# Comparing `tmp/fdicdatatest-0.1.0.tar.gz` & `tmp/fdicdatatest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdicdatatest-0.1.0.tar", last modified: Tue Jul 11 12:40:35 2023, max compression
+gzip compressed data, was "fdicdatatest-0.1.1.tar", last modified: Tue Jul 11 13:00:16 2023, max compression
```

## Comparing `fdicdatatest-0.1.0.tar` & `fdicdatatest-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:40:35.336274 fdicdatatest-0.1.0/
--rw-rw-rw-   0        0        0     1069 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      905 2023-07-11 12:40:35.334887 fdicdatatest-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 12:40:35.322388 fdicdatatest-0.1.0/fdicdatatest.egg-info/
--rw-rw-rw-   0        0        0      905 2023-07-11 12:40:35.000000 fdicdatatest-0.1.0/fdicdatatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-07-11 12:40:35.000000 fdicdatatest-0.1.0/fdicdatatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:40:35.000000 fdicdatatest-0.1.0/fdicdatatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-11 12:40:35.000000 fdicdatatest-0.1.0/fdicdatatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 12:40:35.000000 fdicdatatest-0.1.0/fdicdatatest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 12:40:35.336274 fdicdatatest-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-07-11 12:37:53.000000 fdicdatatest-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:40:35.332887 fdicdatatest-0.1.0/source/
--rw-rw-rw-   0        0        0      347 2023-07-11 10:20:12.000000 fdicdatatest-0.1.0/source/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/dataTaxonomy.py
--rw-rw-rw-   0        0        0     1130 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/getFailures.py
--rw-rw-rw-   0        0        0     1312 2023-07-11 10:26:40.000000 fdicdatatest-0.1.0/source/getFinancials.py
--rw-rw-rw-   0        0        0      895 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/getHistory.py
--rw-rw-rw-   0        0        0     1382 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/getInstitution.py
--rw-rw-rw-   0        0        0      613 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/getLocation.py
--rw-rw-rw-   0        0        0     1301 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/getSummary.py
--rw-rw-rw-   0        0        0      441 2023-07-10 09:13:21.000000 fdicdatatest-0.1.0/source/get_institutions_all.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:40:35.333887 fdicdatatest-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-10 14:34:30.000000 fdicdatatest-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0        1 2023-07-10 15:09:36.000000 fdicdatatest-0.1.0/tests/test_fdicdata.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:16.032609 fdicdatatest-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      905 2023-07-11 13:00:16.032609 fdicdatatest-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:16.019606 fdicdatatest-0.1.1/fdicdatatest.egg-info/
+-rw-rw-rw-   0        0        0      905 2023-07-11 13:00:15.000000 fdicdatatest-0.1.1/fdicdatatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-07-11 13:00:15.000000 fdicdatatest-0.1.1/fdicdatatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:00:15.000000 fdicdatatest-0.1.1/fdicdatatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-11 13:00:15.000000 fdicdatatest-0.1.1/fdicdatatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 13:00:15.000000 fdicdatatest-0.1.1/fdicdatatest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:00:16.033610 fdicdatatest-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2023-07-11 12:59:25.000000 fdicdatatest-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:16.029609 fdicdatatest-0.1.1/source/
+-rw-rw-rw-   0        0        0      347 2023-07-11 10:20:12.000000 fdicdatatest-0.1.1/source/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/dataTaxonomy.py
+-rw-rw-rw-   0        0        0     1130 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/getFailures.py
+-rw-rw-rw-   0        0        0     1312 2023-07-11 10:26:40.000000 fdicdatatest-0.1.1/source/getFinancials.py
+-rw-rw-rw-   0        0        0      895 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/getHistory.py
+-rw-rw-rw-   0        0        0     1382 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/getInstitution.py
+-rw-rw-rw-   0        0        0      613 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/getLocation.py
+-rw-rw-rw-   0        0        0     1301 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/getSummary.py
+-rw-rw-rw-   0        0        0      441 2023-07-10 09:13:21.000000 fdicdatatest-0.1.1/source/get_institutions_all.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:16.031610 fdicdatatest-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-10 14:34:30.000000 fdicdatatest-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0        1 2023-07-10 15:09:36.000000 fdicdatatest-0.1.1/tests/test_fdicdata.py
```

### Comparing `fdicdatatest-0.1.0/LICENSE.txt` & `fdicdatatest-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/PKG-INFO` & `fdicdatatest-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdicdatatest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Federal Deposit Insurance Corporation (FDIC) tarafından sigortalanmış kurumlar için finansal verileri almak ve veri taksonomisine erişmek için bir dizi işlev sağlayan bir sistem.
 Home-page: https://github.com/boray1/fdicdataPy
 Author: Ugur Dar, Brian Pillmore, Boray Yıldız
 Author-email: ugurdarr@gmail.com, brian@visbanking.com, boray.yldz@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `fdicdatatest-0.1.0/fdicdatatest.egg-info/PKG-INFO` & `fdicdatatest-0.1.1/fdicdatatest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdicdatatest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Federal Deposit Insurance Corporation (FDIC) tarafından sigortalanmış kurumlar için finansal verileri almak ve veri taksonomisine erişmek için bir dizi işlev sağlayan bir sistem.
 Home-page: https://github.com/boray1/fdicdataPy
 Author: Ugur Dar, Brian Pillmore, Boray Yıldız
 Author-email: ugurdarr@gmail.com, brian@visbanking.com, boray.yldz@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `fdicdatatest-0.1.0/setup.py` & `fdicdatatest-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fdicdatatest",
-    version="0.1.0",
+    version="0.1.1",
     description="Federal Deposit Insurance Corporation (FDIC) tarafından sigortalanmış kurumlar için finansal verileri almak ve veri taksonomisine erişmek için bir dizi işlev sağlayan bir sistem.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Ugur Dar, Brian Pillmore, Boray Yıldız",
     author_email="ugurdarr@gmail.com, brian@visbanking.com, boray.yldz@gmail.com",
     url="https://github.com/boray1/fdicdataPy",
     packages=find_packages(),
@@ -17,13 +17,13 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=[
-        "tempfile>=3.0.0",
-        "requests>=2.25.0",
-        "pyyaml>=5.4.1",
-        "urllib3>=1.26.5",
+        "tempfile",
+        "requests",
+        "pyyaml",
+        "urllib3",
     ],
 )
```

### Comparing `fdicdatatest-0.1.0/source/dataTaxonomy.py` & `fdicdatatest-0.1.1/source/dataTaxonomy.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getFailures.py` & `fdicdatatest-0.1.1/source/getFailures.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getFinancials.py` & `fdicdatatest-0.1.1/source/getFinancials.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getHistory.py` & `fdicdatatest-0.1.1/source/getHistory.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getInstitution.py` & `fdicdatatest-0.1.1/source/getInstitution.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getLocation.py` & `fdicdatatest-0.1.1/source/getLocation.py`

 * *Files identical despite different names*

### Comparing `fdicdatatest-0.1.0/source/getSummary.py` & `fdicdatatest-0.1.1/source/getSummary.py`

 * *Files identical despite different names*

