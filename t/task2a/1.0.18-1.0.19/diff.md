# Comparing `tmp/task2a-1.0.18.tar.gz` & `tmp/task2a-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.18.tar", max compression
+gzip compressed data, was "task2a-1.0.19.tar", max compression
```

## Comparing `task2a-1.0.18.tar` & `task2a-1.0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.18/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.18/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.18/pwgen/__main__.py
--rw-r--r--   0        0        0       24 2023-07-10 16:33:33.227433 task2a-1.0.18/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.18/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.18/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.18/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8456 2023-07-10 12:22:20.970691 task2a-1.0.18/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.18/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.18/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.18/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-09 17:21:49.870912 task2a-1.0.18/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    20700 2023-07-10 16:32:35.306652 task2a-1.0.18/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      686 2023-07-10 16:33:33.231438 task2a-1.0.18/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.18/README.md
--rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.19/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.19/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.19/pwgen/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-10 23:53:36.394193 task2a-1.0.19/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.19/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.19/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.19/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8456 2023-07-10 12:22:20.970691 task2a-1.0.19/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.19/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.19/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20813 2023-07-10 23:53:30.926187 task2a-1.0.19/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      686 2023-07-10 23:53:30.931187 task2a-1.0.19/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.19/README.md
+-rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.19/PKG-INFO
```

### Comparing `task2a-1.0.18/pwgen/cli/cli.py` & `task2a-1.0.19/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.18/pwgen/pwgen.py` & `task2a-1.0.19/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.18/pwgen/showcase/showcase.py` & `task2a-1.0.19/pwgen/showcase/showcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 
 # Determine the platform
 current_platform = platform.system()
 
 # Set the Python command based on the platform
 if current_platform == 'Windows':
     python_command = 'python -m'
+    bash_symbol = '$'
 else:
     python_command = 'python3 -m'
+    bash_symbol = '\$'
 
 select_style = questionary.Style([
     #     ('default', "bg:#ffffff fg:#000000"),
     # ('selected', 'bg:#336699 fg:#ffffff'),
     ('highlighted', '#008888'),
     ('pointer', '#008888'),
     # ('question', 'fg:#009b06'),
@@ -133,16 +135,16 @@
                 'descr': 'custom charset based on default',
                 'command': 'pwgen -S dp -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen -S dp -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_additional': {
                 'descr': 'custom charset with additional symbols',
-                'command': 'pwgen -S "u\\@\\$\\%\\&\\#\\*\\!" -n{} -c{} {}',
-                'module_command': f'{python_command} pwgen -S "u\\@\\$\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
+                'command': f'pwgen -S "u\\@\\{bash_symbol}\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
+                'module_command': f'{python_command} pwgen -S "u\\@\\{bash_symbol}\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_exclusions': {
                 'descr': 'custom charset with exclusions',
                 'command': 'pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
@@ -174,28 +176,28 @@
                 'descr': 'pattern with a custom charset placeholder',
                 'command': 'pwgen -t u{{4}}[pd]{{3}}l{{2}} -c{} {} {}',
                 'module_command': f'{python_command} pwgen -t u{{{{4}}}}[pd]{{{{3}}}}l{{{{2}}}} -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_specific': {
                 'descr': 'pattern with a custom charset with a specific symbol placeholder',
-                'command': 'pwgen -t "u{{4}}[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
-                'module_command': f'{python_command} pwgen -t "u{{{{4}}}}[pd\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                'command': f'pwgen -t "u{{{{4}}}}[pd\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                'module_command': f'{python_command} pwgen -t "u{{{{4}}}}[pd\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_exclusions': {
                 'descr': 'pattern with a custom charset placeholder with exclusions',
                 'command': 'pwgen -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{} {} {}',
                 'module_command': f'{python_command} pwgen -t "u{{{{4}}}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_complex': {
                 'descr': 'complex pattern',
                 'command':
-                    'pwgen -t "u{{4}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
+                    f'pwgen -t f"u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'module_command':
                     f'{python_command} pwgen -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
         },
     },
     'file': {
@@ -226,16 +228,16 @@
                 'descr': 'pipe stderr to a file',
                 'command': 'pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" {} 2> {}',
                 'module_command': f'{python_command} pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" {{}} 2> {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['v'], OPTIONS_ARGUMENTS['f_log'], ],
             },
             'pipe_complex': {
                 'descr': 'complex pipe with a sort command',
-                'command': 'echo u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}} | pwgen -c6 {} | sort -r',
-                'module_command': f'echo u{{{{4}}}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{{{3}}}}l{{{{2}}}} | {python_command} pwgen -c6 {{}} | sort -r',
+                'command': 'echo "u{{4}}d{{3}}\\-l{{2}}" | pwgen -c6 {} | sort -r',
+                'module_command': f'echo "u{{{{4}}}}d{{{{3}}}}\\-l{{{{2}}}}" | {python_command} pwgen -c6 {{}} | sort -r',
                 'arguments': [OPTIONS_ARGUMENTS['v'], ],
             },
         }
     },
     'with_errors': {
         'descr': 'patterns and character sets with errors',
         'options': {
```

### Comparing `task2a-1.0.18/pyproject.toml` & `task2a-1.0.19/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2a"
-version = "1.0.18"
+version = "1.0.19"
 description = "Password generation CLI and library"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen"}]
 #packages = [{include = "pwgen", format = "sdist"}]
 license = "MIT"
```

### Comparing `task2a-1.0.18/README.md` & `task2a-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.18/PKG-INFO` & `task2a-1.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.18
+Version: 1.0.19
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
-Metadata-Version: 2.1 Name: task2a Version: 1.0.18 Summary: Password generation
+Metadata-Version: 2.1 Name: task2a Version: 1.0.19 Summary: Password generation
 CLI and library Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
 task2a License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

