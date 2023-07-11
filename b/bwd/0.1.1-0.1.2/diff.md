# Comparing `tmp/bwd-0.1.1.tar.gz` & `tmp/bwd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwd-0.1.1.tar", max compression
+gzip compressed data, was "bwd-0.1.2.tar", max compression
```

## Comparing `bwd-0.1.1.tar` & `bwd-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.1/LICENSE
--rw-r--r--   0        0        0      854 2023-07-11 11:01:58.243429 bwd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      495 2022-05-17 20:40:56.204982 bwd-0.1.1/src/bwd/__init__.py
--rw-r--r--   0        0        0     4204 2023-07-10 21:49:37.009554 bwd-0.1.1/src/bwd/bwd.py
--rw-r--r--   0        0        0     4107 2023-07-10 21:48:49.286458 bwd-0.1.1/src/bwd/bwd_random.py
--rw-r--r--   0        0        0     4745 2023-07-10 21:51:11.360429 bwd-0.1.1/src/bwd/multi_bwd.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bwd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3782 2023-07-11 11:09:37.228356 bwd-0.1.2/README.md
+-rw-r--r--   0        0        0     1058 2023-07-11 11:08:55.903459 bwd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      495 2022-05-17 20:40:56.204982 bwd-0.1.2/src/bwd/__init__.py
+-rw-r--r--   0        0        0     4204 2023-07-10 21:49:37.009554 bwd-0.1.2/src/bwd/bwd.py
+-rw-r--r--   0        0        0     4107 2023-07-10 21:48:49.286458 bwd-0.1.2/src/bwd/bwd_random.py
+-rw-r--r--   0        0        0     4745 2023-07-10 21:51:11.360429 bwd-0.1.2/src/bwd/multi_bwd.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bwd-0.1.2/PKG-INFO
```

### Comparing `bwd-0.1.1/LICENSE` & `bwd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bwd-0.1.1/pyproject.toml` & `bwd-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "bwd"
-version = "0.1.1"
+version = "0.1.2"
 description = "A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)"
 authors = ["Drew Dimmery <drew.dimmery@gmail.com>"]
 license = "Apache-2.0"
+readme = "README.md"
+homepage = "https://ddimmery.github.io/balancer-package/"
+repository = "https://github.com/ddimmery/balancer-package"
+keywords = ["causal inference", "experimentation", "ab testing"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "^1.22.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `bwd-0.1.1/src/bwd/bwd.py` & `bwd-0.1.2/src/bwd/bwd.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.1/src/bwd/bwd_random.py` & `bwd-0.1.2/src/bwd/bwd_random.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.1/src/bwd/multi_bwd.py` & `bwd-0.1.2/src/bwd/multi_bwd.py`

 * *Files identical despite different names*

