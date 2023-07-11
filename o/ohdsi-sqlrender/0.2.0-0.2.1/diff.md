# Comparing `tmp/ohdsi-sqlrender-0.2.0.tar.gz` & `tmp/ohdsi-sqlrender-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-sqlrender-0.2.0.tar", last modified: Wed Jun 14 08:26:52 2023, max compression
+gzip compressed data, was "ohdsi-sqlrender-0.2.1.tar", last modified: Tue Jul 11 14:30:34 2023, max compression
```

## Comparing `ohdsi-sqlrender-0.2.0.tar` & `ohdsi-sqlrender-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi/sqlrender/
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-06-14 08:26:29.000000 ohdsi-sqlrender-0.2.0/ohdsi/sqlrender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-14 08:26:29.000000 ohdsi-sqlrender-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-07-11 14:30:22.000000 ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-11 14:30:22.000000 ohdsi-sqlrender-0.2.1/setup.py
```

### Comparing `ohdsi-sqlrender-0.2.0/ohdsi/sqlrender/__init__.py` & `ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/__init__.py`

 * *Files identical despite different names*

### Comparing `ohdsi-sqlrender-0.2.0/setup.py` & `ohdsi-sqlrender-0.2.1/setup.py`

 * *Files identical despite different names*

