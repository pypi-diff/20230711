# Comparing `tmp/SmartHackerTools-0.1.tar.gz` & `tmp/SmartHackerTools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartHackerTools-0.1.tar", last modified: Sat May 27 13:08:04 2023, max compression
+gzip compressed data, was "SmartHackerTools-0.1.1.tar", last modified: Tue Jul 11 19:39:18 2023, max compression
```

## Comparing `SmartHackerTools-0.1.tar` & `SmartHackerTools-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 13:08:04.897734 SmartHackerTools-0.1/
--rw-rw-rw-   0        0        0     1056 2023-05-27 13:08:04.897734 SmartHackerTools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-05-27 12:40:08.000000 SmartHackerTools-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 13:08:04.890412 SmartHackerTools-0.1/SmartHackerTools/
--rw-rw-rw-   0        0        0       33 2023-05-27 12:14:33.000000 SmartHackerTools-0.1/SmartHackerTools/__init__.py
--rw-rw-rw-   0        0        0       33 2023-05-27 12:15:00.000000 SmartHackerTools-0.1/SmartHackerTools/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:08:04.896809 SmartHackerTools-0.1/SmartHackerTools.egg-info/
--rw-rw-rw-   0        0        0     1056 2023-05-27 13:08:04.000000 SmartHackerTools-0.1/SmartHackerTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-27 13:08:04.000000 SmartHackerTools-0.1/SmartHackerTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:08:04.000000 SmartHackerTools-0.1/SmartHackerTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-27 13:08:04.000000 SmartHackerTools-0.1/SmartHackerTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-27 13:08:04.000000 SmartHackerTools-0.1/SmartHackerTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-27 12:40:49.000000 SmartHackerTools-0.1/license.txt
--rw-rw-rw-   0        0        0       86 2023-05-27 13:08:04.898303 SmartHackerTools-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1950 2023-05-27 12:42:09.000000 SmartHackerTools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:39:18.101041 SmartHackerTools-0.1.1/
+-rw-rw-rw-   0        0        0     1058 2023-07-11 19:39:18.101041 SmartHackerTools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-05-27 12:40:08.000000 SmartHackerTools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:39:18.096263 SmartHackerTools-0.1.1/SmartHackerTools/
+-rw-rw-rw-   0        0        0       33 2023-05-27 12:14:33.000000 SmartHackerTools-0.1.1/SmartHackerTools/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-11 19:07:36.000000 SmartHackerTools-0.1.1/SmartHackerTools/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:39:18.100033 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/
+-rw-rw-rw-   0        0        0     1058 2023-07-11 19:39:17.000000 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-11 19:39:18.000000 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:39:17.000000 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 19:39:17.000000 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 19:39:17.000000 SmartHackerTools-0.1.1/SmartHackerTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-27 12:40:49.000000 SmartHackerTools-0.1.1/license.txt
+-rw-rw-rw-   0        0        0       86 2023-07-11 19:39:18.102037 SmartHackerTools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1933 2023-07-11 19:33:52.000000 SmartHackerTools-0.1.1/setup.py
```

### Comparing `SmartHackerTools-0.1/PKG-INFO` & `SmartHackerTools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartHackerTools
-Version: 0.1
+Version: 0.1.1
 Summary: These contain some smart hacker tools!
 Home-page: https://github.com/IndentationOrELSE
 Download-URL: https://github.com/IndentationOrELSE/SmartHackerTools/archive/refs/tags/v_01.tar.gz
 Author: Smart_Hacker
 Author-email: sarthakmishra2100@gmail.com
 License: MIT
 Keywords: Tools,Simple,Beginner
```

### Comparing `SmartHackerTools-0.1/SmartHackerTools.egg-info/PKG-INFO` & `SmartHackerTools-0.1.1/SmartHackerTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartHackerTools
-Version: 0.1
+Version: 0.1.1
 Summary: These contain some smart hacker tools!
 Home-page: https://github.com/IndentationOrELSE
 Download-URL: https://github.com/IndentationOrELSE/SmartHackerTools/archive/refs/tags/v_01.tar.gz
 Author: Smart_Hacker
 Author-email: sarthakmishra2100@gmail.com
 License: MIT
 Keywords: Tools,Simple,Beginner
```

### Comparing `SmartHackerTools-0.1/license.txt` & `SmartHackerTools-0.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `SmartHackerTools-0.1/setup.py` & `SmartHackerTools-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from distutils.core import setup
 setup(
   name = 'SmartHackerTools',         # How you named your package folder (MyLib)
   packages = ['SmartHackerTools'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'These contain some smart hacker tools!',   # Give a short description about your library
   author = 'Smart_Hacker',                   # Type in your name
   author_email = 'sarthakmishra2100@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/IndentationOrELSE',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/IndentationOrELSE/SmartHackerTools/archive/refs/tags/v_01.tar.gz',    # I explain this later on
   keywords = ['Tools', 'Simple', 'Beginner'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
-          'time',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

