# Comparing `tmp/task2b-1.0.17.tar.gz` & `tmp/task2b-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2b-1.0.17.tar", max compression
+gzip compressed data, was "task2b-1.0.18.tar", max compression
```

## Comparing `task2b-1.0.17.tar` & `task2b-1.0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.17/LICENSE
--rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.17/pwgen2/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.17/pwgen2/__main__.py
--rw-r--r--   0        0        0       24 2023-07-11 00:15:54.751984 task2b-1.0.17/pwgen2/__version__.py
--rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.17/pwgen2/cli/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.17/pwgen2/cli/__main__.py
--rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.17/pwgen2/cli/cli.py
--rw-r--r--   0        0        0    10294 2023-07-10 22:43:31.232041 task2b-1.0.17/pwgen2/pwgen2.py
--rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.17/pwgen2/showcase/__init__.py
--rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.17/pwgen2/showcase/__main__.py
--rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.17/pwgen2/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      276 2023-07-10 21:35:29.827459 task2b-1.0.17/pwgen2/showcase/pattern-list.txt
--rw-r--r--   0        0        0    23166 2023-07-10 23:47:02.310666 task2b-1.0.17/pwgen2/showcase/showcase.py
--rw-r--r--   0        0        0      588 2023-07-11 00:15:54.755982 task2b-1.0.17/pyproject.toml
--rw-r--r--   0        0        0    17425 2023-07-11 00:15:54.747988 task2b-1.0.17/README.md
--rw-r--r--   0        0        0    17821 1970-01-01 00:00:00.000000 task2b-1.0.17/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.18/LICENSE
+-rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.18/pwgen2/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.18/pwgen2/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-11 09:08:07.390951 task2b-1.0.18/pwgen2/__version__.py
+-rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.18/pwgen2/cli/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.18/pwgen2/cli/__main__.py
+-rw-r--r--   0        0        0     4668 2023-07-11 09:05:02.736640 task2b-1.0.18/pwgen2/cli/cli.py
+-rw-r--r--   0        0        0    10294 2023-07-11 09:05:02.737647 task2b-1.0.18/pwgen2/pwgen2.py
+-rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.18/pwgen2/showcase/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.18/pwgen2/showcase/__main__.py
+-rw-r--r--   0        0        0      132 2023-07-11 09:05:02.737647 task2b-1.0.18/pwgen2/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      276 2023-07-11 09:05:02.738638 task2b-1.0.18/pwgen2/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    23176 2023-07-11 09:05:02.738638 task2b-1.0.18/pwgen2/showcase/showcase.py
+-rw-r--r--   0        0        0      588 2023-07-11 09:08:07.395955 task2b-1.0.18/pyproject.toml
+-rw-r--r--   0        0        0    17425 2023-07-11 09:05:02.726644 task2b-1.0.18/README.md
+-rw-r--r--   0        0        0    17821 1970-01-01 00:00:00.000000 task2b-1.0.18/PKG-INFO
```

### Comparing `task2b-1.0.17/pwgen2/cli/cli.py` & `task2b-1.0.18/pwgen2/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     return sys.stdin.read().strip().splitlines()
 
 
 def pwgen_cli():
     sys.stdout.reconfigure(encoding="utf-8")
 
-    parser = argparse.ArgumentParser(description='Password Generator')
+    parser = argparse.ArgumentParser(description='Password Generator v.2')
     [parser.add_argument('-' + key, **ARGUMENTS[key].to_argparse()) for key, val in ARGUMENTS.items()]
     args = parser.parse_args()
 
     set_log_level(args.v)
 
     logger.info(f'Password generator has started as a standalone application.')
     [logger.debug(f'{ARGUMENTS[key].name}: {val}') for key, val in vars(args).items() if
```

### Comparing `task2b-1.0.17/pwgen2/pwgen2.py` & `task2b-1.0.18/pwgen2/pwgen2.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.17/pwgen2/showcase/showcase.py` & `task2b-1.0.18/pwgen2/showcase/showcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,17 +439,17 @@
 
     [print_output(el[1], el[0]) for el in command_packet]
 
 
 def pwgen_showcase():
     sys.stdout.reconfigure(encoding="utf-8")
 
-    parser = argparse.ArgumentParser(description='Password Generator')
+    parser = argparse.ArgumentParser(description='Password Generator showcase')
     parser.add_argument('--all', action='store_true', help='Show all use cases at once without any interaction')
-    parser.add_argument('-m', action='store_true', help='Invoke pwgen using python -m approach')
+    parser.add_argument('-m', action='store_true', help='Invoke pwgen2 using python -m approach')
     args = parser.parse_args()
 
     command_key_name = 'module_command' if args.m else 'command'
 
     if args.all:
         packet_output(command_key_name)
         return
```

### Comparing `task2b-1.0.17/pyproject.toml` & `task2b-1.0.18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2b"
-version = "1.0.17"
+version = "1.0.18"
 description = "Password generation CLI and library version 2"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen2"}]
 license = "MIT"
```

### Comparing `task2b-1.0.17/README.md` & `task2b-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `task2b-1.0.17/PKG-INFO` & `task2b-1.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2b
-Version: 1.0.17
+Version: 1.0.18
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
-Metadata-Version: 2.1 Name: task2b Version: 1.0.17 Summary: Password generation
+Metadata-Version: 2.1 Name: task2b Version: 1.0.18 Summary: Password generation
 CLI and library version 2 Home-page: https://gitlab.com/Bill-EPAM-
 DevOpsInt2023/python/task2b License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

