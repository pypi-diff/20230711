# Comparing `tmp/peek-field-doc-3.4.7.tar.gz` & `tmp/peek-field-doc-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-doc-3.4.7.tar", last modified: Mon Jul  3 08:33:23 2023, max compression
+gzip compressed data, was "peek-field-doc-3.4.8.tar", last modified: Tue Jul 11 02:52:29 2023, max compression
```

## Comparing `peek-field-doc-3.4.7.tar` & `peek-field-doc-3.4.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      672 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:23.487174 peek-field-doc-3.4.7/peek_field_doc/
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/peek_field_doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/peek_field_doc/_static/fonts/
--rw-r--r--   0 root         (0) root         (0)    77160 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/build_html_docs.sh
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/build_latex_docs.sh
--rw-r--r--   0 root         (0) root         (0)    10784 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/watch_docs.sh
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-03 08:32:05.000000 peek-field-doc-3.4.7/peek_field_doc/welcome.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/peek_field_doc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/peek_field_doc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:33:23.488174 peek-field-doc-3.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3090 2023-07-03 08:33:23.000000 peek-field-doc-3.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:29.457054 peek-field-doc-3.4.8/
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-11 02:52:29.457054 peek-field-doc-3.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      672 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:29.456054 peek-field-doc-3.4.8/peek_field_doc/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:29.457054 peek-field-doc-3.4.8/peek_field_doc/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:29.457054 peek-field-doc-3.4.8/peek_field_doc/_static/fonts/
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/build_html_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/build_latex_docs.sh
+-rw-r--r--   0 root         (0) root         (0)    10784 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/watch_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-11 02:51:11.000000 peek-field-doc-3.4.8/peek_field_doc/welcome.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:29.456054 peek-field-doc-3.4.8/peek_field_doc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/peek_field_doc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:52:29.457054 peek-field-doc-3.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-07-11 02:52:29.000000 peek-field-doc-3.4.8/setup.py
```

### Comparing `peek-field-doc-3.4.7/README.rst` & `peek-field-doc-3.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/peek_field_doc/_static/fonts/fontawesome-webfont.woff2` & `peek-field-doc-3.4.8/peek_field_doc/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/peek_field_doc/build_html_docs.sh` & `peek-field-doc-3.4.8/peek_field_doc/build_html_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/peek_field_doc/build_latex_docs.sh` & `peek-field-doc-3.4.8/peek_field_doc/build_latex_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/peek_field_doc/conf.py` & `peek-field-doc-3.4.8/peek_field_doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 title = "Synerty Peek - Field App Documentation"
 __project__ = "SynertyPeek-FieldAppDocs"
 __copyright__ = "2019, Synerty"
 __author__ = "Synerty"
-__version__ = '3.4.7'
+__version__ = '3.4.8'
 
 import sphinx_rtd_theme
 
 # -- General configuration ------------------------------------------------
 
 #
 # needs_sphinx = '1.0'
```

### Comparing `peek-field-doc-3.4.7/peek_field_doc/watch_docs.sh` & `peek-field-doc-3.4.8/peek_field_doc/watch_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/peek_field_doc.egg-info/SOURCES.txt` & `peek-field-doc-3.4.8/peek_field_doc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-field-doc-3.4.7/setup.py` & `peek-field-doc-3.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_doc"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.7"
+package_version = "3.4.8"
 description = "Peek Developer Documentation."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

