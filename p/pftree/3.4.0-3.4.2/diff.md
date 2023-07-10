# Comparing `tmp/pftree-3.4.0.tar.gz` & `tmp/pftree-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pftree-3.4.0.tar", last modified: Thu Jun 22 21:12:18 2023, max compression
+gzip compressed data, was "pftree-3.4.2.tar", last modified: Mon Jul 10 22:33:41 2023, max compression
```

## Comparing `pftree-3.4.0.tar` & `pftree-3.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2022-10-06 19:19:07.000000 pftree-3.4.0/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-06-22 21:12:18.918562 pftree-3.4.0/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9639 2022-10-11 16:42:40.000000 pftree-3.4.0/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/pftree/
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      123 2022-10-06 19:19:07.000000 pftree-3.4.0/pftree/__init__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    21572 2022-10-19 15:31:08.000000 pftree-3.4.0/pftree/__main__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    60593 2023-06-22 21:07:06.000000 pftree-3.4.0/pftree/pftree.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/pftree.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      293 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       48 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-10-11 15:48:34.000000 pftree-3.4.0/pftree.egg-info/not-zip-safe
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        7 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-06-22 21:12:18.918562 pftree-3.4.0/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      901 2023-06-22 21:09:51.000000 pftree-3.4.0/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-07-10 22:33:41.008049 pftree-3.4.2/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2022-09-30 15:08:40.000000 pftree-3.4.2/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-07-10 22:33:41.008049 pftree-3.4.2/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9639 2022-10-13 15:00:28.000000 pftree-3.4.2/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-07-10 22:33:41.007049 pftree-3.4.2/pftree/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      123 2022-10-05 20:59:00.000000 pftree-3.4.2/pftree/__init__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    21572 2022-10-19 13:21:51.000000 pftree-3.4.2/pftree/__main__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    60625 2023-07-10 22:30:50.000000 pftree-3.4.2/pftree/pftree.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-07-10 22:33:41.008049 pftree-3.4.2/pftree.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      293 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       48 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-09-30 16:51:07.000000 pftree-3.4.2/pftree.egg-info/not-zip-safe
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        7 2023-07-10 22:33:40.000000 pftree-3.4.2/pftree.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-07-10 22:33:41.008049 pftree-3.4.2/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      901 2023-07-10 22:31:32.000000 pftree-3.4.2/setup.py
```

### Comparing `pftree-3.4.0/LICENSE` & `pftree-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pftree-3.4.0/PKG-INFO` & `pftree-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pftree
-Version: 3.4.0
+Version: 3.4.2
 Summary: Utility to create dict representations of file system trees.
 Home-page: https://github.com/FNNDSC/pftree
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 License-File: LICENSE
```

### Comparing `pftree-3.4.0/README.rst` & `pftree-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pftree-3.4.0/pftree/__main__.py` & `pftree-3.4.2/pftree/__main__.py`

 * *Files identical despite different names*

### Comparing `pftree-3.4.0/pftree/pftree.py` & `pftree-3.4.2/pftree/pftree.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,22 +501,22 @@
             l_range     = tqdm(l_files, desc = ' Constructing tree')
         else:
             l_range     = l_files
         for l_series in l_range:
             if len(l_series):
                 str_path    = os.path.dirname(l_series[0])
                 l_series    = [ os.path.basename(i) for i in l_series]
-            # self.simpleProgress_show(index, total)
-            self.d_inputTree[str_path]  = l_series
-            if fn_constructCallback:
-                kwargs['path']          = str_path
-                d_constructCallback     = fn_constructCallback(l_series, **kwargs)
-                self.d_inputTreeCallback[str_path]  = d_constructCallback
-            self.d_outputTree[str_path] = ""
-            index += 1
+                # self.simpleProgress_show(index, total)
+                self.d_inputTree[str_path]  = l_series
+                if fn_constructCallback:
+                    kwargs['path']          = str_path
+                    d_constructCallback     = fn_constructCallback(l_series, **kwargs)
+                    self.d_inputTreeCallback[str_path]  = d_constructCallback
+                self.d_outputTree[str_path] = ""
+                index += 1
         return {
             'status':                   True,
             'd_constructCallback':      d_constructCallback,
             'totalNumberOfAllSeries':   index,
             'd_probe':                  d_probe
         }
```

### Comparing `pftree-3.4.0/pftree.egg-info/PKG-INFO` & `pftree-3.4.2/pftree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pftree
-Version: 3.4.0
+Version: 3.4.2
 Summary: Utility to create dict representations of file system trees.
 Home-page: https://github.com/FNNDSC/pftree
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 License-File: LICENSE
```

### Comparing `pftree-3.4.0/setup.py` & `pftree-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
       name             =   'pftree',
-      version          =   '3.4.0',
+      version          =   '3.4.2',
       description      =   'Utility to create dict representations of file system trees.',
       long_description =   readme(),
       author           =   'FNNDSC',
       author_email     =   'dev@babymri.org',
       url              =   'https://github.com/FNNDSC/pftree',
       packages         =   ['pftree'],
       install_requires =   ['tqdm', 'pfmisc', 'pudb'],
```

