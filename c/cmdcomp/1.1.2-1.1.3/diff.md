# Comparing `tmp/cmdcomp-1.1.2.tar.gz` & `tmp/cmdcomp-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.2.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.3.tar", max compression
```

## Comparing `cmdcomp-1.1.2.tar` & `cmdcomp-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/README.md
--rw-r--r--   0        0        0       79 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2117 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1623 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1169 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1687 2023-07-11 01:36:04.340558 cmdcomp-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1511 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/README.md
+-rw-r--r--   0        0        0       79 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2117 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1623 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1169 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1687 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 cmdcomp-1.1.3/PKG-INFO
```

### Comparing `cmdcomp-1.1.2/README.md` & `cmdcomp-1.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```shell
 cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ### Docker
 
 ```shell
-docker run --rm -itv $(pwd):/apps/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
+docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ## Config
 
 Configuration can be written in JSON, YAML, and TOML file formats.
 
 ```toml
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (bash or zsh) from config toml file.
 ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
 --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
---rm -itv $(pwd):/apps/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
+--rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
 shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
 TOML file formats. ```toml [cmdcomp] version = "1" [app] name = "mycli" alias =
 "my-cli" [root] options = ["-h", "--help", "--version"] [root.subcommands.list]
 options = ["-a"] alias = "ls" [root.subcommands.execute] options = { type =
 "command", execute = "your_app_name ps -s" } alias = ["restart", "shell",
 "log"] [root.subcommands.cd] options = { type = "file", base_path = "$(cd $
 (dirname $0); pwd)/../apps" } ``` ## JSON Schema ### Config https://
```

### Comparing `cmdcomp-1.1.2/cmdcomp/app.py` & `cmdcomp-1.1.3/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/completion.py` & `cmdcomp-1.1.3/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/config/app_info.py` & `cmdcomp-1.1.3/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/config/command/command.py` & `cmdcomp-1.1.3/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/config/config.py` & `cmdcomp-1.1.3/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.3/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.3/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.2/pyproject.toml` & `cmdcomp-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.2"
+version = "1.1.3"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-1.1.2/PKG-INFO` & `cmdcomp-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.2
+Version: 1.1.3
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,15 +50,15 @@
 ```shell
 cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ### Docker
 
 ```shell
-docker run --rm -itv $(pwd):/apps/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
+docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ## Config
 
 Configuration can be written in JSON, YAML, and TOML file formats.
 
 ```toml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.2 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.3 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
@@ -11,15 +11,15 @@
 pydantic (>=2.0,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Project-URL:
 Repository, https://github.com/yassun4dev/cmdcomp Description-Content-Type:
 text/markdown # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (bash or zsh) from config toml file.
 ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
 --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
---rm -itv $(pwd):/apps/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
+--rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
 shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
 TOML file formats. ```toml [cmdcomp] version = "1" [app] name = "mycli" alias =
 "my-cli" [root] options = ["-h", "--help", "--version"] [root.subcommands.list]
 options = ["-a"] alias = "ls" [root.subcommands.execute] options = { type =
 "command", execute = "your_app_name ps -s" } alias = ["restart", "shell",
 "log"] [root.subcommands.cd] options = { type = "file", base_path = "$(cd $
 (dirname $0); pwd)/../apps" } ``` ## JSON Schema ### Config https://
```

