# Comparing `tmp/trainyard-0.0.0.tar.gz` & `tmp/trainyard-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainyard-0.0.0.tar", last modified: Mon Jun 26 20:30:33 2023, max compression
+gzip compressed data, was "trainyard-0.0.1.tar", last modified: Tue Jul 11 20:04:43 2023, max compression
```

## Comparing `trainyard-0.0.0.tar` & `trainyard-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:30:33.555649 trainyard-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 20:30:22.000000 trainyard-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 20:30:33.555649 trainyard-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:30:22.000000 trainyard-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 20:30:22.000000 trainyard-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:30:33.555649 trainyard-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:30:33.555649 trainyard-0.0.0/trainyard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:30:22.000000 trainyard-0.0.0/trainyard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:30:33.555649 trainyard-0.0.0/trainyard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 20:30:33.000000 trainyard-0.0.0/trainyard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-26 20:30:33.000000 trainyard-0.0.0/trainyard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:30:33.000000 trainyard-0.0.0/trainyard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 20:30:33.000000 trainyard-0.0.0/trainyard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 20:30:33.000000 trainyard-0.0.0/trainyard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 20:04:32.000000 trainyard-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 20:04:43.833976 trainyard-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 20:04:32.000000 trainyard-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 20:04:32.000000 trainyard-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:04:43.833976 trainyard-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 20:04:32.000000 trainyard-0.0.1/tests/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/runhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/trainer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/prefect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/top_level.txt
```

### Comparing `trainyard-0.0.0/LICENSE` & `trainyard-0.0.1/LICENSE`

 * *Files identical despite different names*

