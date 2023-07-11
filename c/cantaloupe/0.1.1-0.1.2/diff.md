# Comparing `tmp/cantaloupe-0.1.1.tar.gz` & `tmp/cantaloupe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cantaloupe-0.1.1.tar", max compression
+gzip compressed data, was "cantaloupe-0.1.2.tar", max compression
```

## Comparing `cantaloupe-0.1.1.tar` & `cantaloupe-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      601 2023-07-11 03:47:46.986514 cantaloupe-0.1.1/README.md
--rw-r--r--   0        0        0      812 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/__init__.py
--rw-r--r--   0        0        0       73 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/__main__.py
--rw-r--r--   0        0        0     1022 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/enums.py
--rw-r--r--   0        0        0      551 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/errors.py
--rw-r--r--   0        0        0     1451 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/hookspecs.py
--rw-r--r--   0        0        0     3390 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/host.py
--rw-r--r--   0        0        0     1658 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/loaders.py
--rw-r--r--   0        0        0      694 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/logger.py
--rw-r--r--   0        0        0     2715 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/models.py
--rw-r--r--   0        0        0        0 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/plugins/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/plugins/core_cli.py
--rw-r--r--   0        0        0      695 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/plugins/core_error_handling.py
--rw-r--r--   0        0        0     3557 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/plugins/core_framework.py
--rw-r--r--   0        0        0        0 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/types.py
--rw-r--r--   0        0        0        0 2023-07-11 03:47:46.990514 cantaloupe-0.1.1/src/cantaloupe/utils.py
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 cantaloupe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1266 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/README.md
+-rw-r--r--   0        0        0      812 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/__main__.py
+-rw-r--r--   0        0        0     1022 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/enums.py
+-rw-r--r--   0        0        0      551 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/errors.py
+-rw-r--r--   0        0        0     1451 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/hookspecs.py
+-rw-r--r--   0        0        0     3382 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/host.py
+-rw-r--r--   0        0        0     1658 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/loaders.py
+-rw-r--r--   0        0        0      694 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/logger.py
+-rw-r--r--   0        0        0     2715 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/models.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_cli.py
+-rw-r--r--   0        0        0      695 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_error_handling.py
+-rw-r--r--   0        0        0     3557 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_framework.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/types.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/utils.py
+-rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 cantaloupe-0.1.2/PKG-INFO
```

### Comparing `cantaloupe-0.1.1/README.md` & `cantaloupe-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -14,19 +14,43 @@
 
 ### Usage
 
 ```bash
 $ poetry run cantaloupe --help
 ```
 
+#### Example Workflow
+
+A workflow is a YAML file that describes a series of steps to be executed.
+The following example workflow will open Google and type "cantaloupe" into the search bar.
+
+Note: nothing will actually happen until a cantaloupe plugin is installed that implements the logic to translate the
+workflow steps into browser actions.
+Please see the [Plugins](#plugins) section for more information.
+
+```yaml
+name: "Google Search"
+steps:
+  - action: goto
+    config:
+      url: "https://google.com"
+  - action: type
+    config:
+      selector: "input[name='q']"
+      text: "cantaloupe"
+```
+
+### Plugins
+
+* [cantaloupe-playwright](#plugins) coming soon
+
 ## Development
 
 ### Requirements
 
 * Python >= 3.10
 * [Poetry](https://python-poetry.org/docs/#installation)
 
-
 ### Creating plugins
 
-Plugins are created by implementing the cantaloupe hookspec. 
-See [cantaloupe/hookspecs.py](cantaloupe/hookspecs.py) for the hookspecs.
+Plugins are created by implementing the cantaloupe hookspec.
+See [cantaloupe/hookspecs.py](src/cantaloupe/hookspecs.py) for the hookspecs.
```

### Comparing `cantaloupe-0.1.1/pyproject.toml` & `cantaloupe-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cantaloupe"
-version = "0.1.1"
+version = "0.1.2"
 description = "An extensible framework for building browser automations."
 authors = ["Lemuel Boyce <lemuelboyce@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "cantaloupe", from = "src" }]
 
 [tool.poetry.scripts]
 cantaloupe = "cantaloupe.__main__:entry"
```

### Comparing `cantaloupe-0.1.1/src/cantaloupe/enums.py` & `cantaloupe-0.1.2/src/cantaloupe/enums.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/errors.py` & `cantaloupe-0.1.2/src/cantaloupe/errors.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/hookspecs.py` & `cantaloupe-0.1.2/src/cantaloupe/hookspecs.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/host.py` & `cantaloupe-0.1.2/src/cantaloupe/host.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             self.relay.cantaloupe_build_workflow(
                 config=config,
                 context=context,
                 workflow=workflow,
             )
 
 
-def main(args: tuple[Any]) -> None:
+def main(args: list[Any]) -> None:
     """
     Main entry point for the Cantaloupe CLI.
     """
 
     manager = get_plugin_manager()
 
     # Add all plugin options to parser
@@ -101,12 +101,12 @@
 
 def get_plugin_manager() -> pluggy.PluginManager:
     """
     Returns the plugin manager for cantaloupe.
     """
     manager = pluggy.PluginManager("cantaloupe")
     manager.add_hookspecs(hookspecs)
-    manager.load_setuptools_entrypoints("cantaloupe_plugin")
+    manager.load_setuptools_entrypoints("cantaloupe")
     manager.register(core_framework)
     manager.register(core_error_handling)
     manager.register(core_cli)
     return manager
```

### Comparing `cantaloupe-0.1.1/src/cantaloupe/loaders.py` & `cantaloupe-0.1.2/src/cantaloupe/loaders.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/logger.py` & `cantaloupe-0.1.2/src/cantaloupe/logger.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/models.py` & `cantaloupe-0.1.2/src/cantaloupe/models.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/plugins/core_cli.py` & `cantaloupe-0.1.2/src/cantaloupe/plugins/core_cli.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/plugins/core_error_handling.py` & `cantaloupe-0.1.2/src/cantaloupe/plugins/core_error_handling.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.1/src/cantaloupe/plugins/core_framework.py` & `cantaloupe-0.1.2/src/cantaloupe/plugins/core_framework.py`

 * *Files identical despite different names*

