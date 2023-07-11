# Comparing `tmp/shell_whiz-0.1.2.tar.gz` & `tmp/shell_whiz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.2.tar", max compression
+gzip compressed data, was "shell_whiz-0.1.3.tar", max compression
```

## Comparing `shell_whiz-0.1.2.tar` & `shell_whiz-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/LICENSE
--rw-r--r--   0        0        0     1023 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/README.md
--rw-r--r--   0        0        0      515 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3874 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1530 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/config.py
--rw-r--r--   0        0        0      194 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     7282 2023-07-11 12:36:42.214880 shell_whiz-0.1.2/shell_whiz/openai.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 shell_whiz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1018 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/README.md
+-rw-r--r--   0        0        0      515 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3874 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1530 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/config.py
+-rw-r--r--   0        0        0      194 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     7282 2023-07-11 18:39:14.545196 shell_whiz-0.1.3/shell_whiz/openai.py
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 shell_whiz-0.1.3/PKG-INFO
```

### Comparing `shell_whiz-0.1.2/LICENSE` & `shell_whiz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.2/README.md` & `shell_whiz-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/beimzhan/shell-whiz)
 ![GitHub license](https://img.shields.io/github/license/beimzhan/shell-whiz)
 
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
 
 ## All features
 - **Pay as you go:** you only pay for what you use; no subscription is required. Just receive an API key from https://platform.openai.com/account/api-keys.
-- **Easy to install:** just run `pip install shell-whiz` and you're good to go.
+- **Easy to install:** run `pip install shell-whiz` and you're good to go.
 - **Easy to use:** Shell Whiz is a command-line tool.
     - Run `sw ask` to generate shell commands from your natural language queries.
     - Run `sw explain` to get an explanation of any shell command..
 
 ## License
 Shell Whiz is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for more information.
```

### Comparing `shell_whiz-0.1.2/pyproject.toml` & `shell_whiz-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.2"
+version = "0.1.3"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.1.2/shell_whiz/__init__.py` & `shell_whiz-0.1.3/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.2/shell_whiz/config.py` & `shell_whiz-0.1.3/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.2/shell_whiz/openai.py` & `shell_whiz-0.1.3/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.2/PKG-INFO` & `shell_whiz-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.1.2
+Version: 0.1.3
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
@@ -19,15 +19,15 @@
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/beimzhan/shell-whiz)
 ![GitHub license](https://img.shields.io/github/license/beimzhan/shell-whiz)
 
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
 
 ## All features
 - **Pay as you go:** you only pay for what you use; no subscription is required. Just receive an API key from https://platform.openai.com/account/api-keys.
-- **Easy to install:** just run `pip install shell-whiz` and you're good to go.
+- **Easy to install:** run `pip install shell-whiz` and you're good to go.
 - **Easy to use:** Shell Whiz is a command-line tool.
     - Run `sw ask` to generate shell commands from your natural language queries.
     - Run `sw explain` to get an explanation of any shell command..
 
 ## License
 Shell Whiz is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for more information.
```

