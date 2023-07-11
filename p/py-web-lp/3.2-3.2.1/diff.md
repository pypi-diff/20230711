# Comparing `tmp/py-web-lp-3.2.tar.gz` & `tmp/py-web-lp-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-web-lp-3.2.tar", last modified: Tue Jul 11 13:17:55 2023, max compression
+gzip compressed data, was "py-web-lp-3.2.1.tar", last modified: Tue Jul 11 17:02:09 2023, max compression
```

## Comparing `py-web-lp-3.2.tar` & `py-web-lp-3.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:55.010384 py-web-lp-3.2/
--rw-r--r--   0 slott      (503) staff       (20)     1514 2022-06-10 14:40:12.000000 py-web-lp-3.2/LICENSE
--rw-------   0 slott      (503) staff       (20)      177 2022-06-12 23:24:53.000000 py-web-lp-3.2/MANIFEST.in
--rw-r--r--   0 slott      (503) staff       (20)     4276 2023-07-11 13:17:55.009922 py-web-lp-3.2/PKG-INFO
--rw-------   0 slott      (503) staff       (20)     3184 2023-07-11 13:09:24.000000 py-web-lp-3.2/README.rst
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:54.954675 py-web-lp-3.2/bootstrap/
--rw-r--r--   0 slott      (503) staff       (20)    69822 2022-06-16 18:21:29.000000 py-web-lp-3.2/bootstrap/pyweb.py
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:54.956820 py-web-lp-3.2/jedit/
--rw-r--r--   0 slott      (503) staff       (20)     4423 2022-06-10 14:40:12.000000 py-web-lp-3.2/jedit/pyweb.xml
--rw-------   0 slott      (503) staff       (20)     1485 2023-07-11 13:14:53.000000 py-web-lp-3.2/pyproject.toml
--rw-r--r--   0 slott      (503) staff       (20)       38 2023-07-11 13:17:55.010581 py-web-lp-3.2/setup.cfg
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:54.979303 py-web-lp-3.2/src/
--rw-r--r--   0 slott      (503) staff       (20)     2174 2022-07-16 16:22:09.000000 py-web-lp-3.2/src/conf.py
--rw-r--r--   0 slott      (503) staff       (20)     7919 2023-07-11 13:14:21.000000 py-web-lp-3.2/src/done.w
--rw-r--r--   0 slott      (503) staff       (20)   125024 2023-07-11 13:03:19.000000 py-web-lp-3.2/src/impl.w
--rw-r--r--   0 slott      (503) staff       (20)    13030 2023-07-11 13:04:54.000000 py-web-lp-3.2/src/intro.w
--rw-r--r--   0 slott      (503) staff       (20)    17066 2023-07-11 13:04:54.000000 py-web-lp-3.2/src/language.w
--rw-r--r--   0 slott      (503) staff       (20)    13121 2023-07-11 13:05:21.000000 py-web-lp-3.2/src/overview.w
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:54.983164 py-web-lp-3.2/src/py_web_lp.egg-info/
--rw-r--r--   0 slott      (503) staff       (20)     4276 2023-07-11 13:17:54.000000 py-web-lp-3.2/src/py_web_lp.egg-info/PKG-INFO
--rw-r--r--   0 slott      (503) staff       (20)      746 2023-07-11 13:17:54.000000 py-web-lp-3.2/src/py_web_lp.egg-info/SOURCES.txt
--rw-r--r--   0 slott      (503) staff       (20)        1 2023-07-11 13:17:54.000000 py-web-lp-3.2/src/py_web_lp.egg-info/dependency_links.txt
--rw-r--r--   0 slott      (503) staff       (20)      190 2023-07-11 13:17:54.000000 py-web-lp-3.2/src/py_web_lp.egg-info/requires.txt
--rw-r--r--   0 slott      (503) staff       (20)       50 2023-07-11 13:17:54.000000 py-web-lp-3.2/src/py_web_lp.egg-info/top_level.txt
--rw-------   0 slott      (503) staff       (20)    59831 2023-07-11 13:11:24.000000 py-web-lp-3.2/src/pyweb.py
--rw-r--r--   0 slott      (503) staff       (20)   236975 2023-07-11 13:15:02.000000 py-web-lp-3.2/src/pyweb.rst
--rwxr-xr-x   0 slott      (503) staff       (20)      750 2022-07-03 17:07:49.000000 py-web-lp-3.2/src/pyweb.w
--rw-r--r--   0 slott      (503) staff       (20)     4385 2022-07-19 13:40:24.000000 py-web-lp-3.2/src/scripts.w
--rw-------   0 slott      (503) staff       (20)      803 2022-07-19 13:40:27.000000 py-web-lp-3.2/src/tangle.py
--rw-r--r--   0 slott      (503) staff       (20)      854 2022-06-12 23:33:11.000000 py-web-lp-3.2/src/tests.w
--rw-r--r--   0 slott      (503) staff       (20)     2791 2023-07-11 13:05:36.000000 py-web-lp-3.2/src/todo.w
--rw-r--r--   0 slott      (503) staff       (20)     9086 2023-07-11 13:06:15.000000 py-web-lp-3.2/src/usage.w
--rw-------   0 slott      (503) staff       (20)     1841 2022-07-19 13:40:27.000000 py-web-lp-3.2/src/weave.py
-drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 13:17:55.007539 py-web-lp-3.2/tests/
--rw-------   0 slott      (503) staff       (20)      206 2022-07-01 00:07:53.000000 py-web-lp-3.2/tests/docutils.conf
--rw-r--r--   0 slott      (503) staff       (20)    16830 2022-07-19 13:40:46.000000 py-web-lp-3.2/tests/func.w
--rw-r--r--   0 slott      (503) staff       (20)     2444 2022-06-10 14:48:04.000000 py-web-lp-3.2/tests/intro.w
--rw-------   0 slott      (503) staff       (20)      315 2022-07-01 00:07:53.000000 py-web-lp-3.2/tests/page-layout.css
--rwxr-xr-x   0 slott      (503) staff       (20)     1326 2010-02-13 18:33:07.000000 py-web-lp-3.2/tests/pyweb.css
--rw-r--r--   0 slott      (503) staff       (20)   155255 2022-07-19 18:29:45.000000 py-web-lp-3.2/tests/pyweb_test.html
--rw-r--r--   0 slott      (503) staff       (20)     1734 2022-07-02 13:39:56.000000 py-web-lp-3.2/tests/pyweb_test.w
--rw-------   0 slott      (503) staff       (20)     1443 2022-06-10 21:03:49.000000 py-web-lp-3.2/tests/runner.py
--rw-r--r--   0 slott      (503) staff       (20)     3068 2022-06-10 21:07:30.000000 py-web-lp-3.2/tests/runner.w
--rw-r--r--   0 slott      (503) staff       (20)     6405 2022-07-04 20:16:47.000000 py-web-lp-3.2/tests/scripts.w
--rw-------   0 slott      (503) staff       (20)     2561 2022-07-01 12:25:36.000000 py-web-lp-3.2/tests/test_loader.py
--rw-------   0 slott      (503) staff       (20)     4873 2022-07-04 20:17:05.000000 py-web-lp-3.2/tests/test_scripts.py
--rw-------   0 slott      (503) staff       (20)     4592 2022-07-02 21:24:15.000000 py-web-lp-3.2/tests/test_tangler.py
--rw-------   0 slott      (503) staff       (20)    34825 2022-07-19 18:29:44.000000 py-web-lp-3.2/tests/test_unit.py
--rw-------   0 slott      (503) staff       (20)     5413 2022-07-19 13:40:48.000000 py-web-lp-3.2/tests/test_weaver.py
--rw-r--r--   0 slott      (503) staff       (20)    47615 2022-07-19 18:29:41.000000 py-web-lp-3.2/tests/unit.w
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.556676 py-web-lp-3.2.1/
+-rw-r--r--   0 slott      (503) staff       (20)     1514 2022-06-10 14:40:12.000000 py-web-lp-3.2.1/LICENSE
+-rw-------   0 slott      (503) staff       (20)      177 2022-06-12 23:24:53.000000 py-web-lp-3.2.1/MANIFEST.in
+-rw-r--r--   0 slott      (503) staff       (20)     4302 2023-07-11 17:02:09.556092 py-web-lp-3.2.1/PKG-INFO
+-rw-------   0 slott      (503) staff       (20)     3208 2023-07-11 13:20:59.000000 py-web-lp-3.2.1/README.rst
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.500716 py-web-lp-3.2.1/bootstrap/
+-rw-r--r--   0 slott      (503) staff       (20)    69822 2022-06-16 18:21:29.000000 py-web-lp-3.2.1/bootstrap/pyweb.py
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.502742 py-web-lp-3.2.1/jedit/
+-rw-r--r--   0 slott      (503) staff       (20)     4423 2022-06-10 14:40:12.000000 py-web-lp-3.2.1/jedit/pyweb.xml
+-rw-------   0 slott      (503) staff       (20)     1487 2023-07-11 17:01:59.000000 py-web-lp-3.2.1/pyproject.toml
+-rw-r--r--   0 slott      (503) staff       (20)       38 2023-07-11 17:02:09.556937 py-web-lp-3.2.1/setup.cfg
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.526101 py-web-lp-3.2.1/src/
+-rw-r--r--   0 slott      (503) staff       (20)     2174 2022-07-16 16:22:09.000000 py-web-lp-3.2.1/src/conf.py
+-rw-r--r--   0 slott      (503) staff       (20)     7919 2023-07-11 13:14:21.000000 py-web-lp-3.2.1/src/done.w
+-rw-r--r--   0 slott      (503) staff       (20)   125024 2023-07-11 13:03:19.000000 py-web-lp-3.2.1/src/impl.w
+-rw-r--r--   0 slott      (503) staff       (20)    13030 2023-07-11 13:04:54.000000 py-web-lp-3.2.1/src/intro.w
+-rw-r--r--   0 slott      (503) staff       (20)    17066 2023-07-11 13:04:54.000000 py-web-lp-3.2.1/src/language.w
+-rw-r--r--   0 slott      (503) staff       (20)    13121 2023-07-11 13:05:21.000000 py-web-lp-3.2.1/src/overview.w
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.530409 py-web-lp-3.2.1/src/py_web_lp.egg-info/
+-rw-r--r--   0 slott      (503) staff       (20)     4302 2023-07-11 17:02:09.000000 py-web-lp-3.2.1/src/py_web_lp.egg-info/PKG-INFO
+-rw-r--r--   0 slott      (503) staff       (20)      746 2023-07-11 17:02:09.000000 py-web-lp-3.2.1/src/py_web_lp.egg-info/SOURCES.txt
+-rw-r--r--   0 slott      (503) staff       (20)        1 2023-07-11 17:02:09.000000 py-web-lp-3.2.1/src/py_web_lp.egg-info/dependency_links.txt
+-rw-r--r--   0 slott      (503) staff       (20)      190 2023-07-11 17:02:09.000000 py-web-lp-3.2.1/src/py_web_lp.egg-info/requires.txt
+-rw-r--r--   0 slott      (503) staff       (20)       50 2023-07-11 17:02:09.000000 py-web-lp-3.2.1/src/py_web_lp.egg-info/top_level.txt
+-rw-------   0 slott      (503) staff       (20)    59831 2023-07-11 13:11:24.000000 py-web-lp-3.2.1/src/pyweb.py
+-rw-r--r--   0 slott      (503) staff       (20)   236975 2023-07-11 13:15:02.000000 py-web-lp-3.2.1/src/pyweb.rst
+-rwxr-xr-x   0 slott      (503) staff       (20)      750 2022-07-03 17:07:49.000000 py-web-lp-3.2.1/src/pyweb.w
+-rw-r--r--   0 slott      (503) staff       (20)     4385 2022-07-19 13:40:24.000000 py-web-lp-3.2.1/src/scripts.w
+-rw-------   0 slott      (503) staff       (20)      803 2022-07-19 13:40:27.000000 py-web-lp-3.2.1/src/tangle.py
+-rw-r--r--   0 slott      (503) staff       (20)      854 2022-06-12 23:33:11.000000 py-web-lp-3.2.1/src/tests.w
+-rw-r--r--   0 slott      (503) staff       (20)     2791 2023-07-11 13:05:36.000000 py-web-lp-3.2.1/src/todo.w
+-rw-r--r--   0 slott      (503) staff       (20)     9086 2023-07-11 13:06:15.000000 py-web-lp-3.2.1/src/usage.w
+-rw-------   0 slott      (503) staff       (20)     1841 2022-07-19 13:40:27.000000 py-web-lp-3.2.1/src/weave.py
+drwxr-xr-x   0 slott      (503) staff       (20)        0 2023-07-11 17:02:09.554106 py-web-lp-3.2.1/tests/
+-rw-------   0 slott      (503) staff       (20)      206 2022-07-01 00:07:53.000000 py-web-lp-3.2.1/tests/docutils.conf
+-rw-r--r--   0 slott      (503) staff       (20)    16830 2022-07-19 13:40:46.000000 py-web-lp-3.2.1/tests/func.w
+-rw-r--r--   0 slott      (503) staff       (20)     2444 2022-06-10 14:48:04.000000 py-web-lp-3.2.1/tests/intro.w
+-rw-------   0 slott      (503) staff       (20)      315 2022-07-01 00:07:53.000000 py-web-lp-3.2.1/tests/page-layout.css
+-rwxr-xr-x   0 slott      (503) staff       (20)     1326 2010-02-13 18:33:07.000000 py-web-lp-3.2.1/tests/pyweb.css
+-rw-r--r--   0 slott      (503) staff       (20)   155255 2022-07-19 18:29:45.000000 py-web-lp-3.2.1/tests/pyweb_test.html
+-rw-r--r--   0 slott      (503) staff       (20)     1734 2022-07-02 13:39:56.000000 py-web-lp-3.2.1/tests/pyweb_test.w
+-rw-------   0 slott      (503) staff       (20)     1443 2022-06-10 21:03:49.000000 py-web-lp-3.2.1/tests/runner.py
+-rw-r--r--   0 slott      (503) staff       (20)     3068 2022-06-10 21:07:30.000000 py-web-lp-3.2.1/tests/runner.w
+-rw-r--r--   0 slott      (503) staff       (20)     6405 2022-07-04 20:16:47.000000 py-web-lp-3.2.1/tests/scripts.w
+-rw-------   0 slott      (503) staff       (20)     2561 2022-07-01 12:25:36.000000 py-web-lp-3.2.1/tests/test_loader.py
+-rw-------   0 slott      (503) staff       (20)     4873 2022-07-04 20:17:05.000000 py-web-lp-3.2.1/tests/test_scripts.py
+-rw-------   0 slott      (503) staff       (20)     4592 2022-07-02 21:24:15.000000 py-web-lp-3.2.1/tests/test_tangler.py
+-rw-------   0 slott      (503) staff       (20)    34825 2022-07-19 18:29:44.000000 py-web-lp-3.2.1/tests/test_unit.py
+-rw-------   0 slott      (503) staff       (20)     5413 2022-07-19 13:40:48.000000 py-web-lp-3.2.1/tests/test_weaver.py
+-rw-r--r--   0 slott      (503) staff       (20)    47615 2022-07-19 18:29:41.000000 py-web-lp-3.2.1/tests/unit.w
```

### Comparing `py-web-lp-3.2/LICENSE` & `py-web-lp-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/PKG-INFO` & `py-web-lp-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-web-lp
-Version: 3.2
+Version: 3.2.1
 Summary: py-web-lp: Yet Another Literate Programming Tool
 Author-email: "S.Lott" <slott56@gmail.com>
 License: BSD
 Project-URL: repository, https://github.com/slott56/py-web-tool
 Project-URL: documentation, https://slott56.github.io/py-web-tool/src/pyweb.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -50,15 +50,15 @@
 Installation
 -------------
 
 This requires Python 3.10. 
 
 ::
 
-    python -m install py-web-lp
+    python -m pip install py-web-lp
     
 This will install the ``pyweb`` module and all of its dependencies.
 
 Produce Documentation
 ---------------------
 
 The supplied documentation uses RST markup; it requires docutils.
@@ -88,15 +88,15 @@
 After installation and authoring, you can then run **py-web-lp** with the following
 command
 
 ::
 
     python3 -m pyweb src/pyweb.w -o src 
 
-This will create the various output files from the source ```.w`` file.
+This will create the various output files from the source ``.w`` file.
 
 -   ``pyweb.rst`` is the final woven document. This can be run through docutils for publication.
 
 -   ``pyweb.py``, ``tangle.py``, ``weave.py`` are the tangled code files.
 
 All of the files are produced from a single source.
 
@@ -118,15 +118,15 @@
 
 Use **pytest** to run all the tests.
 
 Here's a typical sequence, used during development:
 
 ::
 
-	python3 bootstrap/pyweb.py -xw src/pyweb.w -o src 
-	python3 src/pyweb.py tests/pyweb_test.w -o tests
-	PYTHONPATH=${PWD}/src pytest
-	rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
+    python3 bootstrap/pyweb.py -xw src/pyweb.w -o src
+    python3 src/pyweb.py tests/pyweb_test.w -o tests
+    PYTHONPATH=${PWD}/src pytest
+    rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
     mypy --strict src
 
-Note that a previous release, untouched, is saved in the ``bootstrap`` directory.
+Note that a previous release, untouched, is saved in the project's ``bootstrap`` directory.
 This is **not** changed during development, since **py-web-lp** is written with **py-web-lp**.
```

### Comparing `py-web-lp-3.2/README.rst` & `py-web-lp-3.2.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Installation
 -------------
 
 This requires Python 3.10. 
 
 ::
 
-    python -m install py-web-lp
+    python -m pip install py-web-lp
     
 This will install the ``pyweb`` module and all of its dependencies.
 
 Produce Documentation
 ---------------------
 
 The supplied documentation uses RST markup; it requires docutils.
@@ -60,15 +60,15 @@
 After installation and authoring, you can then run **py-web-lp** with the following
 command
 
 ::
 
     python3 -m pyweb src/pyweb.w -o src 
 
-This will create the various output files from the source ```.w`` file.
+This will create the various output files from the source ``.w`` file.
 
 -   ``pyweb.rst`` is the final woven document. This can be run through docutils for publication.
 
 -   ``pyweb.py``, ``tangle.py``, ``weave.py`` are the tangled code files.
 
 All of the files are produced from a single source.
 
@@ -90,15 +90,15 @@
 
 Use **pytest** to run all the tests.
 
 Here's a typical sequence, used during development:
 
 ::
 
-	python3 bootstrap/pyweb.py -xw src/pyweb.w -o src 
-	python3 src/pyweb.py tests/pyweb_test.w -o tests
-	PYTHONPATH=${PWD}/src pytest
-	rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
+    python3 bootstrap/pyweb.py -xw src/pyweb.w -o src
+    python3 src/pyweb.py tests/pyweb_test.w -o tests
+    PYTHONPATH=${PWD}/src pytest
+    rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
     mypy --strict src
 
-Note that a previous release, untouched, is saved in the ``bootstrap`` directory.
+Note that a previous release, untouched, is saved in the project's ``bootstrap`` directory.
 This is **not** changed during development, since **py-web-lp** is written with **py-web-lp**.
```

### Comparing `py-web-lp-3.2/bootstrap/pyweb.py` & `py-web-lp-3.2.1/bootstrap/pyweb.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/jedit/pyweb.xml` & `py-web-lp-3.2.1/jedit/pyweb.xml`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/pyproject.toml` & `py-web-lp-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.2.0", "wheel >= 0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
-version = "3.2"
+version = "3.2.1"
 requires-python = ">=3.10"
 name = "py-web-lp"
 description="py-web-lp: Yet Another Literate Programming Tool"
 readme = "README.rst"
 authors = [{"name" = "S.Lott", "email" = "slott56@gmail.com"}]
 license = {text = "BSD"}
 classifiers = [
```

### Comparing `py-web-lp-3.2/src/conf.py` & `py-web-lp-3.2.1/src/conf.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/done.w` & `py-web-lp-3.2.1/src/done.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/impl.w` & `py-web-lp-3.2.1/src/impl.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/intro.w` & `py-web-lp-3.2.1/src/intro.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/language.w` & `py-web-lp-3.2.1/src/language.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/overview.w` & `py-web-lp-3.2.1/src/overview.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/py_web_lp.egg-info/PKG-INFO` & `py-web-lp-3.2.1/src/py_web_lp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-web-lp
-Version: 3.2
+Version: 3.2.1
 Summary: py-web-lp: Yet Another Literate Programming Tool
 Author-email: "S.Lott" <slott56@gmail.com>
 License: BSD
 Project-URL: repository, https://github.com/slott56/py-web-tool
 Project-URL: documentation, https://slott56.github.io/py-web-tool/src/pyweb.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -50,15 +50,15 @@
 Installation
 -------------
 
 This requires Python 3.10. 
 
 ::
 
-    python -m install py-web-lp
+    python -m pip install py-web-lp
     
 This will install the ``pyweb`` module and all of its dependencies.
 
 Produce Documentation
 ---------------------
 
 The supplied documentation uses RST markup; it requires docutils.
@@ -88,15 +88,15 @@
 After installation and authoring, you can then run **py-web-lp** with the following
 command
 
 ::
 
     python3 -m pyweb src/pyweb.w -o src 
 
-This will create the various output files from the source ```.w`` file.
+This will create the various output files from the source ``.w`` file.
 
 -   ``pyweb.rst`` is the final woven document. This can be run through docutils for publication.
 
 -   ``pyweb.py``, ``tangle.py``, ``weave.py`` are the tangled code files.
 
 All of the files are produced from a single source.
 
@@ -118,15 +118,15 @@
 
 Use **pytest** to run all the tests.
 
 Here's a typical sequence, used during development:
 
 ::
 
-	python3 bootstrap/pyweb.py -xw src/pyweb.w -o src 
-	python3 src/pyweb.py tests/pyweb_test.w -o tests
-	PYTHONPATH=${PWD}/src pytest
-	rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
+    python3 bootstrap/pyweb.py -xw src/pyweb.w -o src
+    python3 src/pyweb.py tests/pyweb_test.w -o tests
+    PYTHONPATH=${PWD}/src pytest
+    rst2html.py tests/pyweb_test.rst tests/pyweb_test.html
     mypy --strict src
 
-Note that a previous release, untouched, is saved in the ``bootstrap`` directory.
+Note that a previous release, untouched, is saved in the project's ``bootstrap`` directory.
 This is **not** changed during development, since **py-web-lp** is written with **py-web-lp**.
```

### Comparing `py-web-lp-3.2/src/py_web_lp.egg-info/SOURCES.txt` & `py-web-lp-3.2.1/src/py_web_lp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/pyweb.py` & `py-web-lp-3.2.1/src/pyweb.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/pyweb.rst` & `py-web-lp-3.2.1/src/pyweb.rst`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/pyweb.w` & `py-web-lp-3.2.1/src/pyweb.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/scripts.w` & `py-web-lp-3.2.1/src/scripts.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/tangle.py` & `py-web-lp-3.2.1/src/tangle.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/tests.w` & `py-web-lp-3.2.1/src/tests.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/todo.w` & `py-web-lp-3.2.1/src/todo.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/usage.w` & `py-web-lp-3.2.1/src/usage.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/src/weave.py` & `py-web-lp-3.2.1/src/weave.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/func.w` & `py-web-lp-3.2.1/tests/func.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/intro.w` & `py-web-lp-3.2.1/tests/intro.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/pyweb.css` & `py-web-lp-3.2.1/tests/pyweb.css`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/pyweb_test.html` & `py-web-lp-3.2.1/tests/pyweb_test.html`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/pyweb_test.w` & `py-web-lp-3.2.1/tests/pyweb_test.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/runner.py` & `py-web-lp-3.2.1/tests/runner.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/runner.w` & `py-web-lp-3.2.1/tests/runner.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/scripts.w` & `py-web-lp-3.2.1/tests/scripts.w`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/test_loader.py` & `py-web-lp-3.2.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/test_scripts.py` & `py-web-lp-3.2.1/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/test_tangler.py` & `py-web-lp-3.2.1/tests/test_tangler.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/test_unit.py` & `py-web-lp-3.2.1/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/test_weaver.py` & `py-web-lp-3.2.1/tests/test_weaver.py`

 * *Files identical despite different names*

### Comparing `py-web-lp-3.2/tests/unit.w` & `py-web-lp-3.2.1/tests/unit.w`

 * *Files identical despite different names*

