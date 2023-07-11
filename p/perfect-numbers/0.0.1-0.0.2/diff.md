# Comparing `tmp/perfect_numbers-0.0.1.tar.gz` & `tmp/perfect_numbers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfect_numbers-0.0.1.tar", last modified: Sun Jul  9 14:53:37 2023, max compression
+gzip compressed data, was "perfect_numbers-0.0.2.tar", last modified: Tue Jul 11 04:35:41 2023, max compression
```

## Comparing `perfect_numbers-0.0.1.tar` & `perfect_numbers-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-09 14:53:37.529664 perfect_numbers-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1089 2023-07-09 14:38:58.000000 perfect_numbers-0.0.1/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1038 2023-07-09 14:53:37.529664 perfect_numbers-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-07-09 14:38:58.000000 perfect_numbers-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-09 14:53:37.529664 perfect_numbers-0.0.1/perfect_numbers/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       41 2023-07-09 14:38:58.000000 perfect_numbers-0.0.1/perfect_numbers/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      743 2023-07-09 14:38:58.000000 perfect_numbers-0.0.1/perfect_numbers/perfect_num.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-09 14:53:37.529664 perfect_numbers-0.0.1/perfect_numbers.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1038 2023-07-09 14:53:37.000000 perfect_numbers-0.0.1/perfect_numbers.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      255 2023-07-09 14:53:37.000000 perfect_numbers-0.0.1/perfect_numbers.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-09 14:53:37.000000 perfect_numbers-0.0.1/perfect_numbers.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       16 2023-07-09 14:53:37.000000 perfect_numbers-0.0.1/perfect_numbers.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-07-09 14:53:37.529664 perfect_numbers-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1869 2023-07-09 14:38:58.000000 perfect_numbers-0.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-11 04:35:41.361232 perfect_numbers-0.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1089 2023-07-09 14:38:58.000000 perfect_numbers-0.0.2/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1038 2023-07-11 04:35:41.361232 perfect_numbers-0.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-07-09 14:38:58.000000 perfect_numbers-0.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-11 04:35:41.353232 perfect_numbers-0.0.2/perfect_numbers/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2023-07-11 03:43:28.000000 perfect_numbers-0.0.2/perfect_numbers/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      732 2023-07-11 03:31:35.000000 perfect_numbers-0.0.2/perfect_numbers/perfect_num.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-11 04:35:41.357232 perfect_numbers-0.0.2/perfect_numbers.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1038 2023-07-11 04:35:41.000000 perfect_numbers-0.0.2/perfect_numbers.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      255 2023-07-11 04:35:41.000000 perfect_numbers-0.0.2/perfect_numbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-11 04:35:41.000000 perfect_numbers-0.0.2/perfect_numbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       16 2023-07-11 04:35:41.000000 perfect_numbers-0.0.2/perfect_numbers.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-07-11 04:35:41.361232 perfect_numbers-0.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1869 2023-07-11 04:34:07.000000 perfect_numbers-0.0.2/setup.py
```

### Comparing `perfect_numbers-0.0.1/LICENSE.txt` & `perfect_numbers-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `perfect_numbers-0.0.1/PKG-INFO` & `perfect_numbers-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect_numbers
-Version: 0.0.1
+Version: 0.0.2
 Summary: MODULE IS USE TO FIND PERFECT NUMBER
 Home-page: https://github.com/RETROEAGLE721/perfect_numbers
 Download-URL: https://github.com/RETROEAGLE721/perfect_numbers/archive/refs/tags/0.0.1.tar.gz
 Author: RETROeagle
 Author-email: postviral75@gmail.com
 License: MIT
 Keywords: CUSTOM,MODULE,PERFECT_NUMBER
```

### Comparing `perfect_numbers-0.0.1/perfect_numbers/perfect_num.py` & `perfect_numbers-0.0.2/perfect_numbers/perfect_num.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def check_perfect_number(checknumber:int) -> int:
+def check_perfect_number(checknumber):
     c = []
     if checknumber == 0 or checknumber == 1 or checknumber == 2:
         return False
     for x  in range(1,int(checknumber/2)):
         if checknumber%x == 0:
             c.append(x)
     sums = sum(c)
```

### Comparing `perfect_numbers-0.0.1/perfect_numbers.egg-info/PKG-INFO` & `perfect_numbers-0.0.2/perfect_numbers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-numbers
-Version: 0.0.1
+Version: 0.0.2
 Summary: MODULE IS USE TO FIND PERFECT NUMBER
 Home-page: https://github.com/RETROEAGLE721/perfect_numbers
 Download-URL: https://github.com/RETROEAGLE721/perfect_numbers/archive/refs/tags/0.0.1.tar.gz
 Author: RETROeagle
 Author-email: postviral75@gmail.com
 License: MIT
 Keywords: CUSTOM,MODULE,PERFECT_NUMBER
```

### Comparing `perfect_numbers-0.0.1/setup.py` & `perfect_numbers-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'perfect_numbers',         # How you named your package folder (MyLib)
   packages = ['perfect_numbers'],   # Chose the same as "name"
-  version = '0.0.1',      # Start with a small number and increase it with every change you make
+  version = '0.0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'MODULE IS USE TO FIND PERFECT NUMBER',   # Give a short description about your library
   author = 'RETROeagle',                   # Type in your name
   author_email = 'postviral75@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/RETROEAGLE721/perfect_numbers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/RETROEAGLE721/perfect_numbers/archive/refs/tags/0.0.1.tar.gz',    # I explain this later on
   keywords = ['CUSTOM', 'MODULE', 'PERFECT_NUMBER'],   # Keywords that define your package best
```

