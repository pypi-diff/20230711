# Comparing `tmp/aws_arns-0.1.1.tar.gz` & `tmp/aws_arns-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_arns-0.1.1.tar", last modified: Wed Mar 15 14:14:25 2023, max compression
+gzip compressed data, was "aws_arns-0.2.1.tar", last modified: Tue Jul 11 15:02:28 2023, max compression
```

## Comparing `aws_arns-0.1.1.tar` & `aws_arns-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 14:14:25.506170 aws_arns-0.1.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      484 2023-03-15 13:53:55.000000 aws_arns-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1118 2023-03-15 13:21:46.000000 aws_arns-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      316 2023-03-15 13:21:46.000000 aws_arns-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     3613 2023-03-15 14:14:25.506001 aws_arns-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2503 2023-03-15 14:03:04.000000 aws_arns-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 14:14:25.502881 aws_arns-0.1.1/aws_arns/
--rw-r--r--   0 sanhehu    (505) staff       (20)      384 2023-03-15 14:14:07.000000 aws_arns-0.1.1/aws_arns/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-03-15 13:59:19.000000 aws_arns-0.1.1/aws_arns/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      208 2023-03-15 13:26:05.000000 aws_arns-0.1.1/aws_arns/compat.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 14:14:25.504881 aws_arns-0.1.1/aws_arns/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-03-15 13:21:47.000000 aws_arns-0.1.1/aws_arns/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2191 2023-03-15 13:58:29.000000 aws_arns-0.1.1/aws_arns/model.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 14:14:25.504722 aws_arns-0.1.1/aws_arns.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     3613 2023-03-15 14:14:25.000000 aws_arns-0.1.1/aws_arns.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      461 2023-03-15 14:14:25.000000 aws_arns-0.1.1/aws_arns.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-03-15 14:14:25.000000 aws_arns-0.1.1/aws_arns.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      216 2023-03-15 14:14:25.000000 aws_arns-0.1.1/aws_arns.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        9 2023-03-15 14:14:25.000000 aws_arns-0.1.1/aws_arns.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      459 2023-03-15 13:54:51.000000 aws_arns-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      300 2023-03-15 14:09:20.000000 aws_arns-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-03-15 13:21:46.000000 aws_arns-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      183 2023-03-15 13:21:46.000000 aws_arns-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       42 2023-03-15 13:25:34.000000 aws_arns-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-03-15 14:14:25.506228 aws_arns-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7703 2023-03-15 13:21:46.000000 aws_arns-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 14:14:25.505573 aws_arns-0.1.1/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      264 2023-03-15 13:55:18.000000 aws_arns-0.1.1/tests/test_import.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2017 2023-03-15 13:53:44.000000 aws_arns-0.1.1/tests/test_model.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.749151 aws_arns-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      484 2023-07-10 21:07:32.000000 aws_arns-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1118 2023-07-10 21:07:32.000000 aws_arns-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      316 2023-07-10 21:07:32.000000 aws_arns-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3613 2023-07-11 15:02:28.749007 aws_arns-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2503 2023-07-10 21:07:32.000000 aws_arns-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.745399 aws_arns-0.2.1/aws_arns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      293 2023-07-11 14:45:03.000000 aws_arns-0.2.1/aws_arns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-11 14:44:23.000000 aws_arns-0.2.1/aws_arns/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      668 2023-07-11 14:41:13.000000 aws_arns-0.2.1/aws_arns/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      208 2023-07-10 21:07:32.000000 aws_arns-0.2.1/aws_arns/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      147 2023-07-11 14:09:55.000000 aws_arns-0.2.1/aws_arns/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.746399 aws_arns-0.2.1/aws_arns/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-10 21:07:32.000000 aws_arns-0.2.1/aws_arns/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7310 2023-07-11 14:25:03.000000 aws_arns-0.2.1/aws_arns/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-10 22:44:15.000000 aws_arns-0.2.1/aws_arns/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.747402 aws_arns-0.2.1/aws_arns/srv/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      167 2023-07-11 14:49:10.000000 aws_arns-0.2.1/aws_arns/srv/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3274 2023-07-11 14:49:39.000000 aws_arns-0.2.1/aws_arns/srv/batch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2691 2023-07-11 14:49:39.000000 aws_arns-0.2.1/aws_arns/srv/iam.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1508 2023-07-11 15:01:31.000000 aws_arns-0.2.1/aws_arns/srv/service.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.747843 aws_arns-0.2.1/aws_arns/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-10 22:43:58.000000 aws_arns-0.2.1/aws_arns/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      446 2023-07-10 22:43:58.000000 aws_arns-0.2.1/aws_arns/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.748290 aws_arns-0.2.1/aws_arns/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-10 22:43:28.000000 aws_arns-0.2.1/aws_arns/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-10 22:43:33.000000 aws_arns-0.2.1/aws_arns/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.746273 aws_arns-0.2.1/aws_arns.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3613 2023-07-11 15:02:28.000000 aws_arns-0.2.1/aws_arns.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      722 2023-07-11 15:02:28.000000 aws_arns-0.2.1/aws_arns.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-11 15:02:28.000000 aws_arns-0.2.1/aws_arns.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      216 2023-07-11 15:02:28.000000 aws_arns-0.2.1/aws_arns.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        9 2023-07-11 15:02:28.000000 aws_arns-0.2.1/aws_arns.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      994 2023-07-11 14:47:05.000000 aws_arns-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      300 2023-07-10 21:07:32.000000 aws_arns-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-07-10 21:07:32.000000 aws_arns-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-07-10 21:07:32.000000 aws_arns-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       42 2023-07-10 21:07:32.000000 aws_arns-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-11 15:02:28.749195 aws_arns-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7703 2023-07-10 21:07:32.000000 aws_arns-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-11 15:02:28.748732 aws_arns-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-07-11 14:42:58.000000 aws_arns-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6846 2023-07-11 14:43:57.000000 aws_arns-0.2.1/tests/test_model.py
```

### Comparing `aws_arns-0.1.1/LICENSE.txt` & `aws_arns-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_arns-0.1.1/PKG-INFO` & `aws_arns-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_arns
-Version: 0.1.1
+Version: 0.2.1
 Summary: Amazon Resource Names (ARNs) utilities.
 Home-page: https://github.com/MacHu-GWU/aws_arns-project
-Download-URL: https://pypi.python.org/pypi/aws_arns/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_arns/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_arns-0.1.1/README.rst` & `aws_arns-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `aws_arns-0.1.1/aws_arns.egg-info/PKG-INFO` & `aws_arns-0.2.1/aws_arns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-arns
-Version: 0.1.1
+Version: 0.2.1
 Summary: Amazon Resource Names (ARNs) utilities.
 Home-page: https://github.com/MacHu-GWU/aws_arns-project
-Download-URL: https://pypi.python.org/pypi/aws_arns/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_arns/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_arns-0.1.1/requirements-doc.txt` & `aws_arns-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_arns-0.1.1/setup.py` & `aws_arns-0.2.1/setup.py`

 * *Files identical despite different names*

