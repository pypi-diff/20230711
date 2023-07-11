# Comparing `tmp/DQR_Data-0.1.tar.gz` & `tmp/DQR_Data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DQR_Data-0.1.tar", last modified: Tue Jul 11 13:54:23 2023, max compression
+gzip compressed data, was "DQR_Data-0.1.1.tar", last modified: Tue Jul 11 14:29:29 2023, max compression
```

## Comparing `DQR_Data-0.1.tar` & `DQR_Data-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:54:23.112061 DQR_Data-0.1/
-drwxrwxrwx   0        0        0        0 2023-07-11 13:54:23.071059 DQR_Data-0.1/DQR_Data/
--rw-rw-rw-   0        0        0       34 2023-07-11 10:38:04.000000 DQR_Data-0.1/DQR_Data/__init__.py
--rw-rw-rw-   0        0        0      294 2023-07-11 10:38:04.000000 DQR_Data-0.1/DQR_Data/example.py
--rw-rw-rw-   0        0        0      548 2023-07-11 10:38:04.000000 DQR_Data-0.1/DQR_Data/main.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:54:23.107813 DQR_Data-0.1/DQR_Data.egg-info/
--rw-rw-rw-   0        0        0      194 2023-07-11 13:54:22.000000 DQR_Data-0.1/DQR_Data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-11 13:54:22.000000 DQR_Data-0.1/DQR_Data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:54:22.000000 DQR_Data-0.1/DQR_Data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-11 13:54:22.000000 DQR_Data-0.1/DQR_Data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 13:54:22.000000 DQR_Data-0.1/DQR_Data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      194 2023-07-11 13:54:23.108975 DQR_Data-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-11 13:54:23.113597 DQR_Data-0.1/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-07-11 10:38:04.000000 DQR_Data-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:29:29.301055 DQR_Data-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-11 14:29:29.209678 DQR_Data-0.1.1/DQR_Data/
+-rw-rw-rw-   0        0        0       34 2023-07-11 10:38:04.000000 DQR_Data-0.1.1/DQR_Data/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-07-11 10:38:04.000000 DQR_Data-0.1.1/DQR_Data/example.py
+-rw-rw-rw-   0        0        0      548 2023-07-11 10:38:04.000000 DQR_Data-0.1.1/DQR_Data/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:29:29.298242 DQR_Data-0.1.1/DQR_Data.egg-info/
+-rw-rw-rw-   0        0        0     5861 2023-07-11 14:29:28.000000 DQR_Data-0.1.1/DQR_Data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-11 14:29:28.000000 DQR_Data-0.1.1/DQR_Data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:29:28.000000 DQR_Data-0.1.1/DQR_Data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-11 14:29:28.000000 DQR_Data-0.1.1/DQR_Data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 14:29:28.000000 DQR_Data-0.1.1/DQR_Data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5861 2023-07-11 14:29:29.301055 DQR_Data-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-07-11 14:29:29.304924 DQR_Data-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      775 2023-07-11 14:27:43.000000 DQR_Data-0.1.1/setup.py
```

### Comparing `DQR_Data-0.1/DQR_Data/main.py` & `DQR_Data-0.1.1/DQR_Data/main.py`

 * *Files identical despite different names*

