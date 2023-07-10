# Comparing `tmp/task2b-1.0.8.tar.gz` & `tmp/task2b-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2b-1.0.8.tar", max compression
+gzip compressed data, was "task2b-1.0.9.tar", max compression
```

## Comparing `task2b-1.0.8.tar` & `task2b-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.8/LICENSE
--rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.8/pwgen2/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.8/pwgen2/__main__.py
--rw-r--r--   0        0        0       23 2023-07-10 22:25:04.185728 task2b-1.0.8/pwgen2/__version__.py
--rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.8/pwgen2/cli/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.8/pwgen2/cli/__main__.py
--rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.8/pwgen2/cli/cli.py
--rw-r--r--   0        0        0    10100 2023-07-10 20:52:19.816687 task2b-1.0.8/pwgen2/pwgen2.py
--rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.8/pwgen2/showcase/__init__.py
--rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.8/pwgen2/showcase/__main__.py
--rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.8/pwgen2/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      276 2023-07-10 21:35:29.827459 task2b-1.0.8/pwgen2/showcase/pattern-list.txt
--rw-r--r--   0        0        0    23210 2023-07-10 22:25:04.197732 task2b-1.0.8/pwgen2/showcase/showcase.py
--rw-r--r--   0        0        0      587 2023-07-10 22:25:04.190741 task2b-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.8/README.md
--rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.9/LICENSE
+-rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.9/pwgen2/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.9/pwgen2/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-10 22:43:48.499514 task2b-1.0.9/pwgen2/__version__.py
+-rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.9/pwgen2/cli/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.9/pwgen2/cli/__main__.py
+-rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.9/pwgen2/cli/cli.py
+-rw-r--r--   0        0        0    10294 2023-07-10 22:43:31.232041 task2b-1.0.9/pwgen2/pwgen2.py
+-rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.9/pwgen2/showcase/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.9/pwgen2/showcase/__main__.py
+-rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.9/pwgen2/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      276 2023-07-10 21:35:29.827459 task2b-1.0.9/pwgen2/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    23210 2023-07-10 22:25:04.197732 task2b-1.0.9/pwgen2/showcase/showcase.py
+-rw-r--r--   0        0        0      587 2023-07-10 22:43:48.503515 task2b-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.9/README.md
+-rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.9/PKG-INFO
```

### Comparing `task2b-1.0.8/pwgen2/cli/cli.py` & `task2b-1.0.9/pwgen2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.8/pwgen2/pwgen2.py` & `task2b-1.0.9/pwgen2/pwgen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,18 @@
         return ''
     # elif pattern.find(' ') != -1:
     #     logger.error(f'You cannot use space symbol in pattern ({pattern})')
 
     # Convert \{ \} \[ \] to the { } [ ]. It could be an error, but it's a minor error. Just sanitize string.
     n_pattern = pattern.replace('\\{', '{').replace('\\}', '}').replace('\\[', '[').replace('\\]', ']')
 
+    # Remove double quotes at the start and at the end of the pattern.
+    if len(n_pattern) > 1 and n_pattern[:1] == '"' and n_pattern[-1] == '"':
+        n_pattern = (n_pattern[1:])[:-1]
+
     if n_pattern[0] == '{':
         logger.error(f'Incorrect utilization of braces in the pattern ({pattern}) due to braces cannot come first')
         return ''
 
     pat_ls = split_pattern(n_pattern)
 
     pat_ls = [(el.replace('{', '').replace('}', ''), ) if el.find('{') != -1 else el
```

### Comparing `task2b-1.0.8/pwgen2/showcase/showcase.py` & `task2b-1.0.9/pwgen2/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.8/pyproject.toml` & `task2b-1.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2b"
-version = "1.0.8"
+version = "1.0.9"
 description = "Password generation CLI and library version 2"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen2"}]
 license = "MIT"
```

### Comparing `task2b-1.0.8/README.md` & `task2b-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `task2b-1.0.8/PKG-INFO` & `task2b-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2b
-Version: 1.0.8
+Version: 1.0.9
 Summary: Password generation CLI and library version 2
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2b Version: 1.0.8 Summary: Password generation
+Metadata-Version: 2.1 Name: task2b Version: 1.0.9 Summary: Password generation
 CLI and library version 2 Home-page: https://gitlab.com/Bill-EPAM-
 DevOpsInt2023/python/task2b License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

