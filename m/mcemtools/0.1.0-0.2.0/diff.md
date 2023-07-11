# Comparing `tmp/mcemtools-0.1.0.tar.gz` & `tmp/mcemtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.1.0.tar", last modified: Fri Sep 30 03:12:19 2022, max compression
+gzip compressed data, was "mcemtools-0.2.0.tar", last modified: Tue Jul 11 03:57:10 2023, max compression
```

## Comparing `mcemtools-0.1.0.tar` & `mcemtools-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-09-30 03:12:09.000000 mcemtools-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-09-30 03:12:09.000000 mcemtools-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-30 03:12:09.000000 mcemtools-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-30 03:12:09.000000 mcemtools-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-30 03:12:09.000000 mcemtools-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-09-30 03:12:19.123701 mcemtools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-30 03:12:09.000000 mcemtools-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-30 03:12:09.000000 mcemtools-0.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-09-30 03:12:09.000000 mcemtools-0.1.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-30 03:12:09.000000 mcemtools-0.1.0/mcemtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/mcemtools/denoise/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-30 03:12:09.000000 mcemtools-0.1.0/mcemtools/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-09-30 03:12:09.000000 mcemtools-0.1.0/mcemtools/denoise/denoise_4DSTEM.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-30 03:12:09.000000 mcemtools-0.1.0/mcemtools/mcemtools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 03:12:18.000000 mcemtools-0.1.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-30 03:12:19.000000 mcemtools-0.1.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-30 03:12:09.000000 mcemtools-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-30 03:12:19.123701 mcemtools-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-09-30 03:12:09.000000 mcemtools-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 03:12:19.123701 mcemtools-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-30 03:12:09.000000 mcemtools-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-09-30 03:12:09.000000 mcemtools-0.1.0/tests/test_mcemtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 03:57:00.000000 mcemtools-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-11 03:57:00.000000 mcemtools-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 03:57:00.000000 mcemtools-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 03:57:00.000000 mcemtools-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 03:57:00.000000 mcemtools-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 03:57:10.011534 mcemtools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 03:57:00.000000 mcemtools-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.007534 mcemtools-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 03:57:00.000000 mcemtools-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-11 03:57:00.000000 mcemtools-0.2.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 03:57:10.000000 mcemtools-0.2.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 03:57:09.000000 mcemtools-0.2.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 03:57:00.000000 mcemtools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 03:57:10.015534 mcemtools-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-11 03:57:00.000000 mcemtools-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:57:10.011534 mcemtools-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 03:57:00.000000 mcemtools-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-11 03:57:00.000000 mcemtools-0.2.0/tests/test_mcemtools.py
```

### Comparing `mcemtools-0.1.0/CONTRIBUTING.rst` & `mcemtools-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/LICENSE` & `mcemtools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/PKG-INFO` & `mcemtools-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =========
 mcemtools
 =========
 
@@ -66,7 +68,13 @@
 History
 =======
 
 0.1.0 (2022-09-07)
 ------------------
 
 * First release on PyPI.
+
+0.2.0 (2023-07-11)
+------------------
+
+* Many functions used for 4D-STEM analysis have been added.
+* OOP is avoided as much as possible.
```

### Comparing `mcemtools-0.1.0/README.rst` & `mcemtools-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/docs/Makefile` & `mcemtools-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/docs/conf.py` & `mcemtools-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/docs/installation.rst` & `mcemtools-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/docs/make.bat` & `mcemtools-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.1.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.2.0/mcemtools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =========
 mcemtools
 =========
 
@@ -66,7 +68,13 @@
 History
 =======
 
 0.1.0 (2022-09-07)
 ------------------
 
 * First release on PyPI.
+
+0.2.0 (2023-07-11)
+------------------
+
+* Many functions used for 4D-STEM analysis have been added.
+* OOP is avoided as much as possible.
```

### Comparing `mcemtools-0.1.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.2.0/mcemtools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 docs/installation.rst
 docs/make.bat
 docs/mcemtools.denoise.rst
 docs/mcemtools.rst
 docs/readme.rst
 docs/usage.rst
 mcemtools/__init__.py
+mcemtools/analysis.py
 mcemtools/cli.py
+mcemtools/masking.py
 mcemtools/mcemtools.py
+mcemtools/tensor_svd.py
+mcemtools/transforms.py
 mcemtools.egg-info/PKG-INFO
 mcemtools.egg-info/SOURCES.txt
 mcemtools.egg-info/dependency_links.txt
 mcemtools.egg-info/entry_points.txt
 mcemtools.egg-info/not-zip-safe
 mcemtools.egg-info/requires.txt
 mcemtools.egg-info/top_level.txt
-mcemtools/denoise/__init__.py
-mcemtools/denoise/denoise_4DSTEM.py
 tests/__init__.py
 tests/test_mcemtools.py
```

### Comparing `mcemtools-0.1.0/setup.py` & `mcemtools-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
+_version = '0.2.0'
+
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
@@ -13,24 +15,26 @@
 requirements = ['Click>=7.0', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alireza Sadri",
     author_email='Alireza.Sadri@monash.edu',
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="State of the art analysis tools for electron microscopy",
     entry_points={
         'console_scripts': [
             'mcemtools=mcemtools.cli:main',
         ],
     },
@@ -40,10 +44,10 @@
     include_package_data=True,
     keywords='mcemtools',
     name='mcemtools',
     packages=find_packages(include=['mcemtools', 'mcemtools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/arsadri/mcemtools',
-    version='0.1.0',
+    version=_version,
     zip_safe=False,
 )
```

