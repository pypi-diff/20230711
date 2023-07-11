# Comparing `tmp/feaASTools-0.0.0.tar.gz` & `tmp/feaASTools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feaASTools-0.0.0.tar", last modified: Mon Jul 10 16:44:20 2023, max compression
+gzip compressed data, was "feaASTools-0.2.2.tar", last modified: Tue Jul 11 12:31:51 2023, max compression
```

## Comparing `feaASTools-0.0.0.tar` & `feaASTools-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:44:20.608934 feaASTools-0.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-10 16:44:19.000000 feaASTools-0.0.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:44:20.606934 feaASTools-0.0.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:44:20.607935 feaASTools-0.0.0/Lib/feaASTools/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-10 16:44:19.000000 feaASTools-0.0.0/Lib/feaASTools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-10 16:44:19.000000 feaASTools-0.0.0/Lib/feaASTools/inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     9052 2023-07-10 16:44:19.000000 feaASTools-0.0.0/Lib/feaASTools/renameGlyph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:44:20.608934 feaASTools-0.0.0/Lib/feaASTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      988 2023-07-10 16:44:20.000000 feaASTools-0.0.0/Lib/feaASTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 16:44:20.000000 feaASTools-0.0.0/Lib/feaASTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:44:20.000000 feaASTools-0.0.0/Lib/feaASTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 16:44:20.000000 feaASTools-0.0.0/Lib/feaASTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 16:44:20.000000 feaASTools-0.0.0/Lib/feaASTools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      988 2023-07-10 16:44:20.608934 feaASTools-0.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-10 16:44:19.000000 feaASTools-0.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-07-10 16:44:20.609934 feaASTools-0.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-10 16:44:19.000000 feaASTools-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.963677 feaASTools-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-11 12:31:50.000000 feaASTools-0.2.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.961677 feaASTools-0.2.2/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.962677 feaASTools-0.2.2/Lib/feaASTools/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     9383 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/renameGlyph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.962677 feaASTools-0.2.2/Lib/feaASTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 12:31:51.963677 feaASTools-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-11 12:31:50.000000 feaASTools-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-07-11 12:31:51.963677 feaASTools-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-11 12:31:50.000000 feaASTools-0.2.2/setup.py
```

### Comparing `feaASTools-0.0.0/LICENSE` & `feaASTools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feaASTools-0.0.0/Lib/feaASTools/renameGlyph.py` & `feaASTools-0.2.2/Lib/feaASTools/renameGlyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 renameGlyph
 ===============================================================================
 
 Rename glyph in feature files.
 
+To make it simple we inject a renameGlyph method in every `ast.Statement` class 
+which deserves one.
+As a result we can simply call `syntaxTree.renameGlyph(oldName, newName)`.
+
 """
 from __future__ import annotations
 
 import logging
 from typing import List, Tuple, Union
 
 import fontTools.feaLib.ast as ast
@@ -257,10 +261,15 @@
                 "unhandled statement type: %r on line %r",
                 statement.__class__.__name__,
                 statement.location[1],
             )
 
 
 def renameGlyphInFeatureText(featureText: str, oldName: str, newName: str):
+    """
+    :param featureText: The feature text to inspect
+    :param oldName: Glyph name to find
+    :param newName: Glyph name to replace with
+    """
     syntaxTree = getFeatureSyntaxTree(featureText)
     syntaxTree.renameGlyph(oldName, newName)
     return syntaxTree.asFea()
```

### Comparing `feaASTools-0.0.0/Lib/feaASTools.egg-info/PKG-INFO` & `feaASTools-0.2.2/Lib/feaASTools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: feaASTools
-Version: 0.0.0
+Version: 0.2.2
 Summary: Tools to handle feature files (*.fea) as abstract syntax tree.
 Home-page: https://gitlab.com/fontstuff/feaASTools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/feaASTools
+Project-URL: Documentation, https://fontstuff.gitlab.io/feaASTools
+Project-URL: Tracker, https://gitlab.com/fontstuff/feaASTools/-/issues
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `feaASTools-0.0.0/PKG-INFO` & `feaASTools-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: feaASTools
-Version: 0.0.0
+Version: 0.2.2
 Summary: Tools to handle feature files (*.fea) as abstract syntax tree.
 Home-page: https://gitlab.com/fontstuff/feaASTools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/feaASTools
+Project-URL: Documentation, https://fontstuff.gitlab.io/feaASTools
+Project-URL: Tracker, https://gitlab.com/fontstuff/feaASTools/-/issues
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `feaASTools-0.0.0/setup.cfg` & `feaASTools-0.2.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.2.2
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
+[bumpversion:file:Lib/feaASTools/__init__.py]
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
+
 [metadata]
 name = feaASTools
+version = attr: feaASTools.__version__
 author = Andreas Eigendorf
 description = Tools to handle feature files (*.fea) as abstract syntax tree.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/fontstuff/feaASTools
 project_urls = 
 	Source = https://gitlab.com/fontstuff/feaASTools
+	Documentation = https://fontstuff.gitlab.io/feaASTools
+	Tracker = https://gitlab.com/fontstuff/feaASTools/-/issues
 platforms = Any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -39,18 +46,14 @@
 python_requires = >=3.8
 install_requires = 
 	fonttools>=4.40.0
 
 [options.packages.find]
 where = Lib
 
-[bumpversion:file:Lib/feaASTools/__init__.py]
-search = __version__ = "{current_version}"
-replace = __version__ = "{new_version}"
-
 [tox:tox]
 min_version = 4.6
 env_list = 
 	py38
 	py39
 	py310
 	py311
```

