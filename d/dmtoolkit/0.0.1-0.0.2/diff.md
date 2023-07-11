# Comparing `tmp/dmtoolkit-0.0.1.tar.gz` & `tmp/dmtoolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolkit-0.0.1.tar", last modified: Tue Jul 11 14:30:40 2023, max compression
+gzip compressed data, was "dmtoolkit-0.0.2.tar", last modified: Tue Jul 11 18:02:41 2023, max compression
```

## Comparing `dmtoolkit-0.0.1.tar` & `dmtoolkit-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.885089 dmtoolkit-0.0.1/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.1/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3467 2023-07-11 14:30:40.885089 dmtoolkit-0.0.1/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1759 2023-06-22 17:38:40.000000 dmtoolkit-0.0.1/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1224 2023-07-11 13:42:13.000000 dmtoolkit-0.0.1/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.1/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-11 14:30:40.885089 dmtoolkit-0.0.1/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.1/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.882089 dmtoolkit-0.0.1/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.883089 dmtoolkit-0.0.1/src/dmtoolkit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       55 2023-07-11 13:33:10.000000 dmtoolkit-0.0.1/src/dmtoolkit/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.884090 dmtoolkit-0.0.1/src/dmtoolkit/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.1/src/dmtoolkit/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.1/src/dmtoolkit/apis/dndbeyondapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.1/src/dmtoolkit/apis/foundryapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5806 2023-07-11 12:55:44.000000 dmtoolkit-0.0.1/src/dmtoolkit/apis/open5eapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.1/src/dmtoolkit/apis/wikijsapi.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.884090 dmtoolkit-0.0.1/src/dmtoolkit/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-06-20 14:20:28.000000 dmtoolkit-0.0.1/src/dmtoolkit/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      293 2023-06-20 21:35:42.000000 dmtoolkit-0.0.1/src/dmtoolkit/db/dndorm.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12563 2023-07-07 15:46:06.000000 dmtoolkit-0.0.1/src/dmtoolkit/dmtoolkit.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.885089 dmtoolkit-0.0.1/src/dmtoolkit/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1932 2023-07-07 15:02:17.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dndcharacter.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      949 2023-07-07 15:28:26.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dnditem.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1808 2023-07-07 16:01:05.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dndmonster.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1519 2023-07-07 14:51:57.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dndobject.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dndshop.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1037 2023-07-07 16:01:33.000000 dmtoolkit-0.0.1/src/dmtoolkit/models/dndspell.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 14:30:40.883089 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3467 2023-07-11 14:30:40.000000 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)      750 2023-07-11 14:30:40.000000 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-11 14:30:40.000000 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-11 14:30:40.000000 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-11 14:30:40.000000 dmtoolkit-0.0.1/src/dmtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.405879 dmtoolkit-0.0.2/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.2/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-11 18:02:41.404879 dmtoolkit-0.0.2/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.2/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1224 2023-07-11 13:42:13.000000 dmtoolkit-0.0.2/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.2/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-11 18:02:41.405879 dmtoolkit-0.0.2/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.2/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.394879 dmtoolkit-0.0.2/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.398879 dmtoolkit-0.0.2/src/dmtoolkit/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-11 18:02:19.000000 dmtoolkit-0.0.2/src/dmtoolkit/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.400879 dmtoolkit-0.0.2/src/dmtoolkit/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/dndbeyondapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/foundryapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     5806 2023-07-11 12:55:44.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/open5eapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/wikijsapi.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.401879 dmtoolkit-0.0.2/src/dmtoolkit/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-06-20 14:20:28.000000 dmtoolkit-0.0.2/src/dmtoolkit/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      293 2023-06-20 21:35:42.000000 dmtoolkit-0.0.2/src/dmtoolkit/db/dndorm.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12561 2023-07-11 18:01:51.000000 dmtoolkit-0.0.2/src/dmtoolkit/dmtools.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.403879 dmtoolkit-0.0.2/src/dmtoolkit/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1932 2023-07-07 15:02:17.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndcharacter.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      949 2023-07-07 15:28:26.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dnditem.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1808 2023-07-07 16:01:05.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndmonster.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1519 2023-07-07 14:51:57.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndobject.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndshop.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1037 2023-07-07 16:01:33.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndspell.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.399879 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      748 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/top_level.txt
```

### Comparing `dmtoolkit-0.0.1/LICENSE` & `dmtoolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/PKG-INFO` & `dmtoolkit-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,16 +94,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 
 ### Issue Tracking
 
 - None
```

### Comparing `dmtoolkit-0.0.1/README.md` & `dmtoolkit-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 
 ### Issue Tracking
 
 - None
```

### Comparing `dmtoolkit-0.0.1/pyproject.toml` & `dmtoolkit-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/setup.py` & `dmtoolkit-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/apis/dndbeyondapi.py` & `dmtoolkit-0.0.2/src/dmtoolkit/apis/dndbeyondapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/apis/open5eapi.py` & `dmtoolkit-0.0.2/src/dmtoolkit/apis/open5eapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/apis/wikijsapi.py` & `dmtoolkit-0.0.2/src/dmtoolkit/apis/wikijsapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/dmtoolkit.py` & `dmtoolkit-0.0.2/src/dmtoolkit/dmtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from models import Monster
 from models import Item
 from models import Spell
 from models import Character
 from models import Shop
 
 
-class DMToolkit:
+class DMTools:
     """
     _summary_
 
     Returns:
         _type_: _description_
     """
```

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dndcharacter.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dndcharacter.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dnditem.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dnditem.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dndmonster.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dndmonster.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dndobject.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dndobject.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dndshop.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dndshop.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit/models/dndspell.py` & `dmtoolkit-0.0.2/src/dmtoolkit/models/dndspell.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit.egg-info/PKG-INFO` & `dmtoolkit-0.0.2/src/dmtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,16 +94,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 
 ### Issue Tracking
 
 - None
```

### Comparing `dmtoolkit-0.0.1/src/dmtoolkit.egg-info/SOURCES.txt` & `dmtoolkit-0.0.2/src/dmtoolkit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 src/dmtoolkit/__init__.py
-src/dmtoolkit/dmtoolkit.py
+src/dmtoolkit/dmtools.py
 src/dmtoolkit.egg-info/PKG-INFO
 src/dmtoolkit.egg-info/SOURCES.txt
 src/dmtoolkit.egg-info/dependency_links.txt
 src/dmtoolkit.egg-info/requires.txt
 src/dmtoolkit.egg-info/top_level.txt
 src/dmtoolkit/apis/__init__.py
 src/dmtoolkit/apis/dndbeyondapi.py
```

