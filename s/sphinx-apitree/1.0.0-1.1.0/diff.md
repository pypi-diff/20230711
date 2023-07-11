# Comparing `tmp/sphinx-apitree-1.0.0.tar.gz` & `tmp/sphinx_apitree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-apitree-1.0.0.tar", last modified: Tue Jul 11 09:22:33 2023, max compression
+gzip compressed data, was "sphinx_apitree-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx-apitree-1.0.0.tar` & `sphinx_apitree-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,23 @@
--rw-r--r--   0        0        0     1240 2023-07-11 08:59:32.590106 sphinx-apitree-1.0.0/.github/workflows/pytest_and_autopublish.yml
--rw-r--r--   0        0        0     3096 2023-06-30 17:11:07.551262 sphinx-apitree-1.0.0/.gitignore
--rw-r--r--   0        0        0       65 2023-06-29 12:31:24.003288 sphinx-apitree-1.0.0/.vscode/extensions.json
--rw-r--r--   0        0        0      768 2023-06-29 12:31:49.464358 sphinx-apitree-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0    11357 2023-06-29 12:25:00.308998 sphinx-apitree-1.0.0/LICENSE
--rw-r--r--   0        0        0     1409 2023-07-07 08:55:23.504398 sphinx-apitree-1.0.0/README.md
--rw-r--r--   0        0        0       66 2023-07-05 12:47:49.151823 sphinx-apitree-1.0.0/apitree/__init__.py
--rw-r--r--   0        0        0     1338 2023-06-29 12:32:15.348554 sphinx-apitree-1.0.0/apitree/ast_utils.py
--rw-r--r--   0        0        0     2565 2023-07-06 13:23:12.126585 sphinx-apitree-1.0.0/apitree/conf_util.py
--rw-r--r--   0        0        0      761 2023-07-06 12:19:36.850237 sphinx-apitree-1.0.0/apitree/ext/docstring.py
--rw-r--r--   0        0        0      443 2023-07-07 09:53:58.823002 sphinx-apitree-1.0.0/apitree/ext/linkify.py
--rw-r--r--   0        0        0     1691 2023-07-04 14:15:02.992895 sphinx-apitree-1.0.0/apitree/html_helper.py
--rw-r--r--   0        0        0       30 2023-07-04 09:35:37.997461 sphinx-apitree-1.0.0/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-04 16:04:02.822095 sphinx-apitree-1.0.0/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-04 15:12:25.388724 sphinx-apitree-1.0.0/apitree/signature_utils.py
--rw-r--r--   0        0        0    10099 2023-07-06 13:46:49.701215 sphinx-apitree-1.0.0/apitree/symbol_match.py
--rw-r--r--   0        0        0      179 2023-07-06 13:40:47.585409 sphinx-apitree-1.0.0/apitree/templates/api.md
--rw-r--r--   0        0        0       13 2023-07-05 11:39:17.948470 sphinx-apitree-1.0.0/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-06 12:05:59.186594 sphinx-apitree-1.0.0/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-06 12:05:43.757892 sphinx-apitree-1.0.0/apitree/templates/function.md
--rw-r--r--   0        0        0      115 2023-07-06 13:36:29.789313 sphinx-apitree-1.0.0/apitree/templates/module.md
--rw-r--r--   0        0        0       13 2023-07-06 12:06:07.661408 sphinx-apitree-1.0.0/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1655 2023-07-06 10:21:30.849044 sphinx-apitree-1.0.0/apitree/tree_extractor.py
--rw-r--r--   0        0        0      874 2023-07-06 13:42:33.125990 sphinx-apitree-1.0.0/apitree/writer.py
--rw-r--r--   0        0        0     1508 2023-07-05 13:05:59.099998 sphinx-apitree-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 sphinx-apitree-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1980 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/README.md
+-rw-r--r--   0        0        0      105 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/__init__.py
+-rw-r--r--   0        0        0     1338 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ast_utils.py
+-rw-r--r--   0        0        0     2723 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/conf_util.py
+-rw-r--r--   0        0        0      761 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ext/docstring.py
+-rw-r--r--   0        0        0      443 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ext/linkify.py
+-rw-r--r--   0        0        0     1691 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/html_helper.py
+-rw-r--r--   0        0        0       30 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/structs.py
+-rw-r--r--   0        0        0     9597 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/symbol_match.py
+-rw-r--r--   0        0        0      183 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/api.md
+-rw-r--r--   0        0        0       13 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/function.md
+-rw-r--r--   0        0        0      154 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/module.md
+-rw-r--r--   0        0        0       13 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1693 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      782 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/writer.py
+-rw-r--r--   0        0        0     1508 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 sphinx_apitree-1.1.0/PKG-INFO
```

### Comparing `sphinx-apitree-1.0.0/LICENSE` & `sphinx_apitree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-apitree-1.0.0/README.md` & `sphinx_apitree-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # sphinx-apitree
 
+[![Unittests](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml)
+[![PyPI version](https://badge.fury.io/py/sphinx-apitree.svg)](https://badge.fury.io/py/sphinx-apitree)
+
+
 `apitree` is a small library to generate a ready-to-use documentation with minimal friction!
 
 `apitree` takes care of everything, so you can only focus on the code.
 
 ## Usage
 
 In `docs/conf.py`, replace everything by:
 
 ```python
 import apitree
 
 apitree.make_project(
-    project_name='my_module',
+    # e.g. `import visu3d as v3d` -> {'v3d': 'visu3d'}
+    project_name={'alias': 'my_module'},
     globals=globals(),
 )
 ```
 
 Then to generate the doc:
 
 ```sh
@@ -32,28 +37,28 @@
   api/my_module/index
 ```
 
 ## Features
 
 * Theme
 * Auto-generate the API tree, with better features
-  * Do not require `__all__`
+  * Do not require `__all__` (smart detect of which symbols are documented)
   * Add expandable toc tree with all symbols
 * ...
 
 ## Installation in a project
 
 1.  In `pyproject.toml`
 
     ```toml
     [project.optional-dependencies]
     # Installed through `pip install .[docs]`
     docs = [
         # Install `apitree` with all extensions (sphinx, theme,...)
-        "sphinx-apitree[ext] @ https://github.com/conchylicultor/sphinx-apitree",
+        "sphinx-apitree[ext]",
     ]
     ```
 
 1.  In `.readthedocs.yaml`
 
     ```yaml
     sphinx:
@@ -65,10 +70,11 @@
         path: .
         extra_requirements:
             - docs
     ```
 
 ## Examples of projects using apitree
 
-* https://github.com/google-research/visu3d
-* https://github.com/google-research/dataclass_array
-* https://github.com/google-research/etils
+* https://github.com/google-research/visu3d (https://visu3d.readthedocs.io/)
+* https://github.com/google-research/dataclass_array (https://dataclass-array.readthedocs.io/)
+* https://github.com/google-research/etils (https://etils.readthedocs.io/)
+* https://github.com/google-research/kauldron (https://kauldron.readthedocs.io/)
```

### Comparing `sphinx-apitree-1.0.0/apitree/ast_utils.py` & `sphinx_apitree-1.1.0/apitree/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-apitree-1.0.0/apitree/conf_util.py` & `sphinx_apitree-1.1.0/apitree/conf_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import importlib
 import pathlib
 from typing import Any
 
 import tomllib
 from etils import epath
 
-from apitree import writer
+from apitree import structs, writer
 from apitree.ext import docstring
 
 
 def setup(app):
   # Fix bad ```python md formatting
   docstring.setup(app)
 
 
 def make_project(
-    modules: dict[str, str],
+    modules: dict[str, str] | structs.ModuleInfo,
     globals: dict[str, Any],
 ):
   root_dir = epath.Path(globals['__file__']).parent  # <repo>/docs/
   project_name = _get_project_name(root_dir=root_dir.parent)
 
   api_dir = root_dir / 'api'
   if api_dir.exists():
     api_dir.rmtree()
   api_dir.mkdir()
 
-  for alias, module_name in modules.items():
-    module = importlib.import_module(module_name)
+  if isinstance(modules, dict):
+    modules = [
+      structs.ModuleInfo(alias=k, module_name=v) for k, v in modules.items()
+    ]
+  if isinstance(modules, structs.ModuleInfo):
+    modules = [modules]
 
-    writer.write_doc(module, alias=alias, root_dir=api_dir)
+  for module_info in modules:
+    writer.write_doc(module_info, root_dir=api_dir)
 
   globals.update(
       # Project information
       project=project_name,
       copyright=f'2023, {project_name} authors',
       author=f'{project_name} authors',
       # General configuration
```

### Comparing `sphinx-apitree-1.0.0/apitree/ext/docstring.py` & `sphinx_apitree-1.1.0/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx-apitree-1.0.0/apitree/html_helper.py` & `sphinx_apitree-1.1.0/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx-apitree-1.0.0/apitree/symbol_match.py` & `sphinx_apitree-1.1.0/apitree/symbol_match.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 import os
 import pathlib
 import types
-from collections.abc import Callable
+from collections.abc import Callable, Iterator
 from typing import Any
 
 import typing_extensions
 from etils import edc, epath, epy
 
 from apitree import ast_utils, md_utils, tree_extractor
 
@@ -42,32 +42,26 @@
   def imported_symbols(self) -> set[str]:
     if self.parent.__file__ is None:  # Implicit package
       return set()
     # TODO(epot): Cache across module
     return set(imp.alias for imp in ast_utils.parse_global_imports(self.parent))
 
   @functools.cached_property
-  def is_package(self) -> bool:
-    # TODO(epot): Could also add custom attribute `__docutil__.is_package` so
-    # standard module behave like package.
-    return _is_package(self.value)
-
-  @functools.cached_property
   def belong_to_namespace(self) -> bool:
     return self.value.__name__.startswith(self.ctx.module_name)
 
   @functools.cached_property
   def match(self) -> type[Match]:
     return Match.root_match(self)
 
   @functools.cached_property
   def qualname(self) -> bool:
     """Exemple: `dca.typing.Float`."""
     if self.parent_symb is None:  # root node
-      assert self.ctx.module_name == self.name
+      # assert self.ctx.module_name == self.name
       return self.ctx.alias
     return f'{self.parent_symb.symbol.qualname}.{self.name}'
 
   @functools.cached_property
   def qualname_no_alias(self) -> bool:
     """Exemple: `dataclass_array.typing.Float`."""
     if self.parent_symb is None:  # root node
@@ -151,14 +145,30 @@
     # * Source code
     return self.template.format(
         qualname=self.symbol.qualname,
         qualname_no_alias=self.symbol.qualname_no_alias,
         **self.extra_template_kwargs,
     )
 
+  def make_symbols_table(self, nodes: Iterator[tree_extractor.Node]):
+    table = md_utils.Table(header=['', '', ''])
+
+    for n in nodes:
+      filename = n.match.filename
+      filename = filename.relative_to(self.filename.parent)
+      filename = os.fspath(filename)
+      filename = filename.removesuffix('.md')
+      table.add_row(
+          f'*{n.match.icon}*',
+          f'[{n.symbol.qualname}]({filename})',
+          f'{n.match.docstring_1line}',
+      )
+
+    return table.make()
+
 
 def _not(cls: type[Match]) -> Callable[[Match], bool]:
   def match(self):
     return not cls.match(self)
 
   return match
 
@@ -195,14 +205,17 @@
         / 'index.md'
     )
 
   @property
   def extra_template_kwargs(self):
     return dict(
         toctree=self.toctree,
+        symbols_table=self.make_symbols_table(
+            self.symbol.node.documented_childs
+        ),
     )
 
   @property
   def toctree(self) -> str:
     items = []
     for n in self.symbol.node.documented_childs:
       path = n.match.filename.relative_to(self.filename.parent)
@@ -225,15 +238,17 @@
     return pathlib.Path(self.symbol.ctx.alias) / 'index.md'
 
   @property
   def extra_template_kwargs(self):
     return dict(
         **super().extra_template_kwargs,
         import_statement=self.import_statement,
-        symbols_table=self.symbols_table,
+        all_symbols_table=self.make_symbols_table(
+            self.symbol.node.iter_documented_nodes()
+        ),
     )
 
   @property
   def import_statement(self) -> str:
     module_name = self.symbol.ctx.module_name
     alias = self.symbol.ctx.alias
 
@@ -254,31 +269,14 @@
         f"""
         ```{{code-block}}
         {stmt}
         ```
         """
     )
 
-  @property
-  def symbols_table(self):
-    table = md_utils.Table(header=['', '', ''])
-
-    for n in self.symbol.node.iter_documented_nodes():
-      filename = n.match.filename
-      filename = filename.relative_to(self.filename.parent)
-      filename = os.fspath(filename)
-      filename = filename.removesuffix('.md')
-      table.add_row(
-          f'*{n.match.icon}*',
-          f'[{n.symbol.qualname}]({filename})',
-          f'{n.match.docstring_1line}',
-      )
-
-    return table.make()
-
 
 class _ImplicitlyImportedModule(_IsModule):
   """Filter implicitly imported modules."""
 
   documented = False
 
   def match(self) -> bool:
@@ -288,32 +286,20 @@
 class _ExternalModule(_IsModule):
   documented = False
 
   def match(self) -> bool:
     return not self.symbol.belong_to_namespace
 
 
-class _BelongToNamespace(_IsModule):
+class _ApiModule(_IsModule):
+  """Modules or packages."""
 
   def match(self) -> bool:
     return self.symbol.belong_to_namespace
 
-
-class _IsPackage(_IsModule):
-
-  def match(self) -> bool:
-    return self.symbol.is_package
-
-
-class _ApiPackage(_BelongToNamespace, _IsPackage):
-  recurse = True
-
-
-class _ApiModule(_BelongToNamespace, _IsModule):
-
   @property
   def documented(self):
     # Only document when the parent is a package
     return _is_package(self.symbol.parent)
 
   @property
   def recurse(self):
@@ -360,25 +346,14 @@
 
   def match(self):
     import __future__
 
     return isinstance(self.symbol.value, __future__._Feature)
 
 
-# class _ImportedValue(_IsValue):
-
-#   @property
-#   def documented(self):
-#     # Only document imported values when the parent is a package
-#     return _is_package(self.symbol.parent)
-
-#   def match(self):
-#     return self.symbol.is_imported
-
-
 class _DocumentedValue(_IsValue):
 
   @property
   def documented(self):
     # Only document imported values when the parent is a package
     return not self.symbol.is_imported or _is_package(self.symbol.parent)
 
@@ -417,11 +392,11 @@
   icon = 'a'
   template_name = 'attribute'
 
   # TODO(epot): Extract doc from parent
 
 
 def _is_package(module: types.ModuleType) -> bool:
-  # TODO(epot): Could also add custom attribute `__docutil__.is_package` so
-  # standard module behave like package.
+  # Have custom attribute so standard module can behave like package.
+  if hasattr(module, '__apitree__'):
+    return module.__apitree__['is_package']
   return module.__name__ == module.__package__
-  # return pathlib.Path(module.__file__).name == '__init__.py'
```

### Comparing `sphinx-apitree-1.0.0/apitree/tree_extractor.py` & `sphinx_apitree-1.1.0/apitree/tree_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
+import importlib
 import types
 from typing import Iterator
 
 from etils import edc, epy
 
-from apitree import symbol_match
+from apitree import structs, symbol_match
 
 
 @dataclasses.dataclass
 class Node:
   symbol: symbol_match.Symbol
 
   def __post_init__(self):
@@ -52,21 +53,23 @@
     if self.childs:
       child_str = epy.Lines.repr([c for c in self.childs if c.match.documented])
     else:
       child_str = ''
     return f'{self.symbol.name}={type(self.match).__name__}{child_str}'
 
 
-def get_api_tree(module: types.ModuleType, alias: str = ''):
-  ctx = symbol_match.Context(
-      module_name=module.__name__,
-      alias=alias or module.__name__,
-  )
+def get_api_tree(info: structs.ModuleInfo):
+  module = importlib.import_module(info.api)
+
+  # ctx = symbol_match.Context(
+  #     module_name=module.__name__,
+  #     info,
+  # )
   return Node(
       symbol_match.Symbol(
           name=module.__name__,
           value=module,
           parent=None,
           parent_symb=None,
-          ctx=ctx,
+          ctx=info,
       ),
   )
```

### Comparing `sphinx-apitree-1.0.0/pyproject.toml` & `sphinx_apitree-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx-apitree-1.0.0/PKG-INFO` & `sphinx_apitree-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.0.0
+Version: 1.1.0
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -22,27 +22,32 @@
 Project-URL: homepage, https://github.com/conchylicultor/sphinx-apitree
 Project-URL: repository, https://github.com/conchylicultor/sphinx-apitree
 Provides-Extra: dev
 Provides-Extra: ext
 
 # sphinx-apitree
 
+[![Unittests](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml)
+[![PyPI version](https://badge.fury.io/py/sphinx-apitree.svg)](https://badge.fury.io/py/sphinx-apitree)
+
+
 `apitree` is a small library to generate a ready-to-use documentation with minimal friction!
 
 `apitree` takes care of everything, so you can only focus on the code.
 
 ## Usage
 
 In `docs/conf.py`, replace everything by:
 
 ```python
 import apitree
 
 apitree.make_project(
-    project_name='my_module',
+    # e.g. `import visu3d as v3d` -> {'v3d': 'visu3d'}
+    project_name={'alias': 'my_module'},
     globals=globals(),
 )
 ```
 
 Then to generate the doc:
 
 ```sh
@@ -58,28 +63,28 @@
   api/my_module/index
 ```
 
 ## Features
 
 * Theme
 * Auto-generate the API tree, with better features
-  * Do not require `__all__`
+  * Do not require `__all__` (smart detect of which symbols are documented)
   * Add expandable toc tree with all symbols
 * ...
 
 ## Installation in a project
 
 1.  In `pyproject.toml`
 
     ```toml
     [project.optional-dependencies]
     # Installed through `pip install .[docs]`
     docs = [
         # Install `apitree` with all extensions (sphinx, theme,...)
-        "sphinx-apitree[ext] @ https://github.com/conchylicultor/sphinx-apitree",
+        "sphinx-apitree[ext]",
     ]
     ```
 
 1.  In `.readthedocs.yaml`
 
     ```yaml
     sphinx:
@@ -91,11 +96,12 @@
         path: .
         extra_requirements:
             - docs
     ```
 
 ## Examples of projects using apitree
 
-* https://github.com/google-research/visu3d
-* https://github.com/google-research/dataclass_array
-* https://github.com/google-research/etils
+* https://github.com/google-research/visu3d (https://visu3d.readthedocs.io/)
+* https://github.com/google-research/dataclass_array (https://dataclass-array.readthedocs.io/)
+* https://github.com/google-research/etils (https://etils.readthedocs.io/)
+* https://github.com/google-research/kauldron (https://kauldron.readthedocs.io/)
```

