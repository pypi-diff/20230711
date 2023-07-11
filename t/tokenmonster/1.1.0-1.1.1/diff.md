# Comparing `tmp/tokenmonster-1.1.0.tar.gz` & `tmp/tokenmonster-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.0.tar", last modified: Mon Jul 10 16:12:50 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.1.tar", last modified: Tue Jul 11 07:32:06 2023, max compression
```

## Comparing `tokenmonster-1.1.0.tar` & `tokenmonster-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/
--rw-r--r--   0 root         (0) root         (0)    16110 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16356 2023-07-10 10:36:05.000000 tokenmonster-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 16:12:50.975208 tokenmonster-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-10 16:12:00.000000 tokenmonster-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:12:50.971208 tokenmonster-1.1.0/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16110 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 16:12:50.000000 tokenmonster-1.1.0/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    46197 2023-07-10 10:29:36.000000 tokenmonster-1.1.0/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:32:06.077788 tokenmonster-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)    16110 2023-07-11 07:32:06.077788 tokenmonster-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-07-10 10:36:05.000000 tokenmonster-1.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 07:32:06.077788 tokenmonster-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-11 07:31:44.000000 tokenmonster-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:32:06.077788 tokenmonster-1.1.1/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16110 2023-07-11 07:32:06.000000 tokenmonster-1.1.1/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-11 07:32:06.000000 tokenmonster-1.1.1/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:32:06.000000 tokenmonster-1.1.1/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 07:32:06.000000 tokenmonster-1.1.1/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    46261 2023-07-11 07:28:27.000000 tokenmonster-1.1.1/tokenmonster.py
```

### Comparing `tokenmonster-1.1.0/PKG-INFO` & `tokenmonster-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.0/README.md` & `tokenmonster-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tokenmonster-1.1.0/setup.py` & `tokenmonster-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.0',
+    version='1.1.1',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.0/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.1/tokenmonster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.0/tokenmonster.py` & `tokenmonster-1.1.1/tokenmonster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1095,20 +1095,22 @@
     _process = None
     _vocabs = []
 
 
 ### Helper Functions
 
 def _is_prebuilt(name):
+    if name == "gpt2" or name == "llama":
+        return True
     parts = name.split("-")
     if len(parts) < 4 or len(parts) > 5:
         return False
     if not parts[0] in ["english", "code", "fiction", "englishcode"]:
         return False
-    if not parts[1] in ["1000", "2000", "4000", "8000", "12000", "16000", "24000", "32000", "40000", "50256", "65536", "100256"]:
+    if not parts[1] in ["1024", "2048", "4096", "8000", "12000", "16000", "24000", "32000", "40000", "50256", "65536", "100256"]:
         return False
     if not parts[2] in ["unfiltered", "clean", "balanced", "consistent", "strict"]:
         return False
     if len(parts) == 4:
         if len(parts[3]) == 0:
             return False
         if parts[3][0] == 'v':
```

