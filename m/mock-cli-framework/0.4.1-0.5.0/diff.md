# Comparing `tmp/mock-cli-framework-0.4.1.tar.gz` & `tmp/mock-cli-framework-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-cli-framework-0.4.1.tar", last modified: Fri Jun 16 22:54:58 2023, max compression
+gzip compressed data, was "mock-cli-framework-0.5.0.tar", last modified: Mon Jul 10 22:51:27 2023, max compression
```

## Comparing `mock-cli-framework-0.4.1.tar` & `mock-cli-framework-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.964267 mock-cli-framework-0.4.1/
--rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.4.1/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     9581 2023-06-16 22:54:58.964327 mock-cli-framework-0.4.1/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     9143 2021-02-19 21:07:02.000000 mock-cli-framework-0.4.1/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.963505 mock-cli-framework-0.4.1/mock_cli/
--rw-r--r--   0 zach       (502) staff       (20)      541 2023-06-16 22:53:18.000000 mock-cli-framework-0.4.1/mock_cli/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)      417 2023-03-14 03:59:29.000000 mock-cli-framework-0.4.1/mock_cli/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.4.1/mock_cli/about.py
--rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.4.1/mock_cli/argv_conversion.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.963641 mock-cli-framework-0.4.1/mock_cli/data/
--rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.4.1/mock_cli/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.4.1/mock_cli/hashing.py
--rw-r--r--   0 zach       (502) staff       (20)     2507 2023-03-14 04:00:13.000000 mock-cli-framework-0.4.1/mock_cli/mock_cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     5494 2023-02-22 23:25:34.000000 mock-cli-framework-0.4.1/mock_cli/mock_cmd_state.py
--rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.4.1/mock_cli/path.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.4.1/mock_cli/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.4.1/mock_cli/responses.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.964144 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     9581 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      452 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)      156 2023-06-16 22:54:58.964514 mock-cli-framework-0.4.1/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.4.1/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.909373 mock-cli-framework-0.5.0/
+-rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.5.0/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-10 22:51:27.909436 mock-cli-framework-0.5.0/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     9452 2023-07-10 22:44:06.000000 mock-cli-framework-0.5.0/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.908559 mock-cli-framework-0.5.0/mock_cli/
+-rw-r--r--   0 zach       (502) staff       (20)      541 2023-07-10 22:50:10.000000 mock-cli-framework-0.5.0/mock_cli/__about__.py
+-rw-r--r--   0 zach       (502) staff       (20)      513 2023-07-01 05:01:04.000000 mock-cli-framework-0.5.0/mock_cli/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.5.0/mock_cli/about.py
+-rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.5.0/mock_cli/argv_conversion.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.908712 mock-cli-framework-0.5.0/mock_cli/data/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.5.0/mock_cli/data/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.5.0/mock_cli/hashing.py
+-rw-r--r--   0 zach       (502) staff       (20)     2507 2023-06-21 02:46:51.000000 mock-cli-framework-0.5.0/mock_cli/mock_cmd.py
+-rw-r--r--   0 zach       (502) staff       (20)     6872 2023-07-01 05:01:04.000000 mock-cli-framework-0.5.0/mock_cli/mock_cmd_state.py
+-rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.5.0/mock_cli/path.py
+-rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.5.0/mock_cli/pkg_resources.py
+-rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.5.0/mock_cli/responses.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.909256 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      452 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        9 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)      156 2023-07-10 22:51:27.909660 mock-cli-framework-0.5.0/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.5.0/setup.py
```

### Comparing `mock-cli-framework-0.4.1/LICENSE` & `mock-cli-framework-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.1/PKG-INFO` & `mock-cli-framework-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.4.1
+Version: 0.5.0
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -161,14 +161,18 @@
 - `cmd_args` is a list of strings represengting command-line arguments
 - `output` is a `bytes` object read from the command's standard output.
 - `error_output` is a `bytes` object read from the command's standard error.
 - `returncode` is the command's numerical exit status when executed with the provided command-line arguments
 - `invocation_name` is a unique, arbitrary name given to this particular invocation
   - It is recommended that the name be related to the command's arguments and intended action
   - The name should be filesystem-safe as it will be used as the directory name on disk to hold the output files
+- `changes_state` a boolean flag indicating if this command should trigger a state iteration
+- `input` is an optional bytes-like object that will be hashed if provided.
+  - The command invocation will be added under "commands_with_input" using its hash as a key
+  - Since more than one command may work with the same input, the invocations will be further keyed by their command-line arguments
 
 Here's an example:
 
 ```Python
 import subprocess
 from mock_cli import ResponseDirectory, CommandInvocation
 
@@ -200,15 +204,14 @@
 )
 ```
 
 ## Limitations
 
 There are a number of limitations to be aware of that prevent `mock-cli-framework` from fully simulating some commands:
 
-- Standard input isn't processed, so behavior that is affected by it isn't simulated
 - Environment variables aren't processed, so behavior that is affected by them isn't simulated
 - Normal and error output can't be interleaved on the console
   - Standard output, if any, is written first
   - Standard error, if any, is written next
 - Timing/performance can't be simulated, and will usually be virtually instaneous
   - A command's typical run-time for a given input/workload can't be simulated
   - No assumptions can be made about one workload being faster/slower than another
```

### Comparing `mock-cli-framework-0.4.1/README.md` & `mock-cli-framework-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 - `cmd_args` is a list of strings represengting command-line arguments
 - `output` is a `bytes` object read from the command's standard output.
 - `error_output` is a `bytes` object read from the command's standard error.
 - `returncode` is the command's numerical exit status when executed with the provided command-line arguments
 - `invocation_name` is a unique, arbitrary name given to this particular invocation
   - It is recommended that the name be related to the command's arguments and intended action
   - The name should be filesystem-safe as it will be used as the directory name on disk to hold the output files
+- `changes_state` a boolean flag indicating if this command should trigger a state iteration
+- `input` is an optional bytes-like object that will be hashed if provided.
+  - The command invocation will be added under "commands_with_input" using its hash as a key
+  - Since more than one command may work with the same input, the invocations will be further keyed by their command-line arguments
 
 Here's an example:
 
 ```Python
 import subprocess
 from mock_cli import ResponseDirectory, CommandInvocation
 
@@ -188,15 +192,14 @@
 )
 ```
 
 ## Limitations
 
 There are a number of limitations to be aware of that prevent `mock-cli-framework` from fully simulating some commands:
 
-- Standard input isn't processed, so behavior that is affected by it isn't simulated
 - Environment variables aren't processed, so behavior that is affected by them isn't simulated
 - Normal and error output can't be interleaved on the console
   - Standard output, if any, is written first
   - Standard error, if any, is written next
 - Timing/performance can't be simulated, and will usually be virtually instaneous
   - A command's typical run-time for a given input/workload can't be simulated
   - No assumptions can be made about one workload being faster/slower than another
```

### Comparing `mock-cli-framework-0.4.1/mock_cli/__about__.py` & `mock-cli-framework-0.5.0/mock_cli/__about__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "Mock CLI Framework"
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 __summary__ = """A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests."""
 
 """
 See PEP 440 for version scheme
 https://www.python.org/dev/peps/pep-0440/#examples-of-compliant-version-schemes
 Examples:
```

### Comparing `mock-cli-framework-0.4.1/mock_cli/argv_conversion.py` & `mock-cli-framework-0.5.0/mock_cli/argv_conversion.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.1/mock_cli/mock_cmd.py` & `mock-cli-framework-0.5.0/mock_cli/mock_cmd.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.1/mock_cli/mock_cmd_state.py` & `mock-cli-framework-0.5.0/mock_cli/mock_cmd_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from . import data
 from .pkg_resources import pkgfiles
 
 STATE_DIR_ENV_NAME = "MOCK_CMD_STATE_DIR"
 
 
@@ -25,19 +25,27 @@
 
     def __init__(self, env_config_dict):
         super().__init__(env_config_dict)
         self._saved_env = dict(os.environ)
 
     @property
     def set_vars(self) -> Dict[str, str]:
-        return self["set_vars"]
+        return self["set"]
+
+    @set_vars.setter
+    def set_vars(self, set_vars: Dict[str, str]):
+        self["set"] = set_vars
 
     @property
     def pop_vars(self) -> List[str]:
-        return self["pop_vars"]
+        return self["pop"]
+
+    @pop_vars.setter
+    def pop_vars(self, pop_vars: List[str]):
+        self["pop"] = pop_vars
 
     def initialize_env(self):
         for var in self.pop_vars:
             os.environ.pop(var, None)
 
         for var, val in self.set_vars.items():
             os.environ[var] = val
@@ -66,27 +74,30 @@
         obj = cls(template_dict)
         return obj
 
 
 class MockCMDStateConfig(dict):
 
     def __init__(self, config_path, config=None):
+        if isinstance(config_path, str):
+            config_path = Path(config_path)
         if config:
             config_dict = config
         else:
             config_dict = json.load(open(config_path, "r"))
         super().__init__(config_dict)
         self._config_path = config_path
         self._env_config: MockCMDEnvironmentConfig = None
         self._initialize_env()
 
     @property
     def response_directory(self):
-        response_dir_list = self["response-directory-list"]
-        response_dir = response_dir_list[self.iteration]
+        state_list = self.state_list
+        current_state = state_list[self.iteration]
+        response_dir = current_state["response-directory"]
         return response_dir
 
     @property
     def iteration(self) -> int:
         return self["iteration"]
 
     @iteration.setter
@@ -97,14 +108,42 @@
     def max_iterations(self) -> int:
         return self["max-iterations"]
 
     @property
     def env_config(self) -> MockCMDEnvironmentConfig:
         pass
 
+    @property
+    def state_list(self):
+        return self["state-list"]
+
+    def increase_max_iterations(self):
+        self["max-iterations"] += 1
+
+    def add_state(self, response_dir_path, set_vars: Optional[Dict] = None, pop_vars: Optional[List] = None):
+        # it's totally okay to have the same response directory more than once
+        # so we're not checking for collisions here
+        if set_vars is None:
+            set_vars = {}
+        if pop_vars is None:
+            pop_vars = []
+        # convert to string in case we got a Path
+        response_dir_path = str(response_dir_path)
+        env = MockCMDEnvironmentConfig.from_template()
+        env.set_vars = set_vars
+        env.pop_vars = pop_vars
+
+        state = {
+            "response-directory": response_dir_path,
+            "env-vars": env
+        }
+        self.state_list.append(state)
+        self.increase_max_iterations()
+        self.save_config()
+
     def iterate(self):
         if self.iteration >= self.max_iterations:
             raise MockCMDStateMaxIterationException(
                 f"Already reached max iterations: {self.max_iterations}")
         self.iteration += 1
         self.save_config()
 
@@ -114,24 +153,26 @@
         # explicitly set env_config to None
         self._env_config = None
 
         # initialize the next env
         self._initialize_env()
 
     def save_config(self):
+        self._config_path.parent.mkdir(parents=True, exist_ok=True)
         with open(self._config_path, "w") as f:
             json.dump(self, f, indent=2)
 
     def _initialize_env(self):
         # don't initialize a config if we have done so already
         # set to None before calling this in order to initialize
         # the next config otherwise we'll clobber the saved config
         if self._env_config is None:
-            env_list = self["env-list"]
-            env_config = env_list[self.iteration]
+            state_list = self.state_list
+            current_state = state_list[self.iteration]
+            env_config = current_state["env-vars"]
             env_config = MockCMDEnvironmentConfig(env_config)
             env_config.initialize_env()
             self._env_config = env_config
 
 
 class MockCMDNewStateConfig(MockCMDStateConfig):
```

### Comparing `mock-cli-framework-0.4.1/mock_cli/path.py` & `mock-cli-framework-0.5.0/mock_cli/path.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.1/mock_cli/responses.py` & `mock-cli-framework-0.5.0/mock_cli/responses.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.1/mock_cli_framework.egg-info/PKG-INFO` & `mock-cli-framework-0.5.0/mock_cli_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.4.1
+Version: 0.5.0
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -161,14 +161,18 @@
 - `cmd_args` is a list of strings represengting command-line arguments
 - `output` is a `bytes` object read from the command's standard output.
 - `error_output` is a `bytes` object read from the command's standard error.
 - `returncode` is the command's numerical exit status when executed with the provided command-line arguments
 - `invocation_name` is a unique, arbitrary name given to this particular invocation
   - It is recommended that the name be related to the command's arguments and intended action
   - The name should be filesystem-safe as it will be used as the directory name on disk to hold the output files
+- `changes_state` a boolean flag indicating if this command should trigger a state iteration
+- `input` is an optional bytes-like object that will be hashed if provided.
+  - The command invocation will be added under "commands_with_input" using its hash as a key
+  - Since more than one command may work with the same input, the invocations will be further keyed by their command-line arguments
 
 Here's an example:
 
 ```Python
 import subprocess
 from mock_cli import ResponseDirectory, CommandInvocation
 
@@ -200,15 +204,14 @@
 )
 ```
 
 ## Limitations
 
 There are a number of limitations to be aware of that prevent `mock-cli-framework` from fully simulating some commands:
 
-- Standard input isn't processed, so behavior that is affected by it isn't simulated
 - Environment variables aren't processed, so behavior that is affected by them isn't simulated
 - Normal and error output can't be interleaved on the console
   - Standard output, if any, is written first
   - Standard error, if any, is written next
 - Timing/performance can't be simulated, and will usually be virtually instaneous
   - A command's typical run-time for a given input/workload can't be simulated
   - No assumptions can be made about one workload being faster/slower than another
```

### Comparing `mock-cli-framework-0.4.1/setup.py` & `mock-cli-framework-0.5.0/setup.py`

 * *Files identical despite different names*

