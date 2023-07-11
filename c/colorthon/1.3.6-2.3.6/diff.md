# Comparing `tmp/Colorthon-1.3.6.tar.gz` & `tmp/colorthon-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Colorthon-1.3.6.tar", last modified: Mon Jul 10 04:29:29 2023, max compression
+gzip compressed data, was "colorthon-2.3.6.tar", last modified: Tue Jul 11 19:44:55 2023, max compression
```

## Comparing `Colorthon-1.3.6.tar` & `colorthon-2.3.6.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-10 04:29:29.694775 Colorthon-1.3.6/
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-10 04:29:29.694269 Colorthon-1.3.6/Colorthon.egg-info/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     1352 2023-07-10 04:29:29.000000 Colorthon-1.3.6/Colorthon.egg-info/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      209 2023-07-10 04:29:29.000000 Colorthon-1.3.6/Colorthon.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-10 04:29:29.000000 Colorthon-1.3.6/Colorthon.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-10 04:29:29.000000 Colorthon-1.3.6/Colorthon.egg-info/top_level.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     1352 2023-07-10 04:29:29.694693 Colorthon-1.3.6/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      774 2023-07-10 04:24:49.000000 Colorthon-1.3.6/README.md
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-10 04:29:29.694547 Colorthon-1.3.6/colorthon/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      264 2023-07-10 03:27:37.000000 Colorthon-1.3.6/colorthon/Text.py
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      738 2023-07-10 04:10:22.000000 Colorthon-1.3.6/colorthon/__init__.py
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      228 2023-07-10 03:16:17.000000 Colorthon-1.3.6/colorthon/utils.py
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-10 04:29:29.694805 Colorthon-1.3.6/setup.cfg
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)      906 2023-07-10 04:05:02.000000 Colorthon-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:44:55.234666 colorthon-2.3.6/
+-rw-rw-rw-   0        0        0     3025 2023-07-11 19:44:55.234666 colorthon-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2330 2023-07-11 19:38:35.000000 colorthon-2.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:44:55.234666 colorthon-2.3.6/colorthon.egg-info/
+-rw-rw-rw-   0        0        0     3025 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 19:44:55.234666 colorthon-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-07-11 19:43:58.000000 colorthon-2.3.6/setup.py
```

