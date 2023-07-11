# Comparing `tmp/json-any-2022.9.tar.gz` & `tmp/json-any-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2022.9.tar", last modified: Mon Jun 20 09:47:31 2022, max compression
+gzip compressed data, was "json-any-2023.1.tar", last modified: Tue Jul 11 10:52:33 2023, max compression
```

## Comparing `json-any-2022.9.tar` & `json-any-2023.1.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-06-20 09:47:31.743058 json-any-2022.9/
--rw-r--r--   0 eric      (1000) users      (984)       61 2022-04-04 12:15:46.000000 json-any-2022.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     2226 2022-06-20 09:47:31.743058 json-any-2022.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2022-02-23 16:31:24.000000 json-any-2022.9/README-COPYRIGHT.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2022.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     1457 2022-05-10 11:19:00.000000 json-any-2022.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-06-20 09:47:31.743058 json-any-2022.9/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1579 2022-05-10 09:32:56.000000 json-any-2022.9/json_any/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)    23039 2022-06-10 12:35:20.000000 json-any-2022.9/json_any/json_any.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-06-20 09:47:31.743058 json-any-2022.9/json_any/test/
--rw-r--r--   0 eric      (1000) users      (984)     9543 2022-06-10 09:23:45.000000 json-any-2022.9/json_any/test/test_json_any.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-06-20 09:47:31.743058 json-any-2022.9/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     2226 2022-06-20 09:47:31.000000 json-any-2022.9/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      292 2022-06-20 09:47:31.000000 json-any-2022.9/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2022-06-20 09:47:31.000000 json-any-2022.9/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2022-06-20 09:47:31.000000 json-any-2022.9/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2022.9/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2022-06-20 09:47:31.743058 json-any-2022.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     4419 2022-06-20 09:46:50.000000 json-any-2022.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 10:52:33.441800 json-any-2023.1/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.1/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.438467 json-any-2023.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.1/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1744 2023-07-10 12:40:50.000000 json-any-2023.1/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.1/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.1/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     2882 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     9304 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.1/json_any/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)    14277 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/object_to_json.py
+-rw-r--r--   0 eric      (1000) users      (984)     3666 2023-07-11 09:56:39.000000 json-any-2023.1/json_any/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-10 17:21:22.000000 json-any-2023.1/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      441 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.1/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-11 10:52:33.441800 json-any-2023.1/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5261 2023-07-11 10:51:15.000000 json-any-2023.1/setup.py
```

### Comparing `json-any-2022.9/README-LICENCE-utf8.txt` & `json-any-2023.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2022.9/json_any/__init__.py` & `json-any-2023.1/json_any/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-# import json_any.json_any
+__version__ = "2023.1"
```

