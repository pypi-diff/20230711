# Comparing `tmp/cmdcomp-1.1.0.tar.gz` & `tmp/cmdcomp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.0.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.1.tar", max compression
```

## Comparing `cmdcomp-1.1.0.tar` & `cmdcomp-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/README.md
--rw-r--r--   0        0        0       79 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2117 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1623 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1169 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1687 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/README.md
+-rw-r--r--   0        0        0       79 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2117 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-11 01:25:12.660017 cmdcomp-1.1.1/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1623 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1169 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1687 2023-07-11 01:25:12.664017 cmdcomp-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.1/PKG-INFO
```

### Comparing `cmdcomp-1.1.0/README.md` & `cmdcomp-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/app.py` & `cmdcomp-1.1.1/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/completion.py` & `cmdcomp-1.1.1/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/config/app_info.py` & `cmdcomp-1.1.1/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/config/command/command.py` & `cmdcomp-1.1.1/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/config/config.py` & `cmdcomp-1.1.1/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.1/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.1/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.0/pyproject.toml` & `cmdcomp-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.0"
+version = "1.1.1"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-1.1.0/PKG-INFO` & `cmdcomp-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.0
+Version: 1.1.1
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.0 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.1 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

