# Comparing `tmp/selenium_remote-0.1.1.tar.gz` & `tmp/selenium_remote-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_remote-0.1.1.tar", max compression
+gzip compressed data, was "selenium_remote-0.1.2.tar", max compression
```

## Comparing `selenium_remote-0.1.1.tar` & `selenium_remote-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.122937 selenium_remote-0.1.1/LICENSE
--rw-r--r--   0        0        0       91 2023-07-11 13:29:28.122937 selenium_remote-0.1.1/README.md
--rw-r--r--   0        0        0      748 2023-07-11 14:10:05.036640 selenium_remote-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:36:32.954532 selenium_remote-0.1.1/selenium_remote/__init__.py
--rw-r--r--   0        0        0      139 2023-07-11 13:54:12.017532 selenium_remote-0.1.1/selenium_remote/main.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 selenium_remote-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.122937 selenium_remote-0.1.2/LICENSE
+-rw-r--r--   0        0        0       91 2023-07-11 13:29:28.122937 selenium_remote-0.1.2/README.md
+-rw-r--r--   0        0        0      748 2023-07-11 14:12:34.320502 selenium_remote-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:36:32.954532 selenium_remote-0.1.2/selenium_remote/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-11 13:54:12.017532 selenium_remote-0.1.2/selenium_remote/main.py
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 selenium_remote-0.1.2/PKG-INFO
```

### Comparing `selenium_remote-0.1.1/LICENSE` & `selenium_remote-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.1/pyproject.toml` & `selenium_remote-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "selenium-remote"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package for haldling and using a selenium grid server."
 authors = ["George Pamfilis <gpamfilis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "selenium_remote"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 fake-useragent = "^1.1.3"
 selenium = "^4.10.0"
 webdriver-manager = "^3.8.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `selenium_remote-0.1.1/PKG-INFO` & `selenium_remote-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: selenium-remote
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for haldling and using a selenium grid server.
 Author: George Pamfilis
 Author-email: gpamfilis@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Description-Content-Type: text/markdown
 
 # selenium-remote
```

