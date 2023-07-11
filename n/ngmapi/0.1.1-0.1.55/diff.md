# Comparing `tmp/ngmapi-0.1.1.tar.gz` & `tmp/ngmapi-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.1.1.tar", last modified: Mon Jul 10 11:34:41 2023, max compression
+gzip compressed data, was "ngmapi-0.1.55.tar", last modified: Tue Jul 11 10:27:37 2023, max compression
```

## Comparing `ngmapi-0.1.1.tar` & `ngmapi-0.1.55.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:34:41.436228 ngmapi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 11:34:41.436228 ngmapi-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:34:41.436228 ngmapi-0.1.1/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:33:58.000000 ngmapi-0.1.1/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 11:33:58.000000 ngmapi-0.1.1/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 11:33:58.000000 ngmapi-0.1.1/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 11:33:58.000000 ngmapi-0.1.1/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:34:41.436228 ngmapi-0.1.1/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 11:34:41.000000 ngmapi-0.1.1/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 11:33:59.000000 ngmapi-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:34:41.436228 ngmapi-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:34:41.436228 ngmapi-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-10 11:33:58.000000 ngmapi-0.1.1/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:27:37.453018 ngmapi-0.1.55/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 10:27:37.453018 ngmapi-0.1.55/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:27:37.449017 ngmapi-0.1.55/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:47.000000 ngmapi-0.1.55/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 10:26:47.000000 ngmapi-0.1.55/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 10:26:47.000000 ngmapi-0.1.55/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 10:26:47.000000 ngmapi-0.1.55/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:27:37.453018 ngmapi-0.1.55/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 10:27:37.000000 ngmapi-0.1.55/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 10:26:47.000000 ngmapi-0.1.55/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:27:37.453018 ngmapi-0.1.55/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:27:37.453018 ngmapi-0.1.55/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 10:26:47.000000 ngmapi-0.1.55/tests/test_add.py
```

### Comparing `ngmapi-0.1.1/pyproject.toml` & `ngmapi-0.1.55/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.1.1"
+version = "0.1.55"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
```

