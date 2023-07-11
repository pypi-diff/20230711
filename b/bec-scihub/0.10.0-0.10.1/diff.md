# Comparing `tmp/bec_scihub-0.10.0.tar.gz` & `tmp/bec_scihub-0.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.10.0.tar", last modified: Sat Jul  8 15:34:17 2023, max compression
+gzip compressed data, was "bec_scihub-0.10.1.tar", last modified: Tue Jul 11 09:32:42 2023, max compression
```

## Comparing `bec_scihub-0.10.0.tar` & `bec_scihub-0.10.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:34:17.482508 bec_scihub-0.10.0/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-08 15:34:17.482508 bec_scihub-0.10.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:34:17.482508 bec_scihub-0.10.0/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      521 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 15:34:17.000000 bec_scihub-0.10.0/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:34:17.479508 bec_scihub-0.10.0/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.10.0/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:34:17.480508 bec_scihub-0.10.0/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.10.0/scihub/scibec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scibec/config_handler.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scibec/scibec.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scibec/scibec_connector.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.10.0/scihub/scibec/scibec_validator.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:34:17.480508 bec_scihub-0.10.0/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.10.0/scihub/scilog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.10.0/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-08 15:34:17.482508 bec_scihub-0.10.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-08 15:33:35.000000 bec_scihub-0.10.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:32:42.710058 bec_scihub-0.10.1/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-11 09:32:42.710058 bec_scihub-0.10.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:32:42.710058 bec_scihub-0.10.1/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 09:32:42.000000 bec_scihub-0.10.1/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:32:42.706058 bec_scihub-0.10.1/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.10.1/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:32:42.708058 bec_scihub-0.10.1/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.10.1/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.10.1/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:32:42.709058 bec_scihub-0.10.1/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.10.1/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.10.1/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-11 09:32:42.711058 bec_scihub-0.10.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-08 15:33:35.000000 bec_scihub-0.10.1/setup.py
```

### Comparing `bec_scihub-0.10.0/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.10.1/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scibec/config_handler.py` & `bec_scihub-0.10.1/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scibec/scibec.py` & `bec_scihub-0.10.1/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scibec/scibec_connector.py` & `bec_scihub-0.10.1/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.10.1/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scibec/scibec_validator.py` & `bec_scihub-0.10.1/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scihub.py` & `bec_scihub-0.10.1/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/scihub/scilog/scilog.py` & `bec_scihub-0.10.1/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/setup.cfg` & `bec_scihub-0.10.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.10.0/setup.py` & `bec_scihub-0.10.1/setup.py`

 * *Files identical despite different names*

