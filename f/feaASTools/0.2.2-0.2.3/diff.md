# Comparing `tmp/feaASTools-0.2.2.tar.gz` & `tmp/feaASTools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feaASTools-0.2.2.tar", last modified: Tue Jul 11 12:31:51 2023, max compression
+gzip compressed data, was "feaASTools-0.2.3.tar", last modified: Tue Jul 11 21:49:51 2023, max compression
```

## Comparing `feaASTools-0.2.2.tar` & `feaASTools-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.963677 feaASTools-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-11 12:31:50.000000 feaASTools-0.2.2/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.961677 feaASTools-0.2.2/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.962677 feaASTools-0.2.2/Lib/feaASTools/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     9383 2023-07-11 12:31:50.000000 feaASTools-0.2.2/Lib/feaASTools/renameGlyph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:31:51.962677 feaASTools-0.2.2/Lib/feaASTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 12:31:51.000000 feaASTools-0.2.2/Lib/feaASTools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 12:31:51.963677 feaASTools-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-11 12:31:50.000000 feaASTools-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-07-11 12:31:51.963677 feaASTools-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-11 12:31:50.000000 feaASTools-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:49:50.994314 feaASTools-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-11 21:49:49.000000 feaASTools-0.2.3/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:49:50.992314 feaASTools-0.2.3/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:49:50.993314 feaASTools-0.2.3/Lib/feaASTools/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-11 21:49:49.000000 feaASTools-0.2.3/Lib/feaASTools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4030 2023-07-11 21:49:49.000000 feaASTools-0.2.3/Lib/feaASTools/inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     9383 2023-07-11 21:49:49.000000 feaASTools-0.2.3/Lib/feaASTools/renameGlyph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:49:50.994314 feaASTools-0.2.3/Lib/feaASTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 21:49:50.000000 feaASTools-0.2.3/Lib/feaASTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-11 21:49:50.000000 feaASTools-0.2.3/Lib/feaASTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 21:49:50.000000 feaASTools-0.2.3/Lib/feaASTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 21:49:50.000000 feaASTools-0.2.3/Lib/feaASTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 21:49:50.000000 feaASTools-0.2.3/Lib/feaASTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 21:49:50.994314 feaASTools-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-11 21:49:49.000000 feaASTools-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-07-11 21:49:50.995314 feaASTools-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-11 21:49:49.000000 feaASTools-0.2.3/setup.py
```

### Comparing `feaASTools-0.2.2/LICENSE` & `feaASTools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feaASTools-0.2.2/Lib/feaASTools/renameGlyph.py` & `feaASTools-0.2.3/Lib/feaASTools/renameGlyph.py`

 * *Files identical despite different names*

### Comparing `feaASTools-0.2.2/Lib/feaASTools.egg-info/PKG-INFO` & `feaASTools-0.2.3/Lib/feaASTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feaASTools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tools to handle feature files (*.fea) as abstract syntax tree.
 Home-page: https://gitlab.com/fontstuff/feaASTools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/feaASTools
 Project-URL: Documentation, https://fontstuff.gitlab.io/feaASTools
 Project-URL: Tracker, https://gitlab.com/fontstuff/feaASTools/-/issues
```

### Comparing `feaASTools-0.2.2/PKG-INFO` & `feaASTools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feaASTools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tools to handle feature files (*.fea) as abstract syntax tree.
 Home-page: https://gitlab.com/fontstuff/feaASTools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/feaASTools
 Project-URL: Documentation, https://fontstuff.gitlab.io/feaASTools
 Project-URL: Tracker, https://gitlab.com/fontstuff/feaASTools/-/issues
```

### Comparing `feaASTools-0.2.2/setup.cfg` & `feaASTools-0.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

