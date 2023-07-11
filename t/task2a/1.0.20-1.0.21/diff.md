# Comparing `tmp/task2a-1.0.20.tar.gz` & `tmp/task2a-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.20.tar", max compression
+gzip compressed data, was "task2a-1.0.21.tar", max compression
```

## Comparing `task2a-1.0.20.tar` & `task2a-1.0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.20/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.20/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.20/pwgen/__main__.py
--rw-r--r--   0        0        0       24 2023-07-10 23:57:39.172788 task2a-1.0.20/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.20/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.20/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.20/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8456 2023-07-10 12:22:20.970691 task2a-1.0.20/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.20/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    20824 2023-07-10 23:57:09.275818 task2a-1.0.20/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      686 2023-07-10 23:57:39.177792 task2a-1.0.20/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.20/README.md
--rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.20/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.21/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.21/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.21/pwgen/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-11 00:04:03.245005 task2a-1.0.21/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.21/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.21/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.21/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8650 2023-07-11 00:04:03.249999 task2a-1.0.21/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.21/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20824 2023-07-10 23:57:09.275818 task2a-1.0.21/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      686 2023-07-11 00:04:03.253997 task2a-1.0.21/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.21/README.md
+-rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.21/PKG-INFO
```

### Comparing `task2a-1.0.20/pwgen/cli/cli.py` & `task2a-1.0.21/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.20/pwgen/pwgen.py` & `task2a-1.0.21/pwgen/pwgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,18 @@
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

### Comparing `task2a-1.0.20/pwgen/showcase/showcase.py` & `task2a-1.0.21/pwgen/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.20/pyproject.toml` & `task2a-1.0.21/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2a"
-version = "1.0.20"
+version = "1.0.21"
 description = "Password generation CLI and library"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen"}]
 #packages = [{include = "pwgen", format = "sdist"}]
 license = "MIT"
```

### Comparing `task2a-1.0.20/README.md` & `task2a-1.0.21/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.20/PKG-INFO` & `task2a-1.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.20
+Version: 1.0.21
 Summary: Password generation CLI and library
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.20 Summary: Password generation
+Metadata-Version: 2.1 Name: task2a Version: 1.0.21 Summary: Password generation
 CLI and library Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
 task2a License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

