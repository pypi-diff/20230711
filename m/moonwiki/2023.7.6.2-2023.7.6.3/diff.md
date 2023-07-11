# Comparing `tmp/moonwiki-2023.7.6.2.tar.gz` & `tmp/moonwiki-2023.7.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonwiki-2023.7.6.2.tar", last modified: Thu Jul  6 08:08:23 2023, max compression
+gzip compressed data, was "moonwiki-2023.7.6.3.tar", last modified: Thu Jul  6 08:33:51 2023, max compression
```

## Comparing `moonwiki-2023.7.6.2.tar` & `moonwiki-2023.7.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:08:23.948496 moonwiki-2023.7.6.2/
--rw-rw-rw-   0        0        0      899 2023-07-06 08:08:23.948496 moonwiki-2023.7.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-07-06 08:05:27.000000 moonwiki-2023.7.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:08:23.901617 moonwiki-2023.7.6.2/moonwiki/
--rw-rw-rw-   0        0        0      877 2023-07-05 10:33:38.000000 moonwiki-2023.7.6.2/moonwiki/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:08:23.948496 moonwiki-2023.7.6.2/moonwiki.egg-info/
--rw-rw-rw-   0        0        0      899 2023-07-06 08:08:23.000000 moonwiki-2023.7.6.2/moonwiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-07-06 08:08:23.000000 moonwiki-2023.7.6.2/moonwiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:08:23.000000 moonwiki-2023.7.6.2/moonwiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 08:08:23.000000 moonwiki-2023.7.6.2/moonwiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 08:08:23.948496 moonwiki-2023.7.6.2/setup.cfg
--rw-rw-rw-   0        0        0      412 2023-07-06 08:08:13.000000 moonwiki-2023.7.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:51.257772 moonwiki-2023.7.6.3/
+-rw-rw-rw-   0        0        0      899 2023-07-06 08:33:51.257772 moonwiki-2023.7.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-07-06 08:05:27.000000 moonwiki-2023.7.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:51.195271 moonwiki-2023.7.6.3/moonwiki/
+-rw-rw-rw-   0        0        0      995 2023-07-06 08:33:28.000000 moonwiki-2023.7.6.3/moonwiki/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:51.242148 moonwiki-2023.7.6.3/moonwiki.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-07-06 08:33:50.000000 moonwiki-2023.7.6.3/moonwiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-07-06 08:33:51.000000 moonwiki-2023.7.6.3/moonwiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:33:50.000000 moonwiki-2023.7.6.3/moonwiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 08:33:50.000000 moonwiki-2023.7.6.3/moonwiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:33:51.257772 moonwiki-2023.7.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-07-06 08:33:44.000000 moonwiki-2023.7.6.3/setup.py
```

### Comparing `moonwiki-2023.7.6.2/PKG-INFO` & `moonwiki-2023.7.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonwiki
-Version: 2023.7.6.2
+Version: 2023.7.6.3
 Summary: moonwiki is a wiki application made with Python
 Home-page: https://github.com/RixTheTyrunt/moonwiki
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `moonwiki-2023.7.6.2/README.md` & `moonwiki-2023.7.6.3/README.md`

 * *Files identical despite different names*

### Comparing `moonwiki-2023.7.6.2/moonwiki.egg-info/PKG-INFO` & `moonwiki-2023.7.6.3/moonwiki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonwiki
-Version: 2023.7.6.2
+Version: 2023.7.6.3
 Summary: moonwiki is a wiki application made with Python
 Home-page: https://github.com/RixTheTyrunt/moonwiki
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

