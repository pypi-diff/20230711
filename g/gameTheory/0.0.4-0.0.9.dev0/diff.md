# Comparing `tmp/gameTheory-0.0.4.tar.gz` & `tmp/gameTheory-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameTheory-0.0.4.tar", last modified: Wed Dec 21 05:52:58 2022, max compression
+gzip compressed data, was "gameTheory-0.0.9.dev0.tar", last modified: Tue Jul 11 02:51:38 2023, max compression
```

## Comparing `gameTheory-0.0.4.tar` & `gameTheory-0.0.9.dev0.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 05:52:58.780921 gameTheory-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-21 05:52:44.000000 gameTheory-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2022-12-21 05:52:58.780921 gameTheory-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-21 05:52:44.000000 gameTheory-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 05:52:58.780921 gameTheory-0.0.4/gamekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 05:52:58.780921 gameTheory-0.0.4/gamekit/gameTheory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2022-12-21 05:52:58.000000 gameTheory-0.0.4/gamekit/gameTheory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-21 05:52:58.000000 gameTheory-0.0.4/gamekit/gameTheory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 05:52:58.000000 gameTheory-0.0.4/gamekit/gameTheory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-21 05:52:58.000000 gameTheory-0.0.4/gamekit/gameTheory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 05:52:58.000000 gameTheory-0.0.4/gamekit/gameTheory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2022-12-21 05:52:44.000000 gameTheory-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 05:52:58.780921 gameTheory-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.053414 gameTheory-0.0.9.dev0/gameTheory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-11 02:51:38.000000 gameTheory-0.0.9.dev0/gameTheory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-11 02:51:38.000000 gameTheory-0.0.9.dev0/gameTheory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:51:38.000000 gameTheory-0.0.9.dev0/gameTheory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 02:51:38.000000 gameTheory-0.0.9.dev0/gameTheory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.053414 gameTheory-0.0.9.dev0/gamekit/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/gamekit/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/algorithms/bankruptcy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/gamekit/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/gamekit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/gamekit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:51:38.057414 gameTheory-0.0.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 02:51:12.000000 gameTheory-0.0.9.dev0/setup.py
```

### Comparing `gameTheory-0.0.4/LICENSE` & `gameTheory-0.0.9.dev0/LICENSE`

 * *Files identical despite different names*

