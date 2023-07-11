# Comparing `tmp/Akatosh-1.7.3.tar.gz` & `tmp/Akatosh-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-1.7.3.tar", last modified: Wed Jun 21 13:17:54 2023, max compression
+gzip compressed data, was "Akatosh-2.1.0.tar", last modified: Tue Jul 11 11:43:22 2023, max compression
```

## Comparing `Akatosh-1.7.3.tar` & `Akatosh-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.529914 Akatosh-1.7.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.509910 Akatosh-1.7.3/Akatosh/
--rw-rw-rw-   0        0        0      129 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    16093 2023-06-21 13:15:43.000000 Akatosh-1.7.3/Akatosh/actor.py
--rw-rw-rw-   0        0        0     1073 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/event.py
--rw-rw-rw-   0        0        0     6678 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/producer.py
--rw-rw-rw-   0        0        0    11540 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/resource.py
--rw-rw-rw-   0        0        0     1443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/timeline.py
--rw-rw-rw-   0        0        0     2443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.518911 Akatosh-1.7.3/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.528915 Akatosh-1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-1.7.3/README.md
--rw-rw-rw-   0        0        0      669 2023-06-21 13:16:13.000000 Akatosh-1.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 13:17:54.529914 Akatosh-1.7.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.525910 Akatosh-1.7.3/test/
--rw-rw-rw-   0        0        0      169 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_actor.py
--rw-rw-rw-   0        0        0      245 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_decorator.py
--rw-rw-rw-   0        0        0      298 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_resource.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.080116 Akatosh-2.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.064604 Akatosh-2.1.0/Akatosh/
+-rw-rw-rw-   0        0        0      181 2023-07-11 07:31:54.000000 Akatosh-2.1.0/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0     5122 2023-07-11 11:37:41.000000 Akatosh-2.1.0/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    11594 2023-07-11 11:31:04.000000 Akatosh-2.1.0/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-06-30 03:47:46.000000 Akatosh-2.1.0/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-11 05:33:51.000000 Akatosh-2.1.0/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-11 04:40:17.000000 Akatosh-2.1.0/Akatosh/states.py
+-rw-rw-rw-   0        0        0     5467 2023-07-11 08:04:04.000000 Akatosh-2.1.0/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:43:22.076116 Akatosh-2.1.0/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 11:43:22.000000 Akatosh-2.1.0/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-11 11:43:22.078115 Akatosh-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-11 11:42:13.000000 Akatosh-2.1.0/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-11 11:42:45.000000 Akatosh-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 11:43:22.080116 Akatosh-2.1.0/setup.cfg
```

### Comparing `Akatosh-1.7.3/pyproject.toml` & `Akatosh-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [project]
 name = "Akatosh"
-version = "1.7.3"
+version = "2.1.0"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ulfaric/Akatosh"
+"Documentation" = "https://ulfaric.github.io/Akatosh"
 "Bug Tracker" = "https://github.com/ulfaric/Akatosh/issues"
 
 [tool.setuptools]
 packages = ["Akatosh"]
 
-[tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra -q"
-testpaths = ["test"]
```

