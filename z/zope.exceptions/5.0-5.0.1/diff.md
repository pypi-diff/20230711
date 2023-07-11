# Comparing `tmp/zope.exceptions-5.0.tar.gz` & `tmp/zope.exceptions-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.exceptions-5.0.tar", last modified: Thu Jun 29 06:08:19 2023, max compression
+gzip compressed data, was "zope.exceptions-5.0.1.tar", last modified: Tue Jul 11 07:40:38 2023, max compression
```

## Comparing `zope.exceptions-5.0.tar` & `zope.exceptions-5.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439715 zope.exceptions-5.0/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5499 2023-06-29 06:08:19.000000 zope.exceptions-5.0/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-06-29 06:08:19.000000 zope.exceptions-5.0/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-06-29 06:08:19.000000 zope.exceptions-5.0/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-06-29 06:08:19.000000 zope.exceptions-5.0/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      344 2023-06-29 06:08:19.000000 zope.exceptions-5.0/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)     8034 2023-06-29 06:08:19.439772 zope.exceptions-5.0/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1175 2023-06-29 06:08:19.000000 zope.exceptions-5.0/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       97 2023-06-29 06:08:19.000000 zope.exceptions-5.0/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.437454 zope.exceptions-5.0/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5596 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/Makefile
--rw-r--r--   0 m.howitz   (502) staff       (20)     1166 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/api.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     8197 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     9152 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/hacking.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      236 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5112 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/make.bat
--rw-r--r--   0 m.howitz   (502) staff       (20)     5970 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/narr.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-06-29 06:08:19.000000 zope.exceptions-5.0/rtd.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-06-29 06:08:19.439997 zope.exceptions-5.0/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2023-06-29 06:08:19.000000 zope.exceptions-5.0/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.434629 zope.exceptions-5.0/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.437587 zope.exceptions-5.0/src/zope/
--rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439141 zope.exceptions-5.0/src/zope/exceptions/
--rw-r--r--   0 m.howitz   (502) staff       (20)     2122 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    11235 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/exceptionformatter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3439 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1236 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/log.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439582 zope.exceptions-5.0/src/zope/exceptions/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)        2 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    35450 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/test_exceptionformatter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2858 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/test_log.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.438573 zope.exceptions-5.0/src/zope.exceptions.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)     8034 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      817 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)       93 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1828 2023-06-29 06:08:19.000000 zope.exceptions-5.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.827049 zope.exceptions-5.0.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5673 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      344 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8210 2023-07-11 07:40:38.827126 zope.exceptions-5.0.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1175 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       97 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.824441 zope.exceptions-5.0.1/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5596 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1166 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8197 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9152 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      236 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5112 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5970 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/docs/narr.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/rtd.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-07-11 07:40:38.827421 zope.exceptions-5.0.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3017 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.821355 zope.exceptions-5.0.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.824606 zope.exceptions-5.0.1/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.826448 zope.exceptions-5.0.1/src/zope/exceptions/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2122 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11240 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/exceptionformatter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3439 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1236 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/log.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.826916 zope.exceptions-5.0.1/src/zope/exceptions/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        2 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    35565 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/tests/test_exceptionformatter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2858 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope/exceptions/tests/test_log.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 07:40:38.825851 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8210 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      817 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       93 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/src/zope.exceptions.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1828 2023-07-11 07:40:38.000000 zope.exceptions-5.0.1/tox.ini
```

### Comparing `zope.exceptions-5.0/CHANGES.rst` & `zope.exceptions-5.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0.1 (2023-07-11)
+==================
+
+- Fix issue introduced in the last release which is breaking
+  ``HTMLExceptionFormatter`` when using non-str ``__traceback_info__``.
+
+
 5.0 (2023-06-29)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.6 (2022-11-10)
```

### Comparing `zope.exceptions-5.0/CONTRIBUTING.md` & `zope.exceptions-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/LICENSE.txt` & `zope.exceptions-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/PKG-INFO` & `zope.exceptions-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.exceptions
-Version: 5.0
+Version: 5.0.1
 Summary: Zope Exceptions
 Home-page: https://github.com/zopefoundation/zope.exceptions
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.exceptions/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.exceptions
@@ -59,14 +59,21 @@
 Please see https://zopeexceptions.readthedocs.io/ for the documentation.
 
 
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0.1 (2023-07-11)
+==================
+
+- Fix issue introduced in the last release which is breaking
+  ``HTMLExceptionFormatter`` when using non-str ``__traceback_info__``.
+
+
 5.0 (2023-06-29)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.6 (2022-11-10)
```

### Comparing `zope.exceptions-5.0/README.rst` & `zope.exceptions-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/Makefile` & `zope.exceptions-5.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/api.rst` & `zope.exceptions-5.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/conf.py` & `zope.exceptions-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/hacking.rst` & `zope.exceptions-5.0.1/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/make.bat` & `zope.exceptions-5.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/docs/narr.rst` & `zope.exceptions-5.0.1/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/setup.py` & `zope.exceptions-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name='zope.exceptions',
-    version='5.0',
+    version='5.0.1',
     author='Zope Foundation and Contributors',
     author_email='zope-dev@zope.dev',
     description='Zope Exceptions',
     long_description=(read('README.rst') + '\n\n' +
                       read('CHANGES.rst')),
     keywords='zope exceptions',
     classifiers=[
```

### Comparing `zope.exceptions-5.0/src/zope/exceptions/__init__.py` & `zope.exceptions-5.0.1/src/zope/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/src/zope/exceptions/exceptionformatter.py` & `zope.exceptions-5.0.1/src/zope/exceptions/exceptionformatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
 
 class HTMLExceptionFormatter(TextExceptionFormatter):
 
     line_sep = '<br />\r\n'
 
     def escape(self, s):
-        return escape(s, quote=False)
+        return escape(str(s), quote=False)
 
     def getPrefix(self):
         return '<p>Traceback (most recent call last):</p>\r\n<ul>'
 
     def formatSupplementLine(self, line):
         return '<b>%s</b>' % self.escape(line)
```

### Comparing `zope.exceptions-5.0/src/zope/exceptions/interfaces.py` & `zope.exceptions-5.0.1/src/zope/exceptions/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/src/zope/exceptions/log.py` & `zope.exceptions-5.0.1/src/zope/exceptions/log.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/src/zope/exceptions/tests/test_exceptionformatter.py` & `zope.exceptions-5.0.1/src/zope/exceptions/tests/test_exceptionformatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,14 +510,18 @@
         self.assertEqual(fmt.limit, 20)
         self.assertEqual(fmt.with_filenames, True)
 
     def test_escape_simple(self):
         fmt = self._makeOne()
         self.assertEqual(fmt.escape('XXX'), 'XXX')
 
+    def test_escape_non_str(self):
+        fmt = self._makeOne()
+        self.assertEqual(fmt.escape(123), '123')
+
     def test_escape_w_markup(self):
         fmt = self._makeOne()
         self.assertEqual(fmt.escape('<span>XXX & YYY<span>'),
                          '&lt;span&gt;XXX &amp; YYY&lt;span&gt;')
 
     def test_getPrefix(self):
         fmt = self._makeOne()
```

### Comparing `zope.exceptions-5.0/src/zope/exceptions/tests/test_log.py` & `zope.exceptions-5.0.1/src/zope/exceptions/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/src/zope.exceptions.egg-info/PKG-INFO` & `zope.exceptions-5.0.1/src/zope.exceptions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.exceptions
-Version: 5.0
+Version: 5.0.1
 Summary: Zope Exceptions
 Home-page: https://github.com/zopefoundation/zope.exceptions
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.exceptions/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.exceptions
@@ -59,14 +59,21 @@
 Please see https://zopeexceptions.readthedocs.io/ for the documentation.
 
 
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0.1 (2023-07-11)
+==================
+
+- Fix issue introduced in the last release which is breaking
+  ``HTMLExceptionFormatter`` when using non-str ``__traceback_info__``.
+
+
 5.0 (2023-06-29)
 ================
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.6 (2022-11-10)
```

### Comparing `zope.exceptions-5.0/src/zope.exceptions.egg-info/SOURCES.txt` & `zope.exceptions-5.0.1/src/zope.exceptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.exceptions-5.0/tox.ini` & `zope.exceptions-5.0.1/tox.ini`

 * *Files identical despite different names*

