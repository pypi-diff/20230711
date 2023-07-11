# Comparing `tmp/peek-admin-doc-3.4.7.tar.gz` & `tmp/peek-admin-doc-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-admin-doc-3.4.7.tar", last modified: Mon Jul  3 08:32:41 2023, max compression
+gzip compressed data, was "peek-admin-doc-3.4.8.tar", last modified: Tue Jul 11 02:51:46 2023, max compression
```

## Comparing `peek-admin-doc-3.4.7.tar` & `peek-admin-doc-3.4.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/peek_admin_doc/
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/peek_admin_doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/peek_admin_doc/_static/fonts/
--rw-r--r--   0 root         (0) root         (0)    77160 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/build_html_docs.sh
--rw-r--r--   0 root         (0) root         (0)      545 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/build_latex_docs.sh
--rw-r--r--   0 root         (0) root         (0)    11240 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1091 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/watch_docs.sh
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-03 08:32:04.000000 peek-admin-doc-3.4.7/peek_admin_doc/welcome.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:41.377061 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/peek_admin_doc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:32:41.378061 peek-admin-doc-3.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3077 2023-07-03 08:32:41.000000 peek-admin-doc-3.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:46.807134 peek-admin-doc-3.4.8/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-11 02:51:46.807134 peek-admin-doc-3.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:46.806134 peek-admin-doc-3.4.8/peek_admin_doc/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:46.806134 peek-admin-doc-3.4.8/peek_admin_doc/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:46.807134 peek-admin-doc-3.4.8/peek_admin_doc/_static/fonts/
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/build_html_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/build_latex_docs.sh
+-rw-r--r--   0 root         (0) root         (0)    11240 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/watch_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-11 02:51:10.000000 peek-admin-doc-3.4.8/peek_admin_doc/welcome.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:46.806134 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/peek_admin_doc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:51:46.807134 peek-admin-doc-3.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-07-11 02:51:46.000000 peek-admin-doc-3.4.8/setup.py
```

### Comparing `peek-admin-doc-3.4.7/README.rst` & `peek-admin-doc-3.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2` & `peek-admin-doc-3.4.8/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc/build_html_docs.sh` & `peek-admin-doc-3.4.8/peek_admin_doc/build_html_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc/build_latex_docs.sh` & `peek-admin-doc-3.4.8/peek_admin_doc/build_latex_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc/conf.py` & `peek-admin-doc-3.4.8/peek_admin_doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # sys.path.insert(0, os.path.abspath('.'))
 from sphinx.ext.apidoc import create_modules_toc_file, recurse_tree
 
 title = "Synerty Peek - Administration Documentation"
 __project__ = "SynertyPeek-AdminDocs"
 __copyright__ = "2021, Synerty"
 __author__ = "Synerty"
-__version__ = '3.4.7'
+__version__ = '3.4.8'
 
 import sphinx_rtd_theme
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
```

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc/watch_docs.sh` & `peek-admin-doc-3.4.8/peek_admin_doc/watch_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/peek_admin_doc.egg-info/SOURCES.txt` & `peek-admin-doc-3.4.8/peek_admin_doc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.7/setup.py` & `peek-admin-doc-3.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_admin_doc"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.7"
+package_version = "3.4.8"
 description = "Peek Admin Docs."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

