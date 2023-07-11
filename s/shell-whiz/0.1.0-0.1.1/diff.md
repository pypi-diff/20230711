# Comparing `tmp/shell_whiz-0.1.0.tar.gz` & `tmp/shell_whiz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.0.tar", max compression
+gzip compressed data, was "shell_whiz-0.1.1.tar", max compression
```

## Comparing `shell_whiz-0.1.0.tar` & `shell_whiz-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/LICENSE
--rw-r--r--   0        0        0     1118 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/README.md
--rw-r--r--   0        0        0      515 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3874 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1530 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/config.py
--rw-r--r--   0        0        0      194 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     7282 2023-07-11 12:14:13.128451 shell_whiz-0.1.0/shell_whiz/openai.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 shell_whiz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1118 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/README.md
+-rw-r--r--   0        0        0      515 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3874 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1530 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/config.py
+-rw-r--r--   0        0        0      194 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     7282 2023-07-11 12:31:50.151888 shell_whiz-0.1.1/shell_whiz/openai.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 shell_whiz-0.1.1/PKG-INFO
```

### Comparing `shell_whiz-0.1.0/LICENSE` & `shell_whiz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.0/README.md` & `shell_whiz-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.0/pyproject.toml` & `shell_whiz-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.0"
+version = "0.1.1"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.1.0/shell_whiz/__init__.py` & `shell_whiz-0.1.1/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.0/shell_whiz/config.py` & `shell_whiz-0.1.1/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.0/shell_whiz/openai.py` & `shell_whiz-0.1.1/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.0/PKG-INFO` & `shell_whiz-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
```

