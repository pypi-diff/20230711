# Comparing `tmp/selenium_remote-0.1.0.tar.gz` & `tmp/selenium_remote-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_remote-0.1.0.tar", max compression
+gzip compressed data, was "selenium_remote-0.1.1.tar", max compression
```

## Comparing `selenium_remote-0.1.0.tar` & `selenium_remote-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.122937 selenium_remote-0.1.0/LICENSE
--rw-r--r--   0        0        0       91 2023-07-11 13:29:28.122937 selenium_remote-0.1.0/README.md
--rw-r--r--   0        0        0      623 2023-07-11 13:48:08.173875 selenium_remote-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:36:32.954532 selenium_remote-0.1.0/selenium_remote/__init__.py
--rw-r--r--   0        0        0      139 2023-07-11 13:54:12.017532 selenium_remote-0.1.0/selenium_remote/main.py
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 selenium_remote-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.122937 selenium_remote-0.1.1/LICENSE
+-rw-r--r--   0        0        0       91 2023-07-11 13:29:28.122937 selenium_remote-0.1.1/README.md
+-rw-r--r--   0        0        0      748 2023-07-11 14:10:05.036640 selenium_remote-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:36:32.954532 selenium_remote-0.1.1/selenium_remote/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-11 13:54:12.017532 selenium_remote-0.1.1/selenium_remote/main.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 selenium_remote-0.1.1/PKG-INFO
```

### Comparing `selenium_remote-0.1.0/LICENSE` & `selenium_remote-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.0/PKG-INFO` & `selenium_remote-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: selenium-remote
-Version: 0.1.0
-Summary: A package for halding and using a selenium grid server.
+Version: 0.1.1
+Summary: A package for haldling and using a selenium grid server.
 Author: George Pamfilis
 Author-email: gpamfilis@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
```

