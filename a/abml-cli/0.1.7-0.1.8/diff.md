# Comparing `tmp/abml_cli-0.1.7.tar.gz` & `tmp/abml_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abml_cli-0.1.7.tar", max compression
+gzip compressed data, was "abml_cli-0.1.8.tar", max compression
```

## Comparing `abml_cli-0.1.7.tar` & `abml_cli-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-04-12 13:16:57.000000 abml_cli-0.1.7/abml_cli/__init__.py
--rw-r--r--   0        0        0      388 2023-07-03 13:42:03.701126 abml_cli-0.1.7/abml_cli/abml_filters.py
--rw-r--r--   0        0        0     1187 2023-07-11 14:15:14.648257 abml_cli-0.1.7/abml_cli/abml_grids.py
--rw-r--r--   0        0        0     1513 2023-07-11 12:53:48.190021 abml_cli-0.1.7/abml_cli/abml_parser.py
--rw-r--r--   0        0        0     4501 2023-07-11 19:11:44.649054 abml_cli-0.1.7/abml_cli/abml_run.py
--rw-r--r--   0        0        0     3493 2023-07-11 19:13:58.648754 abml_cli-0.1.7/abml_cli/abml_yamler.py
--rw-r--r--   0        0        0      901 2023-07-11 19:25:50.328763 abml_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 13:18:26.000000 abml_cli-0.1.7/README.md
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 abml_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 13:16:57.000000 abml_cli-0.1.8/abml_cli/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-03 13:42:03.701126 abml_cli-0.1.8/abml_cli/abml_filters.py
+-rw-r--r--   0        0        0     1576 2023-07-11 21:20:22.065008 abml_cli-0.1.8/abml_cli/abml_grids.py
+-rw-r--r--   0        0        0     1513 2023-07-11 12:53:48.190021 abml_cli-0.1.8/abml_cli/abml_parser.py
+-rw-r--r--   0        0        0     4836 2023-07-11 21:31:52.947285 abml_cli-0.1.8/abml_cli/abml_run.py
+-rw-r--r--   0        0        0     3457 2023-07-11 20:35:49.947966 abml_cli-0.1.8/abml_cli/abml_yamler.py
+-rw-r--r--   0        0        0      901 2023-07-11 21:49:37.398484 abml_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 13:18:26.000000 abml_cli-0.1.8/README.md
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 abml_cli-0.1.8/PKG-INFO
```

### Comparing `abml_cli-0.1.7/abml_cli/abml_grids.py` & `abml_cli-0.1.8/abml_cli/abml_grids.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,7 +29,17 @@
 
 def get_parameters_list(parameters, grids):
     parameters_list = []
     for set_ in generate_param_grid(grids):
         parameters_list.append(update_nested_dict(parameters, set_))
     return parameters_list
 
+
+def flatten_dict(dictionary, parent_key='', separator='_'):
+    items = []
+    for key, value in dictionary.items():
+        new_key = f"{parent_key}{separator}{key}" if parent_key else key
+        if isinstance(value, dict):
+            items.extend(flatten_dict(value, new_key, separator).items())
+        else:
+            items.append((new_key, value))
+    return dict(items)
```

### Comparing `abml_cli-0.1.7/abml_cli/abml_parser.py` & `abml_cli-0.1.8/abml_cli/abml_parser.py`

 * *Files identical despite different names*

### Comparing `abml_cli-0.1.7/abml_cli/abml_run.py` & `abml_cli-0.1.8/abml_cli/abml_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import yaml
 import click
+from pandas import DataFrame
 from subprocess import run as prun
 from pathlib import Path
 from rich.console import Console
 from abml_cli.abml_yamler import generate_abml_file
-from abml_cli.abml_grids import get_parameters_list, generate_param_grid
+from abml_cli.abml_grids import get_parameters_list, generate_param_grid,flatten_dict
 import glob
 from os import remove, rename
 from os.path import isfile
 from yaml import safe_load
 import logging
 import sys
+import time
 
 c = Console()
 
 parser_path = (Path(__file__).parents[0] / "abml_parser.py").resolve()
 
 logger = logging.getLogger(__name__)
 logFormatter = logging.Formatter("%(asctime)s [%(name)s] [%(levelname)s]  %(message)s")
@@ -88,16 +90,20 @@
     root.mkdir(exist_ok=True)
 
     for grid_name in grids:
         grid_path = root / Path(grid_name)
         grid_path.mkdir(exist_ok=True)
         
         params_list = get_parameters_list(params, grids[grid_name])
+        df = DataFrame(map(flatten_dict, params_list))
+        names = []
         for i, params_grid in enumerate(params_list):
-            path = grid_path / Path(f"{i+1}")
+            timestr = time.strftime("%Y%m%d-%H%M%S")
+            names.append(timestr)
+            path = grid_path / Path(f"{timestr}")
             path.mkdir(exist_ok=True)
             
             filename = f'{file.split(".abml")[0]}.{path.name}'
             generate_abml_file(file, path=path, filename=filename, **params_grid)
             rendered = f"_{filename}.render.abml"
             cwd = Path().cwd()
             cmd = f'abaqus cae nogui="{parser_path}" -- --yml "{cwd / path / rendered}" --path "{cwd / path}"'
@@ -120,19 +126,20 @@
             if inp_new.is_file():
                 inp_new.unlink()
             inp.rename(inp_new)
 
             if input_folder is not None:
                 Path(cwd / grid_path / input_folder).mkdir(exist_ok=True)
                 Path(cwd / grid_path / input_folder / f"{i+1}.inp").write_bytes(inp_new.read_bytes())
-       
+        df["name"] = names
+        df.set_index("name", inplace=True)
+        df.to_csv(grid_path / "env.csv", sep=",")
+
     rpys = glob.glob("*.rpy*")
     recs = glob.glob("*.rec*")
 
     for file in rpys+recs:
         try:
             remove(file)
         except PermissionError:
             pass
 
-
-
```

### Comparing `abml_cli-0.1.7/abml_cli/abml_yamler.py` & `abml_cli-0.1.8/abml_cli/abml_yamler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
             for arg in args:
                 result.update(render_yaml_file(arg, **Include_Loader.params))
             return result
         if isinstance(node, nodes.MappingNode):  # type: ignore
             kwargs = self.construct_mapping(node)
             filename = kwargs.pop("filename")
             filter_module = kwargs.pop("filter") if "filter" in kwargs else None
-            Include_Loader.params.update(kwargs)
-            result = render_yaml_file(filename, filter_module=filter_module, **Include_Loader.params)
+            result = render_yaml_file(filename, filter_module=filter_module, **{**kwargs, **Include_Loader.params})
             return result
 
 
 Loader.add_constructor('!include', Include_Loader.include)
 
 class Env(Environment):
     def load_filters(self, module):
@@ -76,19 +75,19 @@
             env.load_filters(module)
         except ImportError:
             pass
         except FileNotFoundError:
             pass
 
     template = env.get_template(filename)
-    Include_Loader.set_params(params)
     return load(template.render(**params), Loader=Loader)
 
 
 def generate_abml_file(file, path=Path(), filename=None, **params):
     if filename is None:
         filename = f'{file.split(".abml")[0]}'
 
+    Include_Loader.set_params(params)
     output = render_yaml_file(file, __file__=filename.split(".")[0], **params)
     
     with open(path / f"_{filename}.render.abml", mode="w", encoding="utf-8") as f:
         dump(output, f)
```

### Comparing `abml_cli-0.1.7/pyproject.toml` & `abml_cli-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abml-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["DavidNaizheZhou <70525024+DavidNaizheZhou@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "abml_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `abml_cli-0.1.7/PKG-INFO` & `abml_cli-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abml-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: DavidNaizheZhou
 Author-email: 70525024+DavidNaizheZhou@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

