# Comparing `tmp/mydaoyipackage-0.0.1.tar.gz` & `tmp/mydaoyipackage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mydaoyipackage-0.0.1.tar", last modified: Mon Jul 10 10:59:28 2023, max compression
+gzip compressed data, was "mydaoyipackage-0.0.2.tar", last modified: Tue Jul 11 03:02:14 2023, max compression
```

## Comparing `mydaoyipackage-0.0.1.tar` & `mydaoyipackage-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 10:59:28.484555 mydaoyipackage-0.0.1/
--rw-rw-rw-   0        0        0       61 2023-07-10 10:59:28.483557 mydaoyipackage-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 10:59:28.479591 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/
--rw-rw-rw-   0        0        0       61 2023-07-10 10:59:28.000000 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-10 10:59:28.000000 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 10:59:28.000000 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-10 10:59:28.000000 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-10 10:59:28.000000 mydaoyipackage-0.0.1/mydaoyipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      214 2023-07-10 10:56:00.000000 mydaoyipackage-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 10:59:28.484555 mydaoyipackage-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 10:59:28.481560 mydaoyipackage-0.0.1/test_package_daoyi/
--rw-rw-rw-   0        0        0      117 2023-07-10 10:57:04.000000 mydaoyipackage-0.0.1/test_package_daoyi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:02:14.968071 mydaoyipackage-0.0.2/
+-rw-rw-rw-   0        0        0       61 2023-07-11 03:02:14.967073 mydaoyipackage-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 03:02:14.961092 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-07-11 03:02:14.000000 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-11 03:02:14.000000 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 03:02:14.000000 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-11 03:02:14.000000 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 03:02:14.000000 mydaoyipackage-0.0.2/mydaoyipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      214 2023-07-11 03:01:37.000000 mydaoyipackage-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 03:02:14.969069 mydaoyipackage-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 03:02:14.965106 mydaoyipackage-0.0.2/test_package_daoyi/
+-rw-rw-rw-   0        0        0      213 2023-07-11 03:01:37.000000 mydaoyipackage-0.0.2/test_package_daoyi/DaoYi.py
+-rw-rw-rw-   0        0        0      117 2023-07-10 10:57:04.000000 mydaoyipackage-0.0.2/test_package_daoyi/__init__.py
```

