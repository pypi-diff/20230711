# Comparing `tmp/postgreslite-0.0.2.tar.gz` & `tmp/postgreslite-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgreslite-0.0.2.tar", last modified: Fri Dec 30 23:59:25 2022, max compression
+gzip compressed data, was "postgreslite-0.0.3.tar", last modified: Tue Jul 11 18:19:20 2023, max compression
```

## Comparing `postgreslite-0.0.2.tar` & `postgreslite-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-30 23:59:25.172560 postgreslite-0.0.2/
--rw-rw-rw-   0        0        0     1090 2022-12-30 22:00:06.000000 postgreslite-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      179 2022-12-30 23:59:25.172560 postgreslite-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      191 2022-12-30 22:42:35.000000 postgreslite-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-30 23:59:25.157010 postgreslite-0.0.2/postgreslite/
--rw-rw-rw-   0        0        0       60 2022-12-30 23:59:10.000000 postgreslite-0.0.2/postgreslite/__init__.py
--rw-rw-rw-   0        0        0     3481 2022-12-30 23:53:16.000000 postgreslite-0.0.2/postgreslite/handler.py
-drwxrwxrwx   0        0        0        0 2022-12-30 23:59:25.171158 postgreslite-0.0.2/postgreslite.egg-info/
--rw-rw-rw-   0        0        0      179 2022-12-30 23:59:25.000000 postgreslite-0.0.2/postgreslite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2022-12-30 23:59:25.000000 postgreslite-0.0.2/postgreslite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-30 23:59:25.000000 postgreslite-0.0.2/postgreslite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-12-30 23:59:25.000000 postgreslite-0.0.2/postgreslite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-30 23:59:25.172560 postgreslite-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      446 2022-12-30 22:37:07.000000 postgreslite-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:19:20.471816 postgreslite-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-07-11 18:19:20.471310 postgreslite-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 18:19:20.465773 postgreslite-0.0.3/postgreslite/
+-rw-rw-rw-   0        0        0       72 2023-07-11 18:16:40.000000 postgreslite-0.0.3/postgreslite/__init__.py
+-rw-rw-rw-   0        0        0     2354 2023-07-11 18:18:04.000000 postgreslite-0.0.3/postgreslite/handler.py
+-rw-rw-rw-   0        0        0     1773 2023-07-11 18:17:57.000000 postgreslite-0.0.3/postgreslite/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:19:20.470305 postgreslite-0.0.3/postgreslite.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-11 18:19:20.000000 postgreslite-0.0.3/postgreslite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-11 18:19:20.000000 postgreslite-0.0.3/postgreslite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:19:20.000000 postgreslite-0.0.3/postgreslite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 18:19:20.000000 postgreslite-0.0.3/postgreslite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:19:20.471816 postgreslite-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.0.3/setup.py
```

### Comparing `postgreslite-0.0.2/LICENSE` & `postgreslite-0.0.3/LICENSE`

 * *Files identical despite different names*

