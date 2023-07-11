# Comparing `tmp/clera-0.1.0.tar.gz` & `tmp/clera-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.1.0.tar", last modified: Tue Jul 11 00:33:43 2023, max compression
+gzip compressed data, was "clera-0.1.1.tar", last modified: Tue Jul 11 01:05:44 2023, max compression
```

## Comparing `clera-0.1.0.tar` & `clera-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,42 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.433447 clera-0.1.0/
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1550 2023-07-11 00:15:16.000000 clera-0.1.0/CHANGELOG.md
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.1.0/LICENCE.txt
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       48 2023-07-04 11:33:56.000000 clera-0.1.0/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3467 2023-07-11 00:33:43.433447 clera-0.1.0/PKG-INFO
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1279 2023-07-08 18:13:25.000000 clera-0.1.0/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.389447 clera-0.1.0/clera/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      194 2023-07-11 00:18:50.000000 clera-0.1.0/clera/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    61327 2023-07-09 14:12:05.000000 clera-0.1.0/clera/core.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.425447 clera-0.1.0/clera/icons/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       65 2023-07-04 11:49:49.000000 clera-0.1.0/clera/icons/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16293 2023-06-19 11:40:22.000000 clera-0.1.0/clera/icons/add-file.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13782 2023-06-19 03:37:40.000000 clera-0.1.0/clera/icons/close.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13430 2023-06-19 11:40:48.000000 clera-0.1.0/clera/icons/document.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16420 2023-06-19 03:41:00.000000 clera-0.1.0/clera/icons/documents.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15098 2023-06-19 03:38:16.000000 clera-0.1.0/clera/icons/gear.png
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.1.0/clera/icons/hand-drawn-icon.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13536 2023-06-19 03:36:08.000000 clera-0.1.0/clera/icons/off.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    14518 2023-06-19 03:36:42.000000 clera-0.1.0/clera/icons/on.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15585 2023-06-19 03:38:52.000000 clera-0.1.0/clera/icons/save-as.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13421 2023-06-19 03:38:40.000000 clera-0.1.0/clera/icons/save.png
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.1.0/clera/icons/toon-icon.ico
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.425447 clera-0.1.0/clera/scripts/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16531 2023-07-11 00:26:54.000000 clera-0.1.0/clera/scripts/editor.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.429447 clera-0.1.0/clera/stubs/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-03 14:47:26.000000 clera-0.1.0/clera/stubs/__init__.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    11965 2023-07-04 17:11:17.000000 clera-0.1.0/clera/stubs/core.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1176 2023-07-11 00:25:50.000000 clera-0.1.0/clera/stubs/handlers.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7669 2023-07-08 14:35:34.000000 clera-0.1.0/clera/stubs/widgets.pyi
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.433447 clera-0.1.0/clera/utils/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      120 2023-07-04 11:49:58.000000 clera-0.1.0/clera/utils/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.1.0/clera/utils/exceptions.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    19722 2023-07-05 13:58:59.000000 clera-0.1.0/clera/utils/handlers.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.1.0/clera/utils/keys.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.1.0/clera/utils/procr.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.1.0/clera/utils/style.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27822 2023-07-09 13:18:50.000000 clera-0.1.0/clera/widgets.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.389447 clera-0.1.0/clera.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3467 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      820 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       46 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-11 00:33:43.433447 clera-0.1.0/setup.cfg
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1340 2023-07-11 00:24:55.000000 clera-0.1.0/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.432115 clera-0.1.1/
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1622 2023-07-11 00:59:12.000000 clera-0.1.1/CHANGELOG.md
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.1.1/LICENCE.txt
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       42 2023-07-11 00:59:20.000000 clera-0.1.1/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3539 2023-07-11 01:05:44.432115 clera-0.1.1/PKG-INFO
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1279 2023-07-08 18:13:25.000000 clera-0.1.1/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.416115 clera-0.1.1/clera/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-11 01:01:47.000000 clera-0.1.1/clera/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    61327 2023-07-11 01:03:32.000000 clera-0.1.1/clera/core.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.428115 clera-0.1.1/clera/icons/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       65 2023-07-04 11:49:49.000000 clera-0.1.1/clera/icons/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16293 2023-06-19 11:40:22.000000 clera-0.1.1/clera/icons/add-file.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13782 2023-06-19 03:37:40.000000 clera-0.1.1/clera/icons/close.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13430 2023-06-19 11:40:48.000000 clera-0.1.1/clera/icons/document.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16420 2023-06-19 03:41:00.000000 clera-0.1.1/clera/icons/documents.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15098 2023-06-19 03:38:16.000000 clera-0.1.1/clera/icons/gear.png
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.1.1/clera/icons/hand-drawn-icon.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13536 2023-06-19 03:36:08.000000 clera-0.1.1/clera/icons/off.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    14518 2023-06-19 03:36:42.000000 clera-0.1.1/clera/icons/on.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15585 2023-06-19 03:38:52.000000 clera-0.1.1/clera/icons/save-as.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13421 2023-06-19 03:38:40.000000 clera-0.1.1/clera/icons/save.png
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.1.1/clera/icons/toon-icon.ico
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.428115 clera-0.1.1/clera/scripts/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       21 2023-07-11 01:02:09.000000 clera-0.1.1/clera/scripts/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16531 2023-07-11 00:26:54.000000 clera-0.1.1/clera/scripts/editor.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.432115 clera-0.1.1/clera/utils/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      120 2023-07-04 11:49:58.000000 clera-0.1.1/clera/utils/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.1.1/clera/utils/exceptions.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    19722 2023-07-05 13:58:59.000000 clera-0.1.1/clera/utils/handlers.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.1.1/clera/utils/keys.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.1.1/clera/utils/procr.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.1.1/clera/utils/style.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27822 2023-07-09 13:18:50.000000 clera-0.1.1/clera/widgets.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.420115 clera-0.1.1/clera.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3539 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      751 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       46 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-11 01:05:44.432115 clera-0.1.1/setup.cfg
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1340 2023-07-11 00:58:31.000000 clera-0.1.1/setup.py
```

### Comparing `clera-0.1.0/CHANGELOG.md` & `clera-0.1.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,11 @@
 > [ CHANGED ]  
 > [+] sizepolicy declaration
 >
 > [ FIXED ]  
 > [+] ModuleNotFoundError: No module named 'clera.stubs'  
 > [+] Window icon display  
 > [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
+
+> **0.1.1** -- [ 11 JULY 2023 ]  
+> [ NOTICE ]  
+> [+] Minor Fixes
```

### Comparing `clera-0.1.0/LICENCE.txt` & `clera-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/PKG-INFO` & `clera-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.1.0
+Version: 0.1.1
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: gui,clera,simple,simplegui,pyside,pyside6,python,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -143,7 +143,11 @@
 > [ CHANGED ]  
 > [+] sizepolicy declaration
 >
 > [ FIXED ]  
 > [+] ModuleNotFoundError: No module named 'clera.stubs'  
 > [+] Window icon display  
 > [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
+
+> **0.1.1** -- [ 11 JULY 2023 ]  
+> [ NOTICE ]  
+> [+] Minor Fixes
```

### Comparing `clera-0.1.0/README.md` & `clera-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/core.py` & `clera-0.1.1/clera/core.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/add-file.png` & `clera-0.1.1/clera/icons/add-file.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/close.png` & `clera-0.1.1/clera/icons/close.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/document.png` & `clera-0.1.1/clera/icons/document.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/documents.png` & `clera-0.1.1/clera/icons/documents.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/gear.png` & `clera-0.1.1/clera/icons/gear.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/hand-drawn-icon.png` & `clera-0.1.1/clera/icons/hand-drawn-icon.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/off.png` & `clera-0.1.1/clera/icons/off.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/on.png` & `clera-0.1.1/clera/icons/on.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/save-as.png` & `clera-0.1.1/clera/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/save.png` & `clera-0.1.1/clera/icons/save.png`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/icons/toon-icon.ico` & `clera-0.1.1/clera/icons/toon-icon.ico`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/scripts/editor.py` & `clera-0.1.1/clera/scripts/editor.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/utils/handlers.py` & `clera-0.1.1/clera/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/utils/keys.py` & `clera-0.1.1/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/utils/procr.py` & `clera-0.1.1/clera/utils/procr.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/utils/style.py` & `clera-0.1.1/clera/utils/style.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera/widgets.py` & `clera-0.1.1/clera/widgets.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.0/clera.egg-info/PKG-INFO` & `clera-0.1.1/clera.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.1.0
+Version: 0.1.1
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: gui,clera,simple,simplegui,pyside,pyside6,python,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -143,7 +143,11 @@
 > [ CHANGED ]  
 > [+] sizepolicy declaration
 >
 > [ FIXED ]  
 > [+] ModuleNotFoundError: No module named 'clera.stubs'  
 > [+] Window icon display  
 > [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
+
+> **0.1.1** -- [ 11 JULY 2023 ]  
+> [ NOTICE ]  
+> [+] Minor Fixes
```

### Comparing `clera-0.1.0/clera.egg-info/SOURCES.txt` & `clera-0.1.1/clera.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 clera/icons/gear.png
 clera/icons/hand-drawn-icon.png
 clera/icons/off.png
 clera/icons/on.png
 clera/icons/save-as.png
 clera/icons/save.png
 clera/icons/toon-icon.ico
+clera/scripts/__init__.py
 clera/scripts/editor.py
-clera/stubs/__init__.pyi
-clera/stubs/core.pyi
-clera/stubs/handlers.pyi
-clera/stubs/widgets.pyi
 clera/utils/__init__.py
 clera/utils/exceptions.py
 clera/utils/handlers.py
 clera/utils/keys.py
 clera/utils/procr.py
 clera/utils/style.py
```

### Comparing `clera-0.1.0/setup.py` & `clera-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Write Simple and Quick Python GUI Application'
 KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6', 'python', 'easy']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

