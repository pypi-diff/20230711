# Comparing `tmp/task2a-1.0.19.tar.gz` & `tmp/task2a-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.19.tar", max compression
+gzip compressed data, was "task2a-1.0.20.tar", max compression
```

## Comparing `task2a-1.0.19.tar` & `task2a-1.0.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.19/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.19/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.19/pwgen/__main__.py
--rw-r--r--   0        0        0       24 2023-07-10 23:53:36.394193 task2a-1.0.19/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.19/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.19/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.19/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8456 2023-07-10 12:22:20.970691 task2a-1.0.19/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.19/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    20813 2023-07-10 23:53:30.926187 task2a-1.0.19/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      686 2023-07-10 23:53:30.931187 task2a-1.0.19/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.19/README.md
--rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.19/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.20/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.20/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.20/pwgen/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-10 23:57:39.172788 task2a-1.0.20/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.20/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.20/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.20/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8456 2023-07-10 12:22:20.970691 task2a-1.0.20/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.20/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.20/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20824 2023-07-10 23:57:09.275818 task2a-1.0.20/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      686 2023-07-10 23:57:39.177792 task2a-1.0.20/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.20/README.md
+-rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.20/PKG-INFO
```

### Comparing `task2a-1.0.19/pwgen/cli/cli.py` & `task2a-1.0.20/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.19/pwgen/pwgen.py` & `task2a-1.0.20/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.19/pwgen/showcase/showcase.py` & `task2a-1.0.20/pwgen/showcase/showcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,17 @@
                 'command': 'pwgen -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{} {} {}',
                 'module_command': f'{python_command} pwgen -t "u{{{{4}}}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_complex': {
                 'descr': 'complex pattern',
                 'command':
-                    f'pwgen -t f"u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                    f'pwgen -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'module_command':
-                    f'{python_command} pwgen -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                    f'{python_command} pwgen -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
         },
     },
     'file': {
         'descr': 'pattern from a file',
         'command': 'pwgen -f {} -c{} {} {}',
```

### Comparing `task2a-1.0.19/pyproject.toml` & `task2a-1.0.20/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2a"
-version = "1.0.19"
+version = "1.0.20"
 description = "Password generation CLI and library"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen"}]
 #packages = [{include = "pwgen", format = "sdist"}]
 license = "MIT"
```

### Comparing `task2a-1.0.19/README.md` & `task2a-1.0.20/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.19/PKG-INFO` & `task2a-1.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.19
+Version: 1.0.20
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
-Metadata-Version: 2.1 Name: task2a Version: 1.0.19 Summary: Password generation
+Metadata-Version: 2.1 Name: task2a Version: 1.0.20 Summary: Password generation
 CLI and library Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
 task2a License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

