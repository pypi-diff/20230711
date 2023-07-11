# Comparing `tmp/grokcore.traverser-3.0.1.tar.gz` & `tmp/grokcore.traverser-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grokcore.traverser-3.0.1.tar", last modified: Fri Jan 12 13:31:40 2018, max compression
+gzip compressed data, was "grokcore.traverser-4.0.tar", last modified: Tue Jul 11 06:30:22 2023, max compression
```

## Comparing `grokcore.traverser-3.0.1.tar` & `grokcore.traverser-4.0.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/
--rw-r--r--   0 jw         (501) staff       (20)      398 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/.travis.yml
--rw-r--r--   0 jw         (501) staff       (20)     6158 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/bootstrap.py
--rw-r--r--   0 jw         (501) staff       (20)      401 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/buildout.cfg
--rw-r--r--   0 jw         (501) staff       (20)      509 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/CHANGES.txt
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/COPYRIGHT.txt
--rw-r--r--   0 jw         (501) staff       (20)     2070 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/LICENSE.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/MANIFEST.in
--rw-r--r--   0 jw         (501) staff       (20)     1955 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      103 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/README.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/requirements.txt
--rw-r--r--   0 jw         (501) staff       (20)       38 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/setup.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2030 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/setup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/
--rw-r--r--   0 jw         (501) staff       (20)      200 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/
--rw-r--r--   0 jw         (501) staff       (20)     1067 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     4814 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/components.py
--rw-r--r--   0 jw         (501) staff       (20)      328 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/configure.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1660 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/directive.py
--rw-r--r--   0 jw         (501) staff       (20)      461 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/ftesting.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1460 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/interfaces.py
--rw-r--r--   0 jw         (501) staff       (20)     1972 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/meta.py
--rw-r--r--   0 jw         (501) staff       (20)      482 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/meta.zcml
--rw-r--r--   0 jw         (501) staff       (20)     2139 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/testing.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/
--rw-r--r--   0 jw         (501) staff       (20)      641 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/
--rw-r--r--   0 jw         (501) staff       (20)       20 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/
--rw-r--r--   0 jw         (501) staff       (20)       20 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     2436 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/containertraverse.py
--rw-r--r--   0 jw         (501) staff       (20)     2415 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/containertraverser.py
--rw-r--r--   0 jw         (501) staff       (20)     1794 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/items_before_views.py
--rw-r--r--   0 jw         (501) staff       (20)     1348 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/modeltraverse.py
--rw-r--r--   0 jw         (501) staff       (20)     1841 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traversableattr.py
--rw-r--r--   0 jw         (501) staff       (20)     1396 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser.py
--rw-r--r--   0 jw         (501) staff       (20)     1586 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser_sets_parent.py
--rw-r--r--   0 jw         (501) staff       (20)     1981 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser_with_layer.py
--rw-r--r--   0 jw         (501) staff       (20)     2343 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/tests/test_functional.py
--rw-r--r--   0 jw         (501) staff       (20)     1212 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore/traverser/util.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/namespace_packages.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/not-zip-safe
--rw-r--r--   0 jw         (501) staff       (20)     1955 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      268 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/requires.txt
--rw-r--r--   0 jw         (501) staff       (20)     1593 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:31:40.000000 grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/top_level.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.187407 grokcore.traverser-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      702 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1832 2023-07-11 06:30:22.187607 grokcore.traverser-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      103 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      485 2023-07-11 06:30:22.188424 grokcore.traverser-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2027 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.149812 grokcore.traverser-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.161617 grokcore.traverser-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.176323 grokcore.traverser-4.0/src/grokcore/traverser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1068 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4821 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/components.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      328 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1660 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/directive.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      461 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/ftesting.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1459 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1912 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/meta.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      482 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2140 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.178062 grokcore.traverser-4.0/src/grokcore/traverser/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      641 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.178924 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.186718 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2443 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/containertraverse.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2425 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/containertraverser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1801 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/items_before_views.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1393 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/modeltraverse.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1848 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traversableattr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1443 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1633 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser_sets_parent.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2042 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser_with_layer.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1996 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/tests/test_functional.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1212 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/src/grokcore/traverser/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:30:22.167723 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1832 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1572 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      281 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:30:22.000000 grokcore.traverser-4.0/src/grokcore.traverser.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1437 2023-07-11 06:30:21.000000 grokcore.traverser-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grokcore.traverser-3.0.1/LICENSE.txt` & `grokcore.traverser-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.traverser-3.0.1/PKG-INFO` & `grokcore.traverser-4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,75 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.traverser
-Version: 3.0.1
+Version: 4.0
 Summary: Traverser for the Grok Framework
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.traverser
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://cheeseshop.python.org/pypi/grok/
-Description: grokcore.traverser
-        ******************
-        
-        This package contains the default traversal mechanism for Grok.
-        
-        Changes
-        *******
-        
-        3.0.1 (2018-01-12)
-        ==================
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-05)
-        ==================
-        
-        - Python 3 compatibility
-        
-        1.2.1 (2016-02-15)
-        ==================
-        
-        - Update tests.
-        
-        1.2 (2012-11-14)
-        ================
-        
-        - Add the layer directive to Traverser Components.
-        
-        1.1 (2012-05-02)
-        ================
-        
-        - Use the component registration api of grokcore.component.
-        
-        1.0 (2011-01-03)
-        ================
-        
-        - Factor out form grok base package.
-        
-        Download
-        ********
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Framework :: Zope3
+Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+grokcore.traverser
+******************
+
+This package contains the default traversal mechanism for Grok.
+
+Changes
+*******
+
+4.0 (2023-07-11)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8, 3.9, and 3.10.
+
+- Drop support for Python 3.4.
+
+
+3.0.1 (2018-01-12)
+==================
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-05)
+==================
+
+- Python 3 compatibility
+
+1.2.1 (2016-02-15)
+==================
+
+- Update tests.
+
+1.2 (2012-11-14)
+================
+
+- Add the layer directive to Traverser Components.
+
+1.1 (2012-05-02)
+================
+
+- Use the component registration api of grokcore.component.
+
+1.0 (2011-01-03)
+================
+
+- Factor out form grok base package.
```

### Comparing `grokcore.traverser-3.0.1/setup.py` & `grokcore.traverser-4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
-    read('README.txt')
-    + '\n' +
-    read('CHANGES.txt')
+    read('README.rst')
     + '\n' +
-    'Download\n'
-    '********\n'
-    )
+    read('CHANGES.rst')
+)
 
 
 tests_require = [
     'grokcore.content',
-    'grokcore.view[security_publication]',
-    'grokcore.view[test]',
+    'grokcore.view [test]',
     'zope.app.appsetup',
     'zope.app.wsgi',
+    'zope.login',
+    'zope.principalregistry',
+    'zope.securitypolicy',
     'zope.testbrowser',
     'zope.testing',
-    ]
+]
 
 
 setup(
     name='grokcore.traverser',
-    version='3.0.1',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://cheeseshop.python.org/pypi/grok/',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.traverser',
     description='Traverser for the Grok Framework',
     long_description=long_description,
     license='ZPL',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
-        'Framework :: Zope3',
-        ],
+        'Framework :: Zope :: 3',
+    ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
-        'grokcore.component >= 2.5dev',
+        'grokcore.component >= 2.5',
         'grokcore.security',
         'grokcore.view',
         'martian',
         'setuptools',
         'zope.component',
         'zope.interface',
         'zope.publisher',
-        ],
+    ],
     tests_require=tests_require,
     extras_require={'test': tests_require},
 )
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/__init__.py` & `grokcore.traverser-4.0/src/grokcore/traverser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 #
 ##############################################################################
 """Grok
 """
 from grokcore.component import *
 from grokcore.security import *
 from grokcore.view import *
+from zope.interface import moduleProvides
 
-from grokcore.traverser.directive import traversable
 from grokcore.traverser.components import Traverser
-
+from grokcore.traverser.directive import traversable
 from grokcore.traverser.interfaces import IGrokTraverser
 from grokcore.traverser.interfaces import IRESTLayer
-from zope.interface import moduleProvides
+
+
 moduleProvides(IGrokTraverser)
 __all__ = list(IGrokTraverser)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/components.py` & `grokcore.traverser-4.0/src/grokcore/traverser/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 
 When an application developer builds a Grok-based application, the
 classes they define each typically inherit from one of the base classes
 provided here.
 """
 
 import zope.interface
-
 from grokcore.component.interfaces import IContext
-from grokcore.traverser import traversable
-from grokcore.traverser.interfaces import IRESTLayer
-from grokcore.traverser.util import safely_locate_maybe
 from zope import component
 from zope.container.interfaces import IContainer
 from zope.container.interfaces import IReadContainer
 from zope.publisher.defaultview import getDefaultViewName
 from zope.publisher.interfaces import NotFound
 from zope.publisher.interfaces.browser import IBrowserPublisher
 from zope.publisher.interfaces.http import IHTTPRequest
 
+import grokcore.traverser
+from grokcore.traverser.interfaces import IRESTLayer
+from grokcore.traverser.util import safely_locate_maybe
+
 
 @zope.interface.implementer(IBrowserPublisher)
-class Traverser(object):
+class Traverser:
     """Base class for traversers in Grok applications."""
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def browserDefault(self, request):
@@ -54,15 +54,16 @@
         return self.context, (view_uri,)
 
     def publishTraverse(self, request, name):
         subob = self.traverse(name)
         if subob is not None:
             return safely_locate_maybe(subob, self.context, name)
 
-        traversable_dict = traversable.bind().get(self.context)
+        traversable_dict = grokcore.traverser.traversable.bind().get(
+            self.context)
         if traversable_dict:
             if name in traversable_dict:
                 subob = getattr(self.context, traversable_dict[name])
                 if callable(subob):
                     subob = subob()
                 return safely_locate_maybe(subob, self.context, name)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/directive.py` & `grokcore.traverser-4.0/src/grokcore/traverser/directive.py`

 * *Files identical despite different names*

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/interfaces.py` & `grokcore.traverser-4.0/src/grokcore/traverser/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 ##############################################################################
 """Grok interfaces
 """
 import grokcore.component.interfaces
 import grokcore.security.interfaces
 import grokcore.view.interfaces
-
 from zope import interface
 from zope.publisher.interfaces.http import IHTTPRequest
 
 
 class IBaseClasses(
         grokcore.component.interfaces.IBaseClasses,
         grokcore.security.interfaces.IBaseClasses,
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/meta.py` & `grokcore.traverser-4.0/src/grokcore/traverser/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 file directs the `martian` library to scan this file, where it discovers
 and registers the grokkers you see below.  The grokkers are then active
 and available as `martian` recursively examines the packages and modules
 of a Grok-based web application.
 
 """
 
-import martian
-import grokcore.view
-import grokcore.traverser
 import grokcore.component
-
-from zope.publisher.interfaces.http import IHTTPRequest
+import grokcore.view
+import martian
 from zope.publisher.interfaces.browser import IBrowserPublisher
 from zope.publisher.interfaces.browser import IDefaultBrowserLayer
 
+import grokcore.traverser
+
 
 class TraverserGrokker(martian.ClassGrokker):
     """Grokker for subclasses of `grok.Traverser`."""
     martian.component(grokcore.traverser.Traverser)
     martian.directive(grokcore.component.context)
     martian.directive(grokcore.view.layer, default=IDefaultBrowserLayer)
 
     def execute(self, factory, config, context, layer, **kw):
         adapts = (context, layer)
         config.action(
             discriminator=('adapter', adapts, IBrowserPublisher, ''),
             callable=grokcore.component.provideAdapter,
             args=(factory, adapts, IBrowserPublisher),
-            )
+        )
         return True
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/testing.py` & `grokcore.traverser-4.0/src/grokcore/traverser/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok test helpers
 """
 import sys
-from zope.configuration.config import ConfigurationMachine
+
 from grokcore.component import zcml
+from zope.configuration.config import ConfigurationMachine
 
 
 def grok(module_name):
     config = ConfigurationMachine()
     zcml.do_grok('grokcore.component.meta', config)
     zcml.do_grok('grokcore.security.meta', config)
     zcml.do_grok('grokcore.view.meta', config)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/__init__.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/containertraverse.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/containertraverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,52 +54,59 @@
   >>> herd['subherd'] = Herd()
   >>> browser.open("http://localhost/herd/subherd")
   >>> print(browser.contents)
   A herd
 
 """
 import grokcore.component as grok
-import grokcore.view as view
 import grokcore.content as content
+import grokcore.view as view
 
 
 class Herd(content.Container):
 
     def traverse(self, name):
         if name == 'special':
             return Special()
         return None
 
+
 class HerdIndex(view.View):
     grok.context(Herd)
     grok.name('index')
 
     def render(self):
         return 'A herd'
 
+
 class Mammoth(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 class Special(content.Model):
     pass
 
+
 class SpecialIndex(view.View):
     grok.context(Special)
     grok.name('index')
 
     def render(self):
         return "special view"
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/containertraverser.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/containertraverser.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,47 +54,57 @@
   >>> herd['subherd'] = Herd()
   >>> browser.open("http://localhost/herd/subherd/special")
   >>> print(browser.contents)
   special view
 
 """
 import grokcore.component as grok
-import grokcore.traverser
 import grokcore.content as content
 import grokcore.view as view
 
+import grokcore.traverser
+
+
 class Herd(content.Container):
     pass
 
+
 class Traverser(grokcore.traverser.Traverser):
     grok.context(Herd)
+
     def traverse(self, name):
         if name == 'special':
             return Special()
         return None
 
+
 class Mammoth(content.Model):
     def __init__(self, name):
         self.name = name
 
+
 class Special(content.Model):
     pass
 
+
 class SpecialIndex(view.View):
     grok.context(Special)
     grok.name('index')
 
     def render(self):
         return "special view"
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/items_before_views.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/items_before_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Containers can have an explicit traverser associated with them.  The
 behaviour falls back to basic container traversal if the 'traverse'
 method returns None. Normal behaviour also means that the standard
-Zope 3 paradigm"items before views" is supported in the fallback.
+Zope 3 paradigm "items before views" is supported in the fallback.
 
   >>> getRootFolder()["herd"] = herd = Herd()
   >>> herd['manfred'] = Mammoth('Manfred')
   >>> herd['ellie'] = Mammoth('Ellie')
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
@@ -31,37 +31,43 @@
   >>> print(browser.contents)
   Hi, it's me, the Ellie view!
 
 """
 import grokcore.component as grok
 import grokcore.content as content
 import grokcore.view as view
+
 import grokcore.traverser
 
+
 class Herd(content.Container):
     pass
 
+
 class Traverser(grokcore.traverser.Traverser):
     grok.context(Herd)
 
     def traverse(self, name):
         # we don't really need to do anything here as we want to test
         # the fallback behaviour
         pass
 
+
 class Ellie(view.View):
     grok.context(Herd)
     grok.name('ellie')
 
     def render(self):
         return "Hi, it's me, the Ellie view!"
 
+
 class Mammoth(content.Model):
     def __init__(self, name):
         self.name = name
 
+
 class MammothIndex(view.View):
     grok.context(Mammoth)
     grok.name('index')
 
     def render(self):
         return "Hello " + self.context.name.title()
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/modeltraverse.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 """
-Models can determine how they want to be traversed by
-implementing a 'traverse' method:
+Apart from using the ``traverse`` method on a model, you can
+also create a separate traverser component:
 
   >>> getRootFolder()["herd"] = Herd('The Big Mammoth Herd')
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
   >>> browser.handleErrors = False
   >>> browser.open("http://localhost/herd/manfred")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Manfred!</h1>
-  <p>Manfred is part of The Big Mammoth Herd.</p>
+  <p>
+    Manfred
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
   >>> browser.open("http://localhost/herd/ellie")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Ellie!</h1>
-  <p>Ellie is part of The Big Mammoth Herd.</p>
+  <p>
+    Ellie
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
 """
 import grokcore.component as grok
 import grokcore.content as content
 import grokcore.view as view
 
+import grokcore.traverser
+
+
 class Herd(content.Model):
 
     def __init__(self, name):
         self.name = name
 
-    def getMammoth(self, name):
-        return Mammoth(name)
+
+class HerdTraverser(grokcore.traverser.Traverser):
+    grok.context(Herd)
 
     def traverse(self, name):
-        return self.getMammoth(name)
+        return Mammoth(name)
+
 
 class Mammoth(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
-<p><span tal:replace="context/name/title" /> is part of <span tal:replace="context/__parent__/name" />.</p>
+<p>
+  <span tal:replace="context/name/title" />
+  is part of
+  <span tal:replace="context/__parent__/name" />.
+</p>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traversableattr.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traversableattr.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,38 +33,45 @@
   ...
   zope.publisher.interfaces.NotFound: ...
 
 """
 import grokcore.component as grok
 import grokcore.content as content
 import grokcore.view as view
+
 import grokcore.traverser
 
+
 class Bar(content.Model):
     def __init__(self, name):
         self.name = name
 
+
 class BarIndex(view.View):
     grok.context(Bar)
     grok.name('index')
 
     def render(self):
         return self.context.name
 
+
 class Foo(content.Model):
     grokcore.traverser.traversable('bar')
     grokcore.traverser.traversable('foo')
     grokcore.traverser.traversable(attr='bar', name='namedbar')
 
     def __init__(self, name):
         self.name = name
 
     foo = Bar('foo')
+
     def bar(self):
         return Bar('bar')
     z = "i'm not called"
 
+
 class FooIndex(view.View):
     grok.context(Foo)
     grok.name('index')
+
     def render(self):
         return self.context.name
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser_sets_parent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 """
-Apart from using the ``traverse`` method on a model, you can
-also create a separate traverser component:
+A traverser can set the __parent__ (and __name__) attributes itself,
+in which case Grok's traverser won't interfere:
 
   >>> getRootFolder()["herd"] = Herd('The Big Mammoth Herd')
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
   >>> browser.handleErrors = False
   >>> browser.open("http://localhost/herd/manfred")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Manfred!</h1>
-  <p>Manfred is part of The Big Mammoth Herd.</p>
+  <p>
+    Manfred
+    is part of
+    The Three Stooges.
+  </p>
   </body>
   </html>
 
   >>> browser.open("http://localhost/herd/ellie")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Ellie!</h1>
-  <p>Ellie is part of The Big Mammoth Herd.</p>
+  <p>
+    Ellie
+    is part of
+    The Three Stooges.
+  </p>
   </body>
   </html>
 
 """
 import grokcore.component as grok
 import grokcore.content as content
-import grokcore.traverser
 import grokcore.view as view
 
+import grokcore.traverser
+
+
 class Herd(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 class HerdTraverser(grokcore.traverser.Traverser):
     grok.context(Herd)
 
     def traverse(self, name):
-        return Mammoth(name)
+        mammoth = Mammoth(name)
+        # We pretend the mammoth is the child object of some competely
+        # differnt Herd object.
+        mammoth.__parent__ = Herd('The Three Stooges')
+        return mammoth
+
 
 class Mammoth(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
-<p><span tal:replace="context/name/title" /> is part of <span tal:replace="context/__parent__/name" />.</p>
+<p>
+  <span tal:replace="context/name/title" />
+  is part of
+  <span tal:replace="context/__parent__/name" />.
+</p>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser_sets_parent.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/traverser_with_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,111 @@
 """
-A traverser can set the __parent__ (and __name__) attributes itself,
-in which case Grok's traverser won't interfere:
+Apart from using the ``traverse`` method on a model, you can
+also create a separate traverser component:
 
   >>> getRootFolder()["herd"] = Herd('The Big Mammoth Herd')
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
   >>> browser.handleErrors = False
   >>> browser.open("http://localhost/herd/manfred")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Manfred!</h1>
-  <p>Manfred is part of The Three Stooges.</p>
+  <p>
+    Manfred
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
   >>> browser.open("http://localhost/herd/ellie")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Ellie!</h1>
-  <p>Ellie is part of The Three Stooges.</p>
+  <p>
+    Ellie
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
+Now let's call the same URI on a different Layer.
+
+  >>> browser.open("http://localhost/++skin++elephant/herd/ellie")
+  >>> print(browser.contents)
+  <html>
+  <body>
+  <h1>Hello, Ellie Elephant!</h1>
+  <p>
+    Ellie Elephant
+    is part of
+    The Big Mammoth Herd.
+  </p>
+  </body>
+  </html>
 """
 import grokcore.component as grok
 import grokcore.content as content
-import grokcore.traverser
 import grokcore.view as view
 
+import grokcore.traverser
+
+
+class ElephantLayer(view.IDefaultBrowserLayer):
+    pass
+
+
+class ElephantSkin(ElephantLayer):
+    view.skin('elephant')
+
+
 class Herd(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 class HerdTraverser(grokcore.traverser.Traverser):
     grok.context(Herd)
 
     def traverse(self, name):
-        mammoth = Mammoth(name)
-        # We pretend the mammoth is the child object of some competely
-        # differnt Herd object.
-        mammoth.__parent__ = Herd('The Three Stooges')
-        return mammoth
+        return Mammoth(name)
+
+
+class ElephantTraverser(grokcore.traverser.Traverser):
+    grok.context(Herd)
+    view.layer(ElephantLayer)
+
+    def traverse(self, name):
+        return Mammoth(name + ' Elephant')
+
 
 class Mammoth(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
-<p><span tal:replace="context/name/title" /> is part of <span tal:replace="context/__parent__/name" />.</p>
+<p>
+  <span tal:replace="context/name/title" />
+  is part of
+  <span tal:replace="context/__parent__/name" />.
+</p>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/functional/traversal/traverser_with_layer.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/functional/traversal/modeltraverse.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,78 @@
 """
-Apart from using the ``traverse`` method on a model, you can
-also create a separate traverser component:
+Models can determine how they want to be traversed by
+implementing a 'traverse' method:
 
   >>> getRootFolder()["herd"] = Herd('The Big Mammoth Herd')
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
   >>> browser.handleErrors = False
   >>> browser.open("http://localhost/herd/manfred")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Manfred!</h1>
-  <p>Manfred is part of The Big Mammoth Herd.</p>
+  <p>
+    Manfred
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
   >>> browser.open("http://localhost/herd/ellie")
   >>> print(browser.contents)
   <html>
   <body>
   <h1>Hello, Ellie!</h1>
-  <p>Ellie is part of The Big Mammoth Herd.</p>
+  <p>
+    Ellie
+    is part of
+    The Big Mammoth Herd.
+  </p>
   </body>
   </html>
 
-Now let's call the same URI on a different Layer.
-
-  >>> browser.open("http://localhost/++skin++elephant/herd/ellie")
-  >>> print(browser.contents)
-  <html>
-  <body>
-  <h1>Hello, Ellie Elephant!</h1>
-  <p>Ellie Elephant is part of The Big Mammoth Herd.</p>
-  </body>
-  </html>
 """
 import grokcore.component as grok
 import grokcore.content as content
-import grokcore.traverser
 import grokcore.view as view
 
 
-class ElephantLayer(view.IDefaultBrowserLayer):
-    pass
-
-class ElephantSkin(ElephantLayer):
-    view.skin('elephant')
-
-
 class Herd(content.Model):
 
     def __init__(self, name):
         self.name = name
 
-
-class HerdTraverser(grokcore.traverser.Traverser):
-    grok.context(Herd)
-
-    def traverse(self, name):
+    def getMammoth(self, name):
         return Mammoth(name)
 
-
-class ElephantTraverser(grokcore.traverser.Traverser):
-    grok.context(Herd)
-    view.layer(ElephantLayer)
-
     def traverse(self, name):
-        return Mammoth(name + ' Elephant')
+        return self.getMammoth(name)
 
 
 class Mammoth(content.Model):
 
     def __init__(self, name):
         self.name = name
 
+
 grok.context(Mammoth)
 
+
 class Index(view.View):
     pass
 
+
 index = view.PageTemplate("""\
 <html>
 <body>
 <h1>Hello, <span tal:replace="context/name/title" />!</h1>
-<p><span tal:replace="context/name/title" /> is part of <span tal:replace="context/__parent__/name" />.</p>
+<p>
+  <span tal:replace="context/name/title" />
+  is part of
+  <span tal:replace="context/__parent__/name" />.
+</p>
 </body>
 </html>
 """)
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/tests/test_functional.py` & `grokcore.traverser-4.0/src/grokcore/traverser/tests/test_functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,72 @@
 import doctest
-import re
 import unittest
-import grokcore.traverser
 
 from pkg_resources import resource_listdir
-from zope.testing import renormalizing
-from zope.app.wsgi.testlayer import http
+
 import zope.testbrowser.wsgi
+from zope.app.wsgi.testlayer import http
+
+import grokcore.traverser
 
 
 class Layer(
         zope.testbrowser.wsgi.TestBrowserLayer,
         zope.app.wsgi.testlayer.BrowserLayer):
     pass
 
-layer = Layer(grokcore.traverser)
 
-checker = renormalizing.RENormalizing([
-    # Accommodate to exception wrapping in newer versions of mechanize
-    (re.compile(r'httperror_seek_wrapper:', re.M), 'HTTPError:'),
-    ])
+layer = Layer(grokcore.traverser)
 
 
 def http_call(method, path, data=None, **kw):
     """Function to help make RESTful calls.
 
     method - HTTP method to use
     path - testbrowser style path
     data - (body) data to submit
     kw - any request parameters
     """
 
     if path.startswith('http://localhost'):
         path = path[len('http://localhost'):]
-    request_string = '%s %s HTTP/1.1\n' % (method, path)
+    request_string = '{} {} HTTP/1.1\n'.format(method, path)
     for key, value in kw.items():
-        request_string += '%s: %s\n' % (key, value)
+        request_string += '{}: {}\n'.format(key, value)
     if data is not None:
         request_string += '\r\n'
         request_string += data
     return http(request_string, handle_errors=False)
 
 
 def suiteFromPackage(name):
     layer_dir = 'functional'
-    files = resource_listdir(__name__, '{}/{}'.format(layer_dir, name))
+    files = resource_listdir(__name__, f'{layer_dir}/{name}')
     suite = unittest.TestSuite()
     for filename in files:
         if not filename.endswith('.py'):
             continue
         if filename == '__init__.py':
             continue
 
-        dottedname = 'grokcore.traverser.tests.%s.%s.%s' % (
+        dottedname = 'grokcore.traverser.tests.{}.{}.{}'.format(
             layer_dir, name, filename[:-3])
         test = doctest.DocTestSuite(
             dottedname,
-            checker=checker,
             extraglobs=dict(http_call=http_call,
                             http=http,
                             getRootFolder=layer.getRootFolder),
-            optionflags=(renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2 +
-                         doctest.ELLIPSIS +
+            optionflags=(doctest.ELLIPSIS +
                          doctest.NORMALIZE_WHITESPACE +
-                         doctest.REPORT_NDIFF))
+                         doctest.REPORT_NDIFF +
+                         doctest.IGNORE_EXCEPTION_DETAIL))
         test.layer = layer
 
         suite.addTest(test)
     return suite
 
 
 def test_suite():
     suite = unittest.TestSuite()
     for name in ['traversal']:
         suite.addTest(suiteFromPackage(name))
     return suite
-
-if __name__ == '__main__':
-    unittest.main(defaultTest='test_suite')
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore/traverser/util.py` & `grokcore.traverser-4.0/src/grokcore/traverser/util.py`

 * *Files identical despite different names*

### Comparing `grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/PKG-INFO` & `grokcore.traverser-4.0/src/grokcore.traverser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,75 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.traverser
-Version: 3.0.1
+Version: 4.0
 Summary: Traverser for the Grok Framework
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.traverser
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://cheeseshop.python.org/pypi/grok/
-Description: grokcore.traverser
-        ******************
-        
-        This package contains the default traversal mechanism for Grok.
-        
-        Changes
-        *******
-        
-        3.0.1 (2018-01-12)
-        ==================
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-05)
-        ==================
-        
-        - Python 3 compatibility
-        
-        1.2.1 (2016-02-15)
-        ==================
-        
-        - Update tests.
-        
-        1.2 (2012-11-14)
-        ================
-        
-        - Add the layer directive to Traverser Components.
-        
-        1.1 (2012-05-02)
-        ================
-        
-        - Use the component registration api of grokcore.component.
-        
-        1.0 (2011-01-03)
-        ================
-        
-        - Factor out form grok base package.
-        
-        Download
-        ********
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Framework :: Zope3
+Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+grokcore.traverser
+******************
+
+This package contains the default traversal mechanism for Grok.
+
+Changes
+*******
+
+4.0 (2023-07-11)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8, 3.9, and 3.10.
+
+- Drop support for Python 3.4.
+
+
+3.0.1 (2018-01-12)
+==================
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-05)
+==================
+
+- Python 3 compatibility
+
+1.2.1 (2016-02-15)
+==================
+
+- Update tests.
+
+1.2 (2012-11-14)
+================
+
+- Add the layer directive to Traverser Components.
+
+1.1 (2012-05-02)
+================
+
+- Use the component registration api of grokcore.component.
+
+1.0 (2011-01-03)
+================
+
+- Factor out form grok base package.
```

### Comparing `grokcore.traverser-3.0.1/src/grokcore.traverser.egg-info/SOURCES.txt` & `grokcore.traverser-4.0/src/grokcore.traverser.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-.travis.yml
-CHANGES.txt
+CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
-README.txt
-bootstrap.py
-buildout.cfg
-requirements.txt
+README.rst
+setup.cfg
 setup.py
+tox.ini
 src/grokcore/__init__.py
 src/grokcore.traverser.egg-info/PKG-INFO
 src/grokcore.traverser.egg-info/SOURCES.txt
 src/grokcore.traverser.egg-info/dependency_links.txt
 src/grokcore.traverser.egg-info/namespace_packages.txt
 src/grokcore.traverser.egg-info/not-zip-safe
 src/grokcore.traverser.egg-info/requires.txt
```

