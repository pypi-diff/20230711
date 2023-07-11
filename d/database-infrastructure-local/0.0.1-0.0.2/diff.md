# Comparing `tmp/database-infrastructure-local-0.0.1.tar.gz` & `tmp/database-infrastructure-local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-infrastructure-local-0.0.1.tar", last modified: Mon Jul 10 13:35:27 2023, max compression
+gzip compressed data, was "database-infrastructure-local-0.0.2.tar", last modified: Mon Jul 10 13:42:01 2023, max compression
```

## Comparing `database-infrastructure-local-0.0.1.tar` & `database-infrastructure-local-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:35:27.013220 database-infrastructure-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-10 13:35:27.013220 database-infrastructure-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-10 13:35:17.000000 database-infrastructure-local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:35:27.013220 database-infrastructure-local-0.0.1/database_infrastructure_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-10 13:35:27.000000 database-infrastructure-local-0.0.1/database_infrastructure_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 13:35:27.000000 database-infrastructure-local-0.0.1/database_infrastructure_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:35:27.000000 database-infrastructure-local-0.0.1/database_infrastructure_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:35:27.000000 database-infrastructure-local-0.0.1/database_infrastructure_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:35:27.013220 database-infrastructure-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-10 13:35:17.000000 database-infrastructure-local-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:35:27.013220 database-infrastructure-local-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-10 13:35:17.000000 database-infrastructure-local-0.0.1/tests/test_number_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:01.363602 database-infrastructure-local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-10 13:42:01.363602 database-infrastructure-local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-10 13:41:48.000000 database-infrastructure-local-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:01.359602 database-infrastructure-local-0.0.2/database_infrastructure_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-10 13:42:01.000000 database-infrastructure-local-0.0.2/database_infrastructure_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 13:42:01.000000 database-infrastructure-local-0.0.2/database_infrastructure_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:42:01.000000 database-infrastructure-local-0.0.2/database_infrastructure_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:42:01.000000 database-infrastructure-local-0.0.2/database_infrastructure_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:42:01.363602 database-infrastructure-local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-10 13:41:48.000000 database-infrastructure-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:01.359602 database-infrastructure-local-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-10 13:41:48.000000 database-infrastructure-local-0.0.2/tests/test_number_generator.py
```

### Comparing `database-infrastructure-local-0.0.1/README.md` & `database-infrastructure-local-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `database-infrastructure-local-0.0.1/setup.py` & `database-infrastructure-local-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='database-infrastructure-local',  
-     version='0.0.1',
+     version='0.0.2',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles Database Infrastructure Local Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `database-infrastructure-local-0.0.1/tests/test_number_generator.py` & `database-infrastructure-local-0.0.2/tests/test_number_generator.py`

 * *Files identical despite different names*

