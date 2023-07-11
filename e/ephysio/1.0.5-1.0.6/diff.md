# Comparing `tmp/ephysio-1.0.5.tar.gz` & `tmp/ephysio-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysio-1.0.5.tar", last modified: Mon Jul 10 02:13:29 2023, max compression
+gzip compressed data, was "ephysio-1.0.6.tar", last modified: Tue Jul 11 20:58:21 2023, max compression
```

## Comparing `ephysio-1.0.5.tar` & `ephysio-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 02:13:29.360564 ephysio-1.0.5/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.5/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 02:13:29.360564 ephysio-1.0.5/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.5/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 02:13:29.360564 ephysio-1.0.5/ephysio/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.5/ephysio/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.5/ephysio/kilosortIO.py
--rw-------   0 wagenaar  (1000) wagenaar  (1000)    58904 2023-07-10 01:01:39.000000 ephysio-1.0.5/ephysio/openEphysIO.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6370 2023-07-10 01:06:33.000000 ephysio-1.0.5/ephysio/spikestats.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.5/ephysio/vizio.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 02:13:29.360564 ephysio-1.0.5/ephysio.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 02:13:29.000000 ephysio-1.0.5/ephysio.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      290 2023-07-10 02:13:29.000000 ephysio-1.0.5/ephysio.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-10 02:13:29.000000 ephysio-1.0.5/ephysio.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-10 02:13:29.000000 ephysio-1.0.5/ephysio.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-10 02:13:29.000000 ephysio-1.0.5/ephysio.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-10 02:12:52.000000 ephysio-1.0.5/pyproject.toml
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-10 02:13:29.360564 ephysio-1.0.5/setup.cfg
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.292050 ephysio-1.0.6/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.6/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-11 20:58:21.292050 ephysio-1.0.6/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.6/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.288050 ephysio-1.0.6/ephysio/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.6/ephysio/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.6/ephysio/kilosortIO.py
+-rw-------   0 wagenaar  (1000) wagenaar  (1000)    58904 2023-07-10 01:01:39.000000 ephysio-1.0.6/ephysio/openEphysIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6370 2023-07-10 01:06:33.000000 ephysio-1.0.6/ephysio/spikestats.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.6/ephysio/vizio.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6897 2023-07-10 20:43:28.000000 ephysio-1.0.6/ephysio/vizly.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.292050 ephysio-1.0.6/ephysio.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      307 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-11 20:58:13.000000 ephysio-1.0.6/pyproject.toml
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-11 20:58:21.292050 ephysio-1.0.6/setup.cfg
```

### Comparing `ephysio-1.0.5/LICENSE` & `ephysio-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/PKG-INFO` & `ephysio-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

### Comparing `ephysio-1.0.5/README.md` & `ephysio-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/ephysio/kilosortIO.py` & `ephysio-1.0.6/ephysio/kilosortIO.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/ephysio/openEphysIO.py` & `ephysio-1.0.6/ephysio/openEphysIO.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/ephysio/spikestats.py` & `ephysio-1.0.6/ephysio/spikestats.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/ephysio/vizio.py` & `ephysio-1.0.6/ephysio/vizio.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.5/ephysio.egg-info/PKG-INFO` & `ephysio-1.0.6/ephysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

