# Comparing `tmp/grainyhead-0.2.1.tar.gz` & `tmp/grainyhead-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grainyhead-0.2.1.tar", last modified: Wed Mar 22 09:59:33 2023, max compression
+gzip compressed data, was "grainyhead-0.3.0.tar", last modified: Mon Jul 10 22:27:12 2023, max compression
```

## Comparing `grainyhead-0.2.1.tar` & `grainyhead-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-03-22 09:59:33.556050 grainyhead-0.2.1/
--rw-r--r--   0 damien    (1000) users      (100)       61 2021-07-28 19:08:33.000000 grainyhead-0.2.1/.gitignore
--rw-r--r--   0 damien    (1000) users      (100)       39 2021-07-28 19:08:33.000000 grainyhead-0.2.1/AUTHORS
--rw-r--r--   0 damien    (1000) users      (100)    35147 2021-07-28 19:08:33.000000 grainyhead-0.2.1/COPYING
--rw-r--r--   0 damien    (1000) users      (100)       67 2023-01-28 22:09:44.000000 grainyhead-0.2.1/MANIFEST.in
--rw-r--r--   0 damien    (1000) users      (100)      478 2023-03-22 09:58:51.000000 grainyhead-0.2.1/NEWS
--rw-r--r--   0 damien    (1000) users      (100)     4936 2023-03-22 09:59:33.556050 grainyhead-0.2.1/PKG-INFO
--rw-r--r--   0 damien    (1000) users      (100)     4362 2023-01-28 22:09:44.000000 grainyhead-0.2.1/README.md
-drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-03-22 09:59:33.537050 grainyhead-0.2.1/docs/
--rw-r--r--   0 damien    (1000) users      (100)     2708 2022-08-14 15:49:39.000000 grainyhead-0.2.1/docs/caching.rst
--rw-r--r--   0 damien    (1000) users      (100)     1459 2022-05-10 21:52:09.000000 grainyhead-0.2.1/docs/conf.py
--rw-r--r--   0 damien    (1000) users      (100)     3318 2023-01-28 22:09:44.000000 grainyhead-0.2.1/docs/configuration.rst
--rw-r--r--   0 damien    (1000) users      (100)      399 2022-08-14 15:49:39.000000 grainyhead-0.2.1/docs/index.rst
--rw-r--r--   0 damien    (1000) users      (100)     2062 2023-03-22 09:58:51.000000 grainyhead-0.2.1/docs/install.rst
--rw-r--r--   0 damien    (1000) users      (100)    14832 2023-01-28 22:09:44.000000 grainyhead-0.2.1/docs/metrics.rst
--rw-r--r--   0 damien    (1000) users      (100)     2935 2023-01-28 22:09:44.000000 grainyhead-0.2.1/docs/old-issues.rst
--rw-r--r--   0 damien    (1000) users      (100)     1748 2023-01-28 22:09:44.000000 grainyhead-0.2.1/docs/quickstart.rst
-drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-03-22 09:59:33.538050 grainyhead-0.2.1/grainyhead.egg-info/
--rw-r--r--   0 damien    (1000) users      (100)     4936 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/PKG-INFO
--rw-r--r--   0 damien    (1000) users      (100)      695 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/SOURCES.txt
--rw-r--r--   0 damien    (1000) users      (100)        1 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/dependency_links.txt
--rw-r--r--   0 damien    (1000) users      (100)       59 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/entry_points.txt
--rw-r--r--   0 damien    (1000) users      (100)       58 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/requires.txt
--rw-r--r--   0 damien    (1000) users      (100)        7 2023-03-22 09:59:33.000000 grainyhead-0.2.1/grainyhead.egg-info/top_level.txt
-drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-03-22 09:59:33.538050 grainyhead-0.2.1/incenp/
--rw-r--r--   0 damien    (1000) users      (100)       65 2021-07-28 19:08:33.000000 grainyhead-0.2.1/incenp/__init__.py
-drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-03-22 09:59:33.556050 grainyhead-0.2.1/incenp/grainyhead/
--rw-r--r--   0 damien    (1000) users      (100)       22 2023-03-22 09:58:51.000000 grainyhead-0.2.1/incenp/grainyhead/__init__.py
--rw-r--r--   0 damien    (1000) users      (100)     7946 2022-08-21 00:27:11.000000 grainyhead-0.2.1/incenp/grainyhead/caching.py
--rw-r--r--   0 damien    (1000) users      (100)     5835 2023-01-28 22:23:17.000000 grainyhead-0.2.1/incenp/grainyhead/filtering.py
--rw-r--r--   0 damien    (1000) users      (100)    12788 2023-01-28 22:09:44.000000 grainyhead-0.2.1/incenp/grainyhead/main.py
--rw-r--r--   0 damien    (1000) users      (100)    16098 2023-01-28 22:23:17.000000 grainyhead-0.2.1/incenp/grainyhead/metrics.py
--rw-r--r--   0 damien    (1000) users      (100)     9941 2023-01-28 22:23:17.000000 grainyhead-0.2.1/incenp/grainyhead/providers.py
--rw-r--r--   0 damien    (1000) users      (100)     2671 2022-08-14 15:49:39.000000 grainyhead-0.2.1/incenp/grainyhead/repository.py
--rw-r--r--   0 damien    (1000) users      (100)     4603 2023-03-22 09:58:51.000000 grainyhead-0.2.1/incenp/grainyhead/util.py
--rw-r--r--   0 damien    (1000) users      (100)       46 2022-08-14 15:49:39.000000 grainyhead-0.2.1/pyproject.toml
--rw-r--r--   0 damien    (1000) users      (100)       59 2022-08-20 19:49:33.000000 grainyhead-0.2.1/requirements.txt
--rw-r--r--   0 damien    (1000) users      (100)       38 2023-03-22 09:59:33.556050 grainyhead-0.2.1/setup.cfg
--rw-r--r--   0 damien    (1000) users      (100)     1873 2023-01-28 22:09:44.000000 grainyhead-0.2.1/setup.py
+drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-07-10 22:27:12.292854 grainyhead-0.3.0/
+-rw-r--r--   0 damien    (1000) users      (100)       61 2021-07-28 19:08:33.000000 grainyhead-0.3.0/.gitignore
+-rw-r--r--   0 damien    (1000) users      (100)       39 2021-07-28 19:08:33.000000 grainyhead-0.3.0/AUTHORS
+-rw-r--r--   0 damien    (1000) users      (100)    35147 2021-07-28 19:08:33.000000 grainyhead-0.3.0/COPYING
+-rw-r--r--   0 damien    (1000) users      (100)       67 2023-01-28 22:09:44.000000 grainyhead-0.3.0/MANIFEST.in
+-rw-r--r--   0 damien    (1000) users      (100)     1073 2023-07-10 22:24:52.000000 grainyhead-0.3.0/NEWS
+-rw-r--r--   0 damien    (1000) users      (100)     4670 2023-07-10 22:27:12.292854 grainyhead-0.3.0/PKG-INFO
+-rw-r--r--   0 damien    (1000) users      (100)     4096 2023-07-10 22:17:52.000000 grainyhead-0.3.0/README.md
+drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-07-10 22:27:12.290854 grainyhead-0.3.0/docs/
+-rw-r--r--   0 damien    (1000) users      (100)     2708 2022-08-14 15:49:39.000000 grainyhead-0.3.0/docs/caching.rst
+-rw-r--r--   0 damien    (1000) users      (100)     1530 2023-07-10 22:18:25.000000 grainyhead-0.3.0/docs/conf.py
+-rw-r--r--   0 damien    (1000) users      (100)     3318 2023-01-28 22:09:44.000000 grainyhead-0.3.0/docs/configuration.rst
+-rw-r--r--   0 damien    (1000) users      (100)      399 2022-08-14 15:49:39.000000 grainyhead-0.3.0/docs/index.rst
+-rw-r--r--   0 damien    (1000) users      (100)     2062 2023-03-22 09:58:51.000000 grainyhead-0.3.0/docs/install.rst
+-rw-r--r--   0 damien    (1000) users      (100)    14956 2023-07-10 22:19:12.000000 grainyhead-0.3.0/docs/metrics.rst
+-rw-r--r--   0 damien    (1000) users      (100)     2935 2023-01-28 22:09:44.000000 grainyhead-0.3.0/docs/old-issues.rst
+-rw-r--r--   0 damien    (1000) users      (100)     1748 2023-01-28 22:09:44.000000 grainyhead-0.3.0/docs/quickstart.rst
+drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-07-10 22:27:12.291854 grainyhead-0.3.0/grainyhead.egg-info/
+-rw-r--r--   0 damien    (1000) users      (100)     4670 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/PKG-INFO
+-rw-r--r--   0 damien    (1000) users      (100)      695 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/SOURCES.txt
+-rw-r--r--   0 damien    (1000) users      (100)        1 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/dependency_links.txt
+-rw-r--r--   0 damien    (1000) users      (100)       59 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/entry_points.txt
+-rw-r--r--   0 damien    (1000) users      (100)       58 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/requires.txt
+-rw-r--r--   0 damien    (1000) users      (100)        7 2023-07-10 22:27:12.000000 grainyhead-0.3.0/grainyhead.egg-info/top_level.txt
+drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-07-10 22:27:12.291854 grainyhead-0.3.0/incenp/
+-rw-r--r--   0 damien    (1000) users      (100)       65 2021-07-28 19:08:33.000000 grainyhead-0.3.0/incenp/__init__.py
+drwxr-xr-x   0 damien    (1000) users      (100)        0 2023-07-10 22:27:12.291854 grainyhead-0.3.0/incenp/grainyhead/
+-rw-r--r--   0 damien    (1000) users      (100)       22 2023-07-10 22:15:30.000000 grainyhead-0.3.0/incenp/grainyhead/__init__.py
+-rw-r--r--   0 damien    (1000) users      (100)     8246 2023-07-10 22:14:35.000000 grainyhead-0.3.0/incenp/grainyhead/caching.py
+-rw-r--r--   0 damien    (1000) users      (100)     5835 2023-01-28 22:23:17.000000 grainyhead-0.3.0/incenp/grainyhead/filtering.py
+-rw-r--r--   0 damien    (1000) users      (100)    12793 2023-07-10 22:14:11.000000 grainyhead-0.3.0/incenp/grainyhead/main.py
+-rw-r--r--   0 damien    (1000) users      (100)    16422 2023-07-10 22:15:01.000000 grainyhead-0.3.0/incenp/grainyhead/metrics.py
+-rw-r--r--   0 damien    (1000) users      (100)    10531 2023-07-10 22:14:47.000000 grainyhead-0.3.0/incenp/grainyhead/providers.py
+-rw-r--r--   0 damien    (1000) users      (100)     4020 2023-07-10 22:12:51.000000 grainyhead-0.3.0/incenp/grainyhead/repository.py
+-rw-r--r--   0 damien    (1000) users      (100)     4603 2023-03-22 09:58:51.000000 grainyhead-0.3.0/incenp/grainyhead/util.py
+-rw-r--r--   0 damien    (1000) users      (100)       46 2022-08-14 15:49:39.000000 grainyhead-0.3.0/pyproject.toml
+-rw-r--r--   0 damien    (1000) users      (100)       59 2022-08-20 19:49:33.000000 grainyhead-0.3.0/requirements.txt
+-rw-r--r--   0 damien    (1000) users      (100)       38 2023-07-10 22:27:12.292854 grainyhead-0.3.0/setup.cfg
+-rw-r--r--   0 damien    (1000) users      (100)     1873 2023-01-28 22:09:44.000000 grainyhead-0.3.0/setup.py
```

### Comparing `grainyhead-0.2.1/COPYING` & `grainyhead-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/PKG-INFO` & `grainyhead-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grainyhead
-Version: 0.2.1
+Version: 0.3.0
 Summary: Helper tools for GitHub
 Home-page: UNKNOWN
 Author: Damien Goutte-Gattat
 Author-email: dpg44@cam.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -107,25 +107,25 @@
 The `metrics` command will list some statistics about the repository
 over a given period of time:
 
 ```
 $ grainyhead metrics
 From 2021-09-02 to 2021-12-01
 
-| Event                | Total | Internal | Inte (%) | External | Exte (%) |
-| -------------------- | ----- | -------- | -------- | -------- | -------- |
-| Contributors         |    24 |       15 |    62.50 |        9 |    37.50 |
-| Issues opened        |    71 |       64 |    90.14 |        7 |     9.86 |
-| Issues closed        |    89 |       77 |    86.52 |       12 |    13.48 |
-| Pull requests opened |    86 |       68 |    79.07 |       18 |    20.93 |
-| Pull requests closed |    94 |       78 |    82.98 |       16 |    17.02 |
-| Pull requests merged |    79 |       65 |    82.28 |       14 |    17.72 |
-| Comments             |   476 |      412 |    86.55 |       64 |    13.45 |
-| Commits              |   232 |      201 |    86.64 |       31 |    13.36 |
-| Releases             |     4 |        4 |   100.00 |        0 |     0.00 |
+| Event | Total | Internal | Internal (%) | External | Externam (%) |
+| -------- | -------- | -------- | -------- | -------- | -------- |
+| Contributors | 24 | 15 | 62.50 | 9 | 37.50 |
+| Issues opened | 71 | 64 | 90.14 | 7 | 9.86 |
+| Issues closed | 89 | 77 | 86.52 | 12 | 13.48 |
+| Pull requests opened | 86 | 68 | 79.07 | 18 | 20.93 |
+| Pull requests closed | 94 | 78 | 82.98 | 16 | 17.02 |
+| Pull requests merged | 79 | 65 | 82.28 | 14 | 17.72 |
+| Comments | 476 | 412 | 86.55 | 64 | 13.45 |
+| Commits | 232 | 201 | 86.64 | 31 | 13.36 |
+| Releases | 4 | 4 | 100.00 | 0 | 0.00 |
 ```
 
 
 Copying
 -------
 GrainyHead is distributed under the terms of the GNU General Public
 License, version 3 or higher. The full license is included in the
```

### Comparing `grainyhead-0.2.1/README.md` & `grainyhead-0.3.0/grainyhead.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: grainyhead
+Version: 0.3.0
+Summary: Helper tools for GitHub
+Home-page: UNKNOWN
+Author: Damien Goutte-Gattat
+Author-email: dpg44@cam.ac.uk
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+Provides-Extra: IPython
+License-File: COPYING
+License-File: AUTHORS
+
 GrainyHead - Helper tools for GitHub
 ====================================
 
 GrainyHead is a set of Python scripts to work with GitHub repositories
 from the command line.
 
 The name comes from the fruit fly gene _grainyhead_ (_grh_).
@@ -88,25 +107,25 @@
 The `metrics` command will list some statistics about the repository
 over a given period of time:
 
 ```
 $ grainyhead metrics
 From 2021-09-02 to 2021-12-01
 
-| Event                | Total | Internal | Inte (%) | External | Exte (%) |
-| -------------------- | ----- | -------- | -------- | -------- | -------- |
-| Contributors         |    24 |       15 |    62.50 |        9 |    37.50 |
-| Issues opened        |    71 |       64 |    90.14 |        7 |     9.86 |
-| Issues closed        |    89 |       77 |    86.52 |       12 |    13.48 |
-| Pull requests opened |    86 |       68 |    79.07 |       18 |    20.93 |
-| Pull requests closed |    94 |       78 |    82.98 |       16 |    17.02 |
-| Pull requests merged |    79 |       65 |    82.28 |       14 |    17.72 |
-| Comments             |   476 |      412 |    86.55 |       64 |    13.45 |
-| Commits              |   232 |      201 |    86.64 |       31 |    13.36 |
-| Releases             |     4 |        4 |   100.00 |        0 |     0.00 |
+| Event | Total | Internal | Internal (%) | External | Externam (%) |
+| -------- | -------- | -------- | -------- | -------- | -------- |
+| Contributors | 24 | 15 | 62.50 | 9 | 37.50 |
+| Issues opened | 71 | 64 | 90.14 | 7 | 9.86 |
+| Issues closed | 89 | 77 | 86.52 | 12 | 13.48 |
+| Pull requests opened | 86 | 68 | 79.07 | 18 | 20.93 |
+| Pull requests closed | 94 | 78 | 82.98 | 16 | 17.02 |
+| Pull requests merged | 79 | 65 | 82.28 | 14 | 17.72 |
+| Comments | 476 | 412 | 86.55 | 64 | 13.45 |
+| Commits | 232 | 201 | 86.64 | 31 | 13.36 |
+| Releases | 4 | 4 | 100.00 | 0 | 0.00 |
 ```
 
 
 Copying
 -------
 GrainyHead is distributed under the terms of the GNU General Public
 License, version 3 or higher. The full license is included in the
@@ -116,7 +135,9 @@
 Homepage and repository
 -----------------------
 
 The project is located at <https://incenp.org/dvlpt/grainyhead.html>
 with the manual at <https://incenp.org/dvlpt/grainyhead/index.html>.
 The source code is available in a Git repository at
 <https://github.com/gouttegd/grainyhead>.
+
+
```

### Comparing `grainyhead-0.2.1/docs/caching.rst` & `grainyhead-0.3.0/docs/caching.rst`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/docs/conf.py` & `grainyhead-0.3.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -- General configuration ------------------------------------------------
 
 source_suffix = '.rst'
 master_doc = 'index'
 
-copyright = u'2021,2022 Damien Goutte-Gattat'
+copyright = u'2021,2022,2023 Damien Goutte-Gattat'
 author = u'Damien Goutte-Gattat <dpg44@cam.ac.uk>'
 
 language = 'en'
 
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 pygments_style = 'sphinx'
@@ -20,34 +20,39 @@
 html_theme = 'sphinx_rtd_theme'
 html_static_path = ['_static']
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_engine = 'lualatex'
 
-latex_elements = {
-        'papersize': 'a4paper',
-        'pointsize': '10pt'
-}
+latex_elements = {'papersize': 'a4paper', 'pointsize': '10pt'}
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'GrainyHead.tex', u'GrainyHead Documentation',
-     u'Damien Goutte-Gattat', 'manual'),
+    (
+        master_doc,
+        'GrainyHead.tex',
+        u'GrainyHead Documentation',
+        u'Damien Goutte-Gattat',
+        'manual',
+    ),
 ]
 
 # -- Options for manual page output ---------------------------------------
 
-man_pages = [
-    (master_doc, 'grainyhead', u'GrainyHead Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, 'grainyhead', u'GrainyHead Documentation', [author], 1)]
 
 # -- Options for Texinfo output -------------------------------------------
 
 texinfo_documents = [
-    (master_doc, 'GrainyHead', u'GrainyHead Documentation',
-     author, 'GrainyHead', 'Helper tools for GitHub.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        'GrainyHead',
+        u'GrainyHead Documentation',
+        author,
+        'GrainyHead',
+        'Helper tools for GitHub.',
+        'Miscellaneous',
+    ),
 ]
```

### Comparing `grainyhead-0.2.1/docs/configuration.rst` & `grainyhead-0.3.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/docs/install.rst` & `grainyhead-0.3.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/docs/metrics.rst` & `grainyhead-0.3.0/docs/metrics.rst`

 * *Files 24% similar despite different names*

```diff
@@ -44,25 +44,25 @@
 Here is an example of a default report:
 
 .. code-block:: console
 
    $ grainyhead metrics
    From 2021-09-02 to 2021-12-01
    
-   | Event                | Total | Internal | Inte (%) | External | Exte (%) |
-   | -------------------- | ----- | -------- | -------- | -------- | -------- |
-   | Contributors         |    24 |       15 |    62.50 |        9 |    37.50 |
-   | Issues opened        |    71 |       64 |    90.14 |        7 |     9.86 |
-   | Issues closed        |    89 |       77 |    86.52 |       12 |    13.48 |
-   | Pull requests opened |    86 |       68 |    79.07 |       18 |    20.93 |
-   | Pull requests closed |    94 |       78 |    82.98 |       16 |    17.02 |
-   | Pull requests merged |    79 |       65 |    82.28 |       14 |    17.72 |
-   | Comments             |   476 |      412 |    86.55 |       64 |    13.45 |
-   | Commits              |   232 |      201 |    86.64 |       31 |    13.36 |
-   | Releases             |     4 |        4 |   100.00 |        0 |     0.00 |
+   | Event | Total | Internal | Internal (%) | External | External (%) |
+   | -------- | -------- | -------- | -------- | -------- | -------- |
+   | Contributors | 24 | 15 | 62.50 | 9 | 37.50 |
+   | Issues opened | 71 | 64 | 90.14 | 7 | 9.86 |
+   | Issues closed | 89 | 77 | 86.52 | 12 | 13.48 |
+   | Pull requests opened | 86 | 68 | 79.07 | 18 | 20.93 |
+   | Pull requests closed | 94 | 78 | 82.98 | 16 | 17.02 |
+   | Pull requests merged | 79 | 65 | 82.28 | 14 | 17.72 |
+   | Comments | 476 | 412 | 86.55 | 64 | 13.45 |
+   | Commits | 232 | 201 | 86.64 | 31 | 13.36 |
+   | Releases | 4 | 4 | 100.00 | 0 | 0.00 |
 
 This report indicates, for example, that 24 users contributed to the repository
 between September 2nd, 2021 and December 1st, 2021; 15 of them (62.5%) were
 known contributors, the other 9 being external users.
 
 
 Custom reports
@@ -134,52 +134,83 @@
 The ``--selector`` option can be repeated as many times as needed to collect
 metrics about different sets of events.
 
 Each selector can be given a human-readable *NAME* to be displayed in the column
 header, by appending ``= NAME`` (or alternatively, ``AS name``, but that form is
 deprecated and should not be used anymore) to the selector.
 
-The ``user`` and ``label`` selectors accept a special syntactic sugar:
-``user:*`` and ``label:*`` will collect events for all contributors and for all
-labels in the repository, respectively. That is, ``--selector 'user:*'`` is
-equivalent for ``--selector user:user1 --selector user:user2 ...``, for all
-users *user1*, *user2*, ..., known to have contributed to the repository;
-likewise, ``--selector 'label:*'`` is equivalent to ``--selector label:label1
---selector label:label2 ...`` for all labels *label1*, *label2*, ..., ever used
-in the repository. Of note, only one wild-card selector may be used in any given
-expression: it is not possible to use both ``user:*`` and ``label:*`` inside the
-same selector option.
+The ``user`` selector accepts a special syntactic sugar: ``user:*TEAM`` will
+collect events for all users in team *TEAM* (or for all contributors if no team
+is specified, that is if the selector is simply ``user:*``). That is,
+``--selector 'user:*elite'`` is equivalent to ``--selector user:user1
+--selector user:user2 ...`` where *user1*, *user2*, etc. are members of the
+*elite* team.
+
+The ``team`` selector similarly accepts the syntactic sugar ``team:*``, which
+will collect events for all labels in the repository. That is, ``--selector
+'label:*'`` is equivalent to ``--selector label:label` --selector label:label2
+...`` for all labels *label1*, *label2*, etc. ever used in the repository.
+
+Of note, only one wild-card selector may be used in any given expression: it is
+not possible to use both ``user:*`` (with or without a team name) and
+``label:*`` inside the same selector option.
 
 Here is an example of a custom report request:
 
 .. code-block:: console
 
    $ grainyhead metrics \
        --selector 'all = Total' \
        --selector '!team:elite = Others' \
        --selector 'label:bugfix = Bugs'
    From 2021-11-09 to 2022-05-08
    
-   | Event                | Total    | Others   | Othe (%) | Bugs     | Bugs (%) |
-   | -------------------- | -------- | -------- | -------- | -------- | -------- |
-   | Contributors         |       46 |       20 |    43.48 |       44 |    95.65 |
-   | Issues opened        |      184 |      116 |    63.04 |      136 |    73.91 |
-   | Issues closed        |      134 |      133 |    99.25 |      106 |    79.10 |
-   | Pull requests opened |      200 |      193 |    96.50 |      196 |    98.00 |
-   | Pull requests closed |      164 |      164 |   100.00 |      162 |    98.78 |
-   | Pull requests merged |      139 |      139 |   100.00 |      138 |    99.28 |
-   | Comments             |     1085 |      938 |    86.45 |        0 |     0.00 |
-   | Commits              |      485 |      475 |    97.94 |        0 |     0.00 |
-   | Releases             |        5 |        5 |   100.00 |        0 |     0.00 |
+   | Event | Total | Others | Others (%) | Bugs | Bugs (%) |
+   | -------- | -------- | -------- | -------- | -------- | -------- |
+   | Contributors | 46 | 20 | 43.48 | 44 | 95.65 |
+   | Issues opened | 184 | 116 | 63.04 | 136 | 73.91 |
+   | Issues closed | 134 | 133 | 99.25 | 106 | 79.10 |
+   | Pull requests opened | 200 | 193 | 96.50 | 196 | 98.00 |
+   | Pull requests closed | 164 | 164 | 100.00 | 162 | 98.78 |
+   | Pull requests merged | 139 | 139 | 100.00 | 138 | 99.28 |
+   | Comments | 1085 | 938 | 86.45 | 0 | 0.00 |
+   | Commits | 485 | 475 | 97.94 | 0 | 0.00 |
+   | Releases | 5 | 5 | 100.00 | 0 | 0.00 |
 
 It prints the numbers of all events in the repository, the number of events
 originating from users that are not members of the *elite* team, and the number
 of events labelled with the *bugfix* label.
 
 
+Special team names
+------------------
+
+The ``team`` selector will recognise a handful of special names, all starting with
+``__``:
+
+``team:__collaborators``
+    All users that are registered as collaborators on the repository.
+    
+``team:__committers``
+    All users who ever committed to the repository.
+    
+``team:__commenters``
+    All users who ever opened a ticket or a PR or commented on a ticket or a PR.
+    
+``team:__contributors``
+    All users who ever contributed anything (commit, issue, PR, comment) to the
+    repository.
+    
+These names are also recognised by the ``user:*TEAM`` syntactic sugar. For
+example, ``--selector 'user:*__committers'`` will be equivalent to ``--selector
+user:user1 --selector user:user2 ...`` where *user1*, *user2*, etc. are users
+who contributed commits to the repository. The special ``user:*`` sugar is
+strictly equivalent to ``user:*__contributors``. 
+
+
 Report formats
 --------------
 
 The ``metrics`` command can print the metrics in four different formats:
 Markdown, JSON, CSV, and TSV. The format can be chosen with the ``--format``
 option. The default format is Markdown.
 
@@ -201,48 +232,48 @@
 .. code-block:: console
 
    $ grainyhead metrics \
        --selector '!team:elite = Others' \
        --selector 'label:bugfix'
    From 2021-11-09 to 2022-05-08
    
-   | Event                | Others   | label:bu |
-   | -------------------- | -------- | -------- |
-   | Contributors         |       20 |       44 |
-   | Issues opened        |      116 |      136 |
-   | Issues closed        |      133 |      106 |
-   | Pull requests opened |      193 |      196 |
-   | Pull requests closed |      164 |      162 |
-   | Pull requests merged |      139 |      138 |
-   | Comments             |      938 |        0 |
-   | Commits              |      475 |        0 |
-   | Releases             |        5 |        0 |
+   | Event | Others | label:bugfix |
+   | -------- | -------- | -------- |
+   | Contributors | 20 | 44 |
+   | Issues opened | 116 | 136 |
+   | Issues closed | 133 | 106 |
+   | Pull requests opened | 193 | 196 |
+   | Pull requests closed | 164 | 162 |
+   | Pull requests merged | 139 | 138 |
+   | Comments | 938 | 0 |
+   | Commits | 475 | 0 |
+   | Releases | 5 | 0 |
 
 As a convenience, if the *first* selector is the ``all`` selector, then for each
 subsequent selector, an extra column is appended to give the proportion of
 events corresponding to the selector relatively to all events:
 
 .. code-block:: console
 
    $ grainyhead metrics \
        --selector 'all = Total' \
        --selector '!team:elite = Others'
    From 2021-11-09 to 2022-05-08
    
-   | Event                | Total    | Others   | Othe (%) |
-   | -------------------- | -------- | -------- | -------- |
-   | Contributors         |       46 |       20 |    43.48 |
-   | Issues opened        |      184 |      116 |    63.04 |
-   | Issues closed        |      134 |      133 |    99.25 |
-   | Pull requests opened |      200 |      193 |    96.50 |
-   | Pull requests closed |      164 |      164 |   100.00 |
-   | Pull requests merged |      139 |      139 |   100.00 |
-   | Comments             |     1085 |      938 |    86.45 |
-   | Commits              |      485 |      475 |    97.94 |
-   | Releases             |        5 |        5 |   100.00 | 
+   | Event | Total | Others | Others (%) |
+   | -------- | -------- | -------- | -------- |
+   | Contributors | 46 | 20 | 43.48 |
+   | Issues opened | 184 | 116 | 63.04 |
+   | Issues closed | 134 | 133 | 99.25 |
+   | Pull requests opened | 200 | 193 | 96.50 |
+   | Pull requests closed | 164 | 164 | 100.00 |
+   | Pull requests merged | 139 | 139 | 100.00 |
+   | Comments | 1085 | 938 | 86.45 |
+   | Commits | 485 | 475 | 97.94 |
+   | Releases | 5 | 5 | 100.00 | 
 
 
 JSON format
 ^^^^^^^^^^^
 
 The JSON format is intended for easy consumption of the report by downstream
 scripts. The output is a JSON dictionary containing two keys, as follows:
```

### Comparing `grainyhead-0.2.1/docs/old-issues.rst` & `grainyhead-0.3.0/docs/old-issues.rst`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/docs/quickstart.rst` & `grainyhead-0.3.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/grainyhead.egg-info/PKG-INFO` & `grainyhead-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: grainyhead
-Version: 0.2.1
-Summary: Helper tools for GitHub
-Home-page: UNKNOWN
-Author: Damien Goutte-Gattat
-Author-email: dpg44@cam.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
-Provides-Extra: IPython
-License-File: COPYING
-License-File: AUTHORS
-
 GrainyHead - Helper tools for GitHub
 ====================================
 
 GrainyHead is a set of Python scripts to work with GitHub repositories
 from the command line.
 
 The name comes from the fruit fly gene _grainyhead_ (_grh_).
@@ -107,25 +88,25 @@
 The `metrics` command will list some statistics about the repository
 over a given period of time:
 
 ```
 $ grainyhead metrics
 From 2021-09-02 to 2021-12-01
 
-| Event                | Total | Internal | Inte (%) | External | Exte (%) |
-| -------------------- | ----- | -------- | -------- | -------- | -------- |
-| Contributors         |    24 |       15 |    62.50 |        9 |    37.50 |
-| Issues opened        |    71 |       64 |    90.14 |        7 |     9.86 |
-| Issues closed        |    89 |       77 |    86.52 |       12 |    13.48 |
-| Pull requests opened |    86 |       68 |    79.07 |       18 |    20.93 |
-| Pull requests closed |    94 |       78 |    82.98 |       16 |    17.02 |
-| Pull requests merged |    79 |       65 |    82.28 |       14 |    17.72 |
-| Comments             |   476 |      412 |    86.55 |       64 |    13.45 |
-| Commits              |   232 |      201 |    86.64 |       31 |    13.36 |
-| Releases             |     4 |        4 |   100.00 |        0 |     0.00 |
+| Event | Total | Internal | Internal (%) | External | Externam (%) |
+| -------- | -------- | -------- | -------- | -------- | -------- |
+| Contributors | 24 | 15 | 62.50 | 9 | 37.50 |
+| Issues opened | 71 | 64 | 90.14 | 7 | 9.86 |
+| Issues closed | 89 | 77 | 86.52 | 12 | 13.48 |
+| Pull requests opened | 86 | 68 | 79.07 | 18 | 20.93 |
+| Pull requests closed | 94 | 78 | 82.98 | 16 | 17.02 |
+| Pull requests merged | 79 | 65 | 82.28 | 14 | 17.72 |
+| Comments | 476 | 412 | 86.55 | 64 | 13.45 |
+| Commits | 232 | 201 | 86.64 | 31 | 13.36 |
+| Releases | 4 | 4 | 100.00 | 0 | 0.00 |
 ```
 
 
 Copying
 -------
 GrainyHead is distributed under the terms of the GNU General Public
 License, version 3 or higher. The full license is included in the
@@ -135,9 +116,7 @@
 Homepage and repository
 -----------------------
 
 The project is located at <https://incenp.org/dvlpt/grainyhead.html>
 with the manual at <https://incenp.org/dvlpt/grainyhead/index.html>.
 The source code is available in a Git repository at
 <https://github.com/gouttegd/grainyhead>.
-
-
```

### Comparing `grainyhead-0.2.1/grainyhead.egg-info/SOURCES.txt` & `grainyhead-0.3.0/grainyhead.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/incenp/grainyhead/caching.py` & `grainyhead-0.3.0/incenp/grainyhead/caching.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # grainyhead - Helper tools for GitHub
-# Copyright © 2021 Damien Goutte-Gattat
+# Copyright © 2021,2023 Damien Goutte-Gattat
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -187,14 +187,17 @@
         if item_type == RepositoryItemType.ISSUES:
             # Force full refresh, so that we get updated status for
             # old issues
             return None
         elif item_type in [RepositoryItemType.LABELS, RepositoryItemType.TEAMS]:
             # Always fetch everything for those
             return None
+        elif item_type == RepositoryItemType.COMMITTERS:
+            # Always fetch everything for those
+            return None
         elif item_type == RepositoryItemType.COMMITS:
             # Only get new commits
             return datetime.strptime(data[-1].commit.author.date, GITHUB_DATE_FORMAT)
         else:
             # Only get new other items
             return datetime.strptime(data[-1].created_at, GITHUB_DATE_FORMAT)
 
@@ -214,14 +217,17 @@
             )
         elif item_type == RepositoryItemType.LABELS:
             # Identify duplicates by label ID
             return list({l.id: l for l in data}.values())
         elif item_type == RepositoryItemType.TEAMS:
             # Identify duplicates by team "slugs"
             return list({t.slug: t for t in data}.values())
+        elif item_type == RepositoryItemType.COMMITTERS:
+            # Identify duplicates by login name
+            return list({l.login: l for l in data}.values())
         else:
             # Identify duplicates by item ID, then force descending
             # chronological order
             return sorted(
                 {i.id: i for i in data}.values(),
                 reverse=True,
                 key=lambda i: datetime.strptime(i.created_at, GITHUB_DATE_FORMAT),
```

### Comparing `grainyhead-0.2.1/incenp/grainyhead/filtering.py` & `grainyhead-0.3.0/incenp/grainyhead/filtering.py`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/incenp/grainyhead/main.py` & `grainyhead-0.3.0/incenp/grainyhead/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # grainyhead - Helper tools for GitHub
-# Copyright © 2021,2022 Damien Goutte-Gattat
+# Copyright © 2021,2022,2023 Damien Goutte-Gattat
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grainyhead-0.2.1/incenp/grainyhead/metrics.py` & `grainyhead-0.3.0/incenp/grainyhead/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # grainyhead - Helper tools for GitHub
-# Copyright © 2021,2022 Damien Goutte-Gattat
+# Copyright © 2021,2022,2023 Damien Goutte-Gattat
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -68,15 +68,19 @@
 
     def _get_report_for_period(self, selectors, start, end):
         rset = _MetricsReportSet(start, end)
         self._date_filter = DateRangeFilter(start, end)
 
         for selector in selectors:
             item_filter = self._get_filter_from_selector(selector)
-            rset.contributions.append(self.get_single_report(item_filter))
+            report = self.get_single_report(item_filter)
+            if report.name.startswith('@') and report.all_contributions == 0:
+                # Exclude reports for users with no contributions at all
+                continue
+            rset.contributions.append(report)
 
         return rset
 
     def get_single_report(self, item_filter):
         """Get a single report object based on the given filter."""
 
         issues_opened = [i for i in self._repo.all_issues if item_filter.filter(i)]
@@ -137,20 +141,23 @@
     def _expand_wildcard_selectors(self, selectors):
         if not True in ['*' in s for s in selectors]:
             return selectors
 
         expanded_selectors = []
         for selector in selectors:
             if 'user:*' in selector:
+                group = selector[6:].split(' ', 2)[0]
+                real_group = group if len(group) > 0 else '__contributors'
                 expanded_selectors.extend(
                     [
-                        selector.replace('user:*', f'user:{u}')
-                        for u in self._repo.contributors
+                        selector.replace('user:*' + group, f'user:{u}')
+                        for u in self._repo.get_usernames(real_group)
                     ]
                 )
+
             elif 'label:*' in selector:
                 expanded_selectors.extend(
                     [
                         selector.replace('label:*', f'label:{l}')
                         for l in self._repo.labels
                     ]
                 )
@@ -167,17 +174,15 @@
             filter_value = pp.Combine(
                 pp.Word(pp.alphanums + '-_')
                 + (pp.White() + pp.Word(pp.alphanums + '-_'))[...]
             ).leaveWhitespace()
             team_filter = (
                 (pp.Literal('team:') + filter_value)
                 .set_parse_action(
-                    lambda t: TeamFilter(
-                        t[1], [m.login for m in self._repo.get_team(t[1])]
-                    )
+                    lambda t: TeamFilter(t[1], self._repo.get_usernames(t[1]))
                 )
                 .leave_whitespace()
             )
             user_filter = (
                 (pp.Literal('user:') + filter_value)
                 .set_parse_action(lambda t: UserFilter(t[1]))
                 .leave_whitespace()
@@ -310,27 +315,27 @@
         end = reportset.end_date
 
         with_total = reportset.contributions[0].selector == 'all'
 
         output.write(f"From {start:%Y-%m-%d} to {end:%Y-%m-%d}\n")
         output.write("\n")
 
-        output.write("| Event                |")
+        output.write("| Event |")
         if with_total:
-            output.write(f" {reportset.contributions[0].name:8.8} |")
+            output.write(f" {reportset.contributions[0].name} |")
             for report in reportset.contributions[1:]:
-                output.write(f" {report.name:8.8} | {report.name:4.4} (%) |")
+                output.write(f" {report.name} | {report.name} (%) |")
             output.write("\n")
-            output.write("| -------------------- | -------- |")
+            output.write("| -------- | -------- |")
             for report in reportset.contributions[1:]:
                 output.write(" -------- | -------- |")
             output.write("\n")
         else:
             for report in reportset.contributions:
-                output.write(f" {report.name:8.8} |")
+                output.write(f" {report.name} |")
             output.write("\n")
             output.write("| -------------------- |")
             for report in reportset.contributions:
                 output.write(" -------- |")
             output.write("\n")
 
         items = [
@@ -350,28 +355,28 @@
         output.write('\n')
 
     def _write_line(self, label, reports, output, with_total):
         property_name = label.lower().replace(' ', '_')
 
         if with_total:
             total = getattr(reports[0], property_name)
-            output.write(f"| {label:20} | {total: 8} |")
+            output.write(f"| {label} | {total} |")
 
             for report in reports[1:]:
                 value = getattr(report, property_name)
                 if total > 0:
                     percent = value / total * 100
                 else:
                     percent = 0.0
-                output.write(f" {value:8} | {percent: 8.2f} |")
+                output.write(f" {value} | {percent: .2f} |")
         else:
-            output.write(f"| {label:20} |")
+            output.write(f"| {label} |")
             for report in reports:
                 value = getattr(report, property_name)
-                output.write(f" {value:8} |")
+                output.write(f" {value} |")
         output.write("\n")
 
 
 class CsvMetricsFormatter(MetricsFormatter):
     def __init__(self, sep=','):
         self._sep = sep
 
@@ -496,14 +501,18 @@
     def commits(self):
         return self._values[6]
 
     @property
     def releases(self):
         return self._values[7]
 
+    @property
+    def all_contributions(self):
+        return sum(self._values)
+
 
 class NamedFilter(IntersectionFilter):
     def __init__(self, name, filters):
         IntersectionFilter.__init__(self, filters)
         self._name = name
 
     @property
```

### Comparing `grainyhead-0.2.1/incenp/grainyhead/providers.py` & `grainyhead-0.3.0/incenp/grainyhead/providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # grainyhead - Helper tools for GitHub
-# Copyright © 2021,2022 Damien Goutte-Gattat
+# Copyright © 2021,2022,2023 Damien Goutte-Gattat
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -35,14 +35,15 @@
     ISSUES = 1
     COMMENTS = 2
     TEAMS = 3
     LABELS = 4
     EVENTS = 5
     COMMITS = 6
     RELEASES = 7
+    COMMITTERS = 8
 
 
 class RepositoryItem(AttrDict):
     """An item from a GitHub repository.
 
     This class extends the AttrDict class used by GhApi to provide
     helper methods to manipulate the items.
@@ -196,14 +197,18 @@
     def commits(self):
         return self.get_data(RepositoryItemType.COMMITS)
 
     @property
     def releases(self):
         return self.get_data(RepositoryItemType.RELEASES)
 
+    @property
+    def committers(self):
+        return self.get_data(RepositoryItemType.COMMITTERS)
+
 
 class OnlineRepositoryProvider(RepositoryProvider):
     """Provides direct access to the data from a GitHub repository."""
 
     def __init__(self, api):
         """Creates a new instance.
 
@@ -227,18 +232,33 @@
         data = None
         if item_type == RepositoryItemType.ISSUES:
             data = self._fetch(
                 self._api.issues.list_for_repo, apiargs={'state': 'all'}, since=since
             )
         elif item_type == RepositoryItemType.TEAMS:
             data = self._fetch_teams()
+        elif item_type == RepositoryItemType.COMMITTERS:
+            data = self._fetch_committers()
         else:
             data = self._fetch(self._calls[item_type], since=since)
         return data
 
+    def _fetch_committers(self):
+        committers = self._api.repos.list_contributors(per_page=100)
+        last_page = self._api.last_page()
+        page = 0
+
+        while page < last_page:
+            page += 1
+            committers.extend(
+                self._api.repos.list_contributors(per_page=100, page=page)
+            )
+
+        return committers
+
     def _fetch(self, apicall, apiargs={}, since=None):
         """Generic method to fetch data from GitHub."""
 
         if since is not None:
             if apicall in self._calls_without_since:
                 # No support for 'since=' parameter in those calls,
                 # we need to ensure manually that we don't get more
```

### Comparing `grainyhead-0.2.1/incenp/grainyhead/util.py` & `grainyhead-0.3.0/incenp/grainyhead/util.py`

 * *Files identical despite different names*

### Comparing `grainyhead-0.2.1/setup.py` & `grainyhead-0.3.0/setup.py`

 * *Files identical despite different names*

