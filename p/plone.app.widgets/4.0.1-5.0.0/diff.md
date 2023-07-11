# Comparing `tmp/plone.app.widgets-4.0.1.tar.gz` & `tmp/plone.app.widgets-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.widgets-4.0.1.tar", last modified: Wed Feb 22 17:40:05 2023, max compression
+gzip compressed data, was "plone.app.widgets-5.0.0.tar", last modified: Tue Jul 11 10:24:31 2023, max compression
```

## Comparing `plone.app.widgets-4.0.1.tar` & `plone.app.widgets-5.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.614556 plone.app.widgets-4.0.1/
--rw-r--r--   0 gil       (1000) gil       (1000)    13642 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    17987 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      733 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/LICENSE.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      184 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    18009 2023-02-22 17:40:05.614556 plone.app.widgets-4.0.1/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     3514 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.610556 plone.app.widgets-4.0.1/docs/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.611556 plone.app.widgets-4.0.1/docs/source/
--rw-r--r--   0 gil       (1000) gil       (1000)      473 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/docs/source/index.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     6170 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/docs/source/select_widget.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.611556 plone.app.widgets-4.0.1/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)      244 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.612556 plone.app.widgets-4.0.1/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)      244 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.613556 plone.app.widgets-4.0.1/plone/app/widgets/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)    10483 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/base.py
--rw-r--r--   0 gil       (1000) gil       (1000)      233 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      309 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/factories.py
--rw-r--r--   0 gil       (1000) gil       (1000)      513 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4747 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.613556 plone.app.widgets-4.0.1/plone/app/widgets/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      262 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/configure.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.614556 plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1512 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/common.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     6874 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/test_querystring_widget.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     4191 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/test_select_widget.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     9626 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/test_base.py
--rw-r--r--   0 gil       (1000) gil       (1000)      874 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/test_robot.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8985 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/tests/test_utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8828 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/plone/app/widgets/utils.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:40:05.612556 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    18009 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     1091 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      214 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-02-22 17:40:05.000000 plone.app.widgets-4.0.1/plone.app.widgets.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      397 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      251 2023-02-22 17:40:05.614556 plone.app.widgets-4.0.1/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     1658 2023-02-22 17:40:04.000000 plone.app.widgets-4.0.1/setup.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.733137 plone.app.widgets-5.0.0/
+-rw-r--r--   0 thet      (1000) thet      (1000)    13931 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/CHANGES.rst
+-rw-r--r--   0 thet      (1000) thet      (1000)       70 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 thet      (1000) thet      (1000)    17987 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/LICENSE.GPL
+-rw-r--r--   0 thet      (1000) thet      (1000)      733 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/LICENSE.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)      184 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/MANIFEST.in
+-rw-r--r--   0 thet      (1000) thet      (1000)    18298 2023-07-11 10:24:31.733137 plone.app.widgets-5.0.0/PKG-INFO
+-rw-r--r--   0 thet      (1000) thet      (1000)     3514 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/README.rst
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.725137 plone.app.widgets-5.0.0/docs/
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.729137 plone.app.widgets-5.0.0/docs/source/
+-rw-r--r--   0 thet      (1000) thet      (1000)      473 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/docs/source/index.rst
+-rw-r--r--   0 thet      (1000) thet      (1000)     6170 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/docs/source/select_widget.rst
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.729137 plone.app.widgets-5.0.0/plone/
+-rw-r--r--   0 thet      (1000) thet      (1000)      244 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/__init__.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.729137 plone.app.widgets-5.0.0/plone/app/
+-rw-r--r--   0 thet      (1000) thet      (1000)      244 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/__init__.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.729137 plone.app.widgets-5.0.0/plone/app/widgets/
+-rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/__init__.py
+-rw-r--r--   0 thet      (1000) thet      (1000)      692 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/base.py
+-rw-r--r--   0 thet      (1000) thet      (1000)      233 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/configure.zcml
+-rw-r--r--   0 thet      (1000) thet      (1000)      309 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/factories.py
+-rw-r--r--   0 thet      (1000) thet      (1000)      513 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/interfaces.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     4747 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/testing.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.733137 plone.app.widgets-5.0.0/plone/app/widgets/tests/
+-rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/__init__.py
+-rw-r--r--   0 thet      (1000) thet      (1000)      262 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/configure.zcml
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.733137 plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/
+-rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/__init__.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     1512 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/common.robot
+-rw-r--r--   0 thet      (1000) thet      (1000)     6874 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/test_querystring_widget.robot
+-rw-r--r--   0 thet      (1000) thet      (1000)     4191 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/test_select_widget.robot
+-rw-r--r--   0 thet      (1000) thet      (1000)     9626 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/test_base.py
+-rw-r--r--   0 thet      (1000) thet      (1000)      874 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/test_robot.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     8985 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/tests/test_utils.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     1615 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone/app/widgets/utils.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-07-11 10:24:31.729137 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/
+-rw-r--r--   0 thet      (1000) thet      (1000)    18298 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/PKG-INFO
+-rw-r--r--   0 thet      (1000) thet      (1000)     1091 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)       16 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/namespace_packages.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/not-zip-safe
+-rw-r--r--   0 thet      (1000) thet      (1000)      214 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/requires.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)        6 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/plone.app.widgets.egg-info/top_level.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)      397 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/pyproject.toml
+-rw-r--r--   0 thet      (1000) thet      (1000)      251 2023-07-11 10:24:31.733137 plone.app.widgets-5.0.0/setup.cfg
+-rw-r--r--   0 thet      (1000) thet      (1000)     1658 2023-07-11 10:24:31.000000 plone.app.widgets-5.0.0/setup.py
```

### Comparing `plone.app.widgets-4.0.1/CHANGES.rst` & `plone.app.widgets-5.0.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.0 (2023-07-11)
+------------------
+
+Breaking changes:
+
+
+- Make this package deprecated. Widget base classes moved to ``plone.app.z3cform.widgets.patterns``.
+  Also see ``plone.app.widgets.utils`` for information about moving utility methods to their new location.
+  [petschki] (#220)
+
+
 4.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Depend on plone.base (#222)
```

### Comparing `plone.app.widgets-4.0.1/LICENSE.GPL` & `plone.app.widgets-5.0.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/LICENSE.txt` & `plone.app.widgets-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/PKG-INFO` & `plone.app.widgets-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.widgets
-Version: 4.0.1
+Version: 5.0.0
 Summary: better plone widgets
 Home-page: https://github.com/plone/plone.app.widgets
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: GPL
 Keywords: plone widgets z3cform
 Classifier: Development Status :: 5 - Production/Stable
@@ -122,14 +122,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.0 (2023-07-11)
+------------------
+
+Breaking changes:
+
+
+- Make this package deprecated. Widget base classes moved to ``plone.app.z3cform.widgets.patterns``.
+  Also see ``plone.app.widgets.utils`` for information about moving utility methods to their new location.
+  [petschki] (#220)
+
+
 4.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Depend on plone.base (#222)
```

### Comparing `plone.app.widgets-4.0.1/README.rst` & `plone.app.widgets-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/docs/source/select_widget.rst` & `plone.app.widgets-5.0.0/docs/source/select_widget.rst`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/interfaces.py` & `plone.app.widgets-5.0.0/plone/app/widgets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/testing.py` & `plone.app.widgets-5.0.0/plone/app/widgets/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/common.robot` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/common.robot`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/test_querystring_widget.robot` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/test_querystring_widget.robot`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/robot/test_select_widget.robot` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/robot/test_select_widget.robot`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/test_base.py` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/test_robot.py` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone/app/widgets/tests/test_utils.py` & `plone.app.widgets-5.0.0/plone/app/widgets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/plone.app.widgets.egg-info/PKG-INFO` & `plone.app.widgets-5.0.0/plone.app.widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.widgets
-Version: 4.0.1
+Version: 5.0.0
 Summary: better plone widgets
 Home-page: https://github.com/plone/plone.app.widgets
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: GPL
 Keywords: plone widgets z3cform
 Classifier: Development Status :: 5 - Production/Stable
@@ -122,14 +122,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.0 (2023-07-11)
+------------------
+
+Breaking changes:
+
+
+- Make this package deprecated. Widget base classes moved to ``plone.app.z3cform.widgets.patterns``.
+  Also see ``plone.app.widgets.utils`` for information about moving utility methods to their new location.
+  [petschki] (#220)
+
+
 4.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Depend on plone.base (#222)
```

### Comparing `plone.app.widgets-4.0.1/plone.app.widgets.egg-info/SOURCES.txt` & `plone.app.widgets-5.0.0/plone.app.widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.widgets-4.0.1/setup.py` & `plone.app.widgets-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '4.0.1'
+version = '5.0.0'
 
 setup(
     name='plone.app.widgets',
     version=version,
     description="better plone widgets",
     long_description='%s\n%s' % (
         open("README.rst").read(),
```

