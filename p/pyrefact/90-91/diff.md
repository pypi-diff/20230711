# Comparing `tmp/pyrefact-90.tar.gz` & `tmp/pyrefact-91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-90.tar", last modified: Sun Jul  2 10:07:03 2023, max compression
+gzip compressed data, was "pyrefact-91.tar", last modified: Tue Jul 11 19:09:11 2023, max compression
```

## Comparing `pyrefact-90.tar` & `pyrefact-91.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:07:03.428372 pyrefact-90/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 10:06:45.000000 pyrefact-90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-02 10:07:03.428372 pyrefact-90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-02 10:06:45.000000 pyrefact-90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-02 10:06:45.000000 pyrefact-90/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:07:03.428372 pyrefact-90/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   130630 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13175 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    23378 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/symbolic_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-07-02 10:06:45.000000 pyrefact-90/pyrefact/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:07:03.428372 pyrefact-90/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 10:07:03.000000 pyrefact-90/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:07:03.428372 pyrefact-90/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:07:03.428372 pyrefact-90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-02 10:06:45.000000 pyrefact-90/tests/testing_infra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 19:08:57.000000 pyrefact-91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-11 19:09:11.063552 pyrefact-91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-11 19:08:57.000000 pyrefact-91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 19:08:57.000000 pyrefact-91/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/pyrefact/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27069 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135094 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/logs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13323 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/object_oriented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/symbolic_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/pyrefact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:09:11.063552 pyrefact-91/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-11 19:08:57.000000 pyrefact-91/tests/testing_infra.py
```

### Comparing `pyrefact-90/LICENSE` & `pyrefact-91/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefact-90/PKG-INFO` & `pyrefact-91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefact
-Version: 90
+Version: 91
 Summary: Automated Python refactoring
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2022 OlleLindgren
```

### Comparing `pyrefact-90/README.md` & `pyrefact-91/README.md`

 * *Files identical despite different names*

### Comparing `pyrefact-90/pyproject.toml` & `pyrefact-91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrefact"
-version = "90"
+version = "91"
 description = "Automated Python refactoring"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {email = "olle.ln@outlook.com"},
     {name = "Olle Lindgren"}
```

### Comparing `pyrefact-90/pyrefact/abstractions.py` & `pyrefact-91/pyrefact/abstractions.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,20 +310,21 @@
     imports = [node for node in scope.body if not isinstance(node, import_types)]
     return min((node.lineno for node in imports)) - 1
 
 
 def create_abstractions(source: str) -> str:
     root = core.parse(source)
     global_names = (
-        _scoped_dependencies(root) | tracing.get_imported_names(root) | constants.BUILTIN_FUNCTIONS
+        _scoped_dependencies(root)
+        | tracing.get_imported_names(root)
+        | constants.BUILTIN_FUNCTIONS
+        | {node.name for node in parsing.iter_funcdefs(root)}
+        | {node.name for node in parsing.iter_classdefs(root)}
     )
-    for node in parsing.iter_funcdefs(root):
-        global_names.add(node.name)
-    for node in parsing.iter_classdefs(root):
-        global_names.add(node.name)
+
     replacements = {}
     additions = []
     removals = []
     abstraction_count = 0
 
     function_def_linenos = []
     import_linenos = []
@@ -532,14 +533,22 @@
     template = (
         ast.Constant,
         ast.Dict(keys={ast.Constant}, values={ast.Constant}),
         ast.Set(elts={ast.Constant}),
         ast.Tuple(elts={ast.Constant}),
         ast.List(elts={ast.Constant}),
     )
+    blacklisted_names = (
+        tracing.get_imported_names(root)
+        | tracing.get_defined_names(root)
+        | constants.BUILTIN_FUNCTIONS
+        | constants.PYTHON_KEYWORDS
+    )
+    blacklisted_names |= {name.upper() for name in blacklisted_names}
+    blacklisted_names |= {name.lower() for name in blacklisted_names}
 
     candidates = set(core.walk(root, template))
 
     for fstring in core.walk(root, ast.JoinedStr):
         for node in core.walk(fstring, ast.AST):
             candidates.discard(node)
 
@@ -557,47 +566,54 @@
     for node in candidates:
         code_node_mapping[core.unparse(node)].add(node)
 
     replacements = {}
     additions = set()
 
     i = 0
-    names = {name.id.lower().strip("_") for name in core.walk(root, ast.Name)}
-    while f"pyrefact_overused_constant_{i}" in names and i < 10:
+    while f"pyrefact_overused_constant_{i}" in blacklisted_names and i < 10:
         i += 1
 
-    if f"pyrefact_overused_constant_{i}" in names:
+    if f"pyrefact_overused_constant_{i}" in blacklisted_names:
         return source
 
     for code, nodes in sorted(code_node_mapping.items(), key=lambda t: t[0]):
         if len(nodes) < 5:
             continue
         if len(re.sub(r"\s", "", code)) < 20:
             continue
 
         common_scopes = set.intersection(*(scope_node_definitions[node] for node in nodes))
 
         # root is a Module and has no lineno
         best_common_scope = max(
             common_scopes, key=lambda node: getattr(node, "lineno", 1), default=root
         )
-        variable_name = f"pyrefact_overused_constant_{i}"
+        nodes = list(nodes)
+        if (
+            core.match_template(nodes[0], ast.Constant(value=str))
+            and re.match(r"[a-zA-Z_]\w*", nodes[0].value)
+            and re.sub(r"[^a-zA-Z0-9_]", "", nodes[0].value)
+        ):
+            variable_name = nodes[0].value
+        else:
+            variable_name = f"pyrefact_overused_constant_{i}"
+            i += 1
+
         variable_name = style.rename_variable(
             variable_name, static=best_common_scope is root and root_is_static, private=False
         )
 
         name = ast.Name(id=variable_name)
         assign = core.parse(f"{variable_name} = {code}").body[0]
         assign.lineno = _get_constant_insertion_lineno(best_common_scope)
         assign.col_offset = best_common_scope.body[0].col_offset
         additions.add(assign)
         replacements.update({node: name for node in nodes})
 
-        i += 1
-
     return processing.alter_code(source, root, additions=additions, replacements=replacements)
 
 
 def simplify_if_control_flow(source: str) -> str:
     root = core.parse(source)
 
     # This should run after the first run of breakout_common_code_in_ifs(), so that code that
```

### Comparing `pyrefact-90/pyrefact/constants.py` & `pyrefact-91/pyrefact/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -280,14 +280,16 @@
     "smtpd",
     "sndhdr",
     "spwd",
     "sunau",
     "telnetlib",
     "uu",
     "xdrlib",
+    "pstats",
+    "cProfile",
 ))
 
 BUILTIN_FUNCTIONS = frozenset(name for name in dir(builtins) if name != "_")
 SAFE_CALLABLES = frozenset({
     "ArithmeticError",
     "AssertionError",
     "AttributeError",
@@ -425,15 +427,19 @@
     "sum",
     "super",
     "tuple",
     "type",
     "vars",
     "zip",
 })
-PYTHON_KEYWORDS = frozenset(keyword.kwlist)
+PYTHON_KEYWORDS = frozenset(
+    keyword.kwlist
+    + getattr(keyword, "softkwlist", [])  # Exists on >= 3.9, but empty on 3.9
+    + ["_", "case", "match", "type"]  # keyword.softkwlist as of 3.12b2
+)
 
 PYTHON_VERSION = tuple(sys.version_info)
 
 REVERSE_OPERATOR_MAPPING = MappingProxyType({
     ast.Eq: ast.NotEq,
     ast.NotEq: ast.Eq,
     ast.Gt: ast.LtE,
```

### Comparing `pyrefact-90/pyrefact/core.py` & `pyrefact-91/pyrefact/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import collections
 import dataclasses
 import functools
 import itertools
 import re
 import textwrap
 import traceback
-from typing import Collection, Iterable, Mapping, NamedTuple, Sequence, Set, Tuple
+from typing import Collection, Iterable, List, Mapping, NamedTuple, Sequence, Set, Tuple
 
 from pyrefact import constants, formatting, logs as logger
 
 
 def unparse(node: ast.AST | str) -> str:
     if isinstance(node, str):
         return node  # Hack to allow format_template to accept strings matched by wildcards.
@@ -116,14 +116,78 @@
 
     # Sort in alphabetical order, but always with "root" first.
     fields = tuple(sorted(namedtuple_vars.keys(), key=lambda k: (k != "root", k)))
     namedtuple_type = _make_match_type(fields)
     return namedtuple_type(*(namedtuple_vars[field] for field in fields))
 
 
+def _match_tuple(node: ast.AST, template: Tuple[ast.AST, ...], ignore: Collection[str]) -> Tuple:
+    for child in template:
+        if match := match_template(node, child, ignore=ignore):
+            return match
+
+    return ()
+
+
+def _match_set(node: ast.AST, template: Set[ast.AST], ignore: Collection[str]) -> Tuple:
+    if not isinstance(node, list):
+        return ()
+
+    matches = (match_template(node_child, tuple(template), ignore=ignore) for node_child in node)
+    return merge_matches(node, matches)
+
+
+def _match_list(node: ast.AST, template: List[ast.AST], ignore: Collection[str]) -> Tuple:
+    if not isinstance(node, list):
+        return ()
+    if len(node) != len(template):
+        return ()
+
+    matches = (
+        match_template(child, template_child, ignore=ignore)
+        for child, template_child in zip(node, template)
+    )
+    return merge_matches(node, matches)
+
+
+def _match_wildcard(node: ast.AST, template: Wildcard, ignore: Collection[str]) -> Tuple:
+    namedtuple_type = _make_match_type((template.name,))
+    template_match = match_template(node, template.template, ignore=ignore)
+    return namedtuple_type(template_match[0]) if len(template_match) == 1 else ()
+
+
+def _match_template_vars(
+    node: ast.AST,
+    template: ast.AST,
+    ignore: Collection[str] = frozenset(("lineno", "end_lineno", "col_offset", "end_col_offset")),
+) -> Tuple:
+    t_vars = vars(template)
+    n_vars = vars(node)
+
+    for k in t_vars:
+        if k in ignore:
+            continue
+        if k not in n_vars:
+            return ()
+
+    matches = (
+        match_template(n_vars[key], t_vars[key], ignore=ignore) for key in t_vars.keys() - ignore
+    )
+    return merge_matches(node, matches)
+
+
+@functools.lru_cache(maxsize=10000)
+def _issubclas_cache(obj: type, types: type | Tuple[type, ...]) -> bool:
+    return issubclass(obj, types)
+
+
+def _isinstance_cache(obj: object, types: type | Tuple[type, ...]) -> bool:
+    return _issubclas_cache(type(obj), types)
+
+
 def match_template(
     node: ast.AST,
     template: ast.AST,
     ignore: Collection[str] = frozenset(("lineno", "end_lineno", "col_offset", "end_col_offset")),
 ) -> Tuple:
     """Match a node against a provided ast template.
 
@@ -158,84 +222,54 @@
     # Match x(1) and y(1)
     `ast.Call(func=ast.Name(id=("x", "y")), args=[ast.Constant(value=1)])`
 
     """
     # A type indicates that the node should be an instance of that type,
     # and nothing else. A tuple indicates that the node should be any of
     # the types in it.
-
-    if isinstance(template, type):
-        return (node,) if isinstance(node, template) else ()
+    if _isinstance_cache(template, type):
+        return (node,) if _isinstance_cache(node, template) else ()
 
     # A tuple indicates an or condition; the node must comply with any of
     # the templates in the child.
     # They may all be types for example, which boils down to the traditional
     # isinstance logic.
     # If there are wildcards, the first match is chosen.
-    if isinstance(template, tuple):
-        for child in template:
-            if match := match_template(node, child, ignore=ignore):
-                return match
-        return ()
+    if _isinstance_cache(template, tuple):
+        return _match_tuple(node, template, ignore)
 
     # A set indicates a variable length list, where all elements must match
     # against at least one of the templates in it.
     # If there are wildcards, the first match is chosen.
     # If there are inconsistencies between different elements, the match is discarded.
-    if isinstance(template, set):
-        if not isinstance(node, list):
-            return ()
-        matches = (
-            match_template(node_child, tuple(template), ignore=ignore) for node_child in node
-        )
+    if _isinstance_cache(template, set):
+        return _match_set(node, template, ignore)
 
-        return merge_matches(node, matches)
     # A list indicates that the node must also be a list, and for every
     # element, it must match against the corresponding node in the template.
     # It must also be equal length.
-    if isinstance(template, list):
-        if isinstance(node, list) and len(node) == len(template):
-            matches = (
-                match_template(child, template_child, ignore=ignore)
-                for child, template_child in zip(node, template)
-            )
-
-            return merge_matches(node, matches)
-
-        return ()
+    if _isinstance_cache(template, list):
+        return _match_list(node, template, ignore)
 
     if template is True or template is False or template is None:
         return (node,) if node is template else ()
 
-    if isinstance(template, Wildcard):
-        namedtuple_type = _make_match_type((template.name,))
-        template_match = match_template(node, template.template, ignore=ignore)
-        return namedtuple_type(template_match[0]) if len(template_match) == 1 else ()
-
-    # If the node is not an ast, we presume it is a string or something like
-    # that, and just assert it should be equal.
-    if not isinstance(node, ast.AST):
-        return (node,) if node == template else ()
+    if _isinstance_cache(template, Wildcard):
+        return _match_wildcard(node, template, ignore)
 
-    if not isinstance(node, type(template)):
-        return ()
+    if _isinstance_cache(template, ast.AST):
+        if isinstance(node, type(template)):
+            return _match_template_vars(node, template, ignore=ignore)
 
-    t_vars = vars(template)
-    n_vars = vars(node)
+        return ()
 
-    for k in t_vars:
-        if k in ignore:
-            continue
-        if k not in n_vars:
-            return ()
+    if node == template:
+        return (node,)
 
-    matches = (
-        match_template(n_vars[key], t_vars[key], ignore=ignore) for key in t_vars.keys() - ignore
-    )
-    return merge_matches(node, matches)
+    return ()
 
 
 @functools.lru_cache(maxsize=100)
 def parse(source_code: str) -> ast.AST:
     """Parse python source code and cache
 
     Args:
@@ -636,14 +670,17 @@
     line_start_charnos = _get_line_start_charnos(source)
     if match_template(node, ast.AST(decorator_list=list)) and node.decorator_list:
         start = min(node.decorator_list, key=lambda n: (n.lineno, n.col_offset))
     else:
         start = node
 
     start_charno = line_start_charnos[start.lineno - 1] + start.col_offset
+    if getattr(node, "end_lineno", None) is None:
+        return Range(start_charno, start_charno)
+
     end_charno = line_start_charnos[node.end_lineno - 1] + node.end_col_offset
 
     code = source[start_charno:end_charno]
     if code[0] == " ":
         whitespace = max(re.findall(r"\A^ *", code), key=len)
         start_charno += len(whitespace)
     if code[-1] == " ":
@@ -665,25 +702,28 @@
     ):
         start_charno += 2
         end_charno += 2
 
     return Range(start_charno, end_charno)
 
 
-def get_code(node: ast.AST, source: str) -> str:
+def get_code(node: ast.AST | Range, source: str) -> str:
     """Get python code from ast
 
     Args:
         node (ast.AST): ast to get code from
         source (str): Python source code that ast was parsed from
 
     Returns:
         str: Python source code
 
     """
+    if isinstance(node, Range):
+        return source[node.start : node.end]
+
     start_charno, end_charno = get_charnos(node, source)
     return source[start_charno:end_charno]
 
 
 def literal_value(node: ast.AST) -> bool:
     if has_side_effect(node):
         raise ValueError("Cannot find a deterministic value for a node with a side effect")
```

### Comparing `pyrefact-90/pyrefact/fixes.py` & `pyrefact-91/pyrefact/fixes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import copy
 import itertools
 import re
 import textwrap
 from pathlib import Path
 from typing import Collection, Iterable, List, Literal, Mapping, Sequence, Tuple
 
-import rmspace
 from pyrefact import (
     abstractions,
     constants,
     core,
     formatting,
     logs as logger,
     parsing,
@@ -68,119 +67,14 @@
         n_end = (refnode.end_lineno, refnode.end_col_offset)
         if end < n_start:
             yield refnode
         elif is_maybe_unordered_scope and n_end < start:
             yield refnode
 
 
-def _get_variable_name_substitutions(
-    ast_tree: ast.AST, source: str, preserve: Collection[str]
-) -> Mapping[ast.AST, str]:
-    renamings = collections.defaultdict(set)
-    classdefs: List[ast.ClassDef] = []
-    funcdefs: List[ast.FunctionDef] = []
-    for node in parsing.iter_classdefs(ast_tree):
-        name = node.name
-        substitute = style.rename_class(
-            name, private=parsing.is_private(name) or name not in preserve
-        )
-        classdefs.append(node)
-        renamings[node].add(substitute)
-        for refnode in _get_uses_of(node, ast_tree, source):
-            renamings[refnode].add(substitute)
-
-    typevars = set()
-    for node in parsing.iter_typedefs(ast_tree):
-        assert len(node.targets) == 1
-        target = node.targets[0]
-        assert isinstance(target, (ast.Name, ast.Attribute))
-        typevars.add(target)
-        for refnode in _get_uses_of(target, ast_tree, source):
-            typevars.add(refnode)
-
-    for node in parsing.iter_funcdefs(ast_tree):
-        name = node.name
-        substitute = style.rename_variable(
-            name, private=parsing.is_private(name) or name not in preserve, static=False
-        )
-        funcdefs.append(node)
-        renamings[node].add(substitute)
-        for refnode in _get_uses_of(node, ast_tree, source):
-            renamings[refnode].add(substitute)
-
-    for node in parsing.iter_assignments(ast_tree):
-        if node in typevars:
-            substitute = style.rename_class(node.id, private=parsing.is_private(node.id))
-        else:
-            substitute = style.rename_variable(
-                node.id, private=parsing.is_private(node.id), static=True
-            )
-        renamings[node].add(substitute)
-        for refnode in _get_uses_of(node, ast_tree, source):
-            renamings[refnode].add(substitute)
-
-    while funcdefs or classdefs:
-        for partial_tree in classdefs.copy():
-            classdefs.remove(partial_tree)
-            for node in parsing.iter_classdefs(partial_tree):
-                name = node.name
-                classdefs.append(node)
-                substitute = style.rename_class(name, private=parsing.is_private(name))
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-            for node in parsing.iter_funcdefs(partial_tree):
-                name = node.name
-                # Don't rename magic members, don't rename if there is inheritance.
-                if partial_tree.bases or parsing.is_magic_method(node):
-                    renamings[node] = {name}
-                funcdefs.append(node)
-                substitute = style.rename_variable(
-                    name, private=parsing.is_private(name), static=False
-                )
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-            for node in parsing.iter_assignments(partial_tree):
-                name = node.id
-                # Don't rename magic members, don't rename if there is inheritance.
-                if partial_tree.bases or (name.startswith("__") and name.endswith("__")):
-                    renamings[node] = {name}
-                substitute = style.rename_variable(
-                    name, private=parsing.is_private(name), static=False
-                )
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-        for partial_tree in funcdefs.copy():
-            funcdefs.remove(partial_tree)
-            for node in parsing.iter_classdefs(partial_tree):
-                name = node.name
-                classdefs.append(node)
-                substitute = style.rename_class(name, private=False)
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-            for node in parsing.iter_funcdefs(partial_tree):
-                name = node.name
-                funcdefs.append(node)
-                substitute = style.rename_variable(name, private=False, static=False)
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-            for node in parsing.iter_assignments(partial_tree):
-                name = node.id
-                substitute = style.rename_variable(name, private=False, static=False)
-                renamings[node].add(substitute)
-                for refnode in _get_uses_of(node, partial_tree, source):
-                    renamings[refnode].add(substitute)
-
-    return renamings
-
-
 def _get_variable_re_pattern(variable) -> str:
     return r"(?<![A-Za-z_\.])" + variable + r"(?![A-Za-z_])"
 
 
 def _get_func_name_start_end(
     node: ast.FunctionDef | ast.AsyncFunctionDef | ast.ClassDef, source: str
 ) -> Tuple[int, int]:
@@ -365,78 +259,41 @@
     ))
     if isinstance(node, ast.Import):
         return f"import {names}"
 
     return f"from {'.' * node.level}{node.module or ''} import {names}"
 
 
-def _remove_unused_imports(
-    ast_tree: ast.Module, source: str, unused_imports: Collection[str]
-) -> str:
-    completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
-        ast_tree, unused_imports
-    )
-    if completely_unused_imports:
-        logger.debug("Removing unused imports")
-        source = processing.remove_nodes(source, completely_unused_imports, ast_tree)
-        if not partially_unused_imports:
-            return source
-        ast_tree = core.parse(source)
-        completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
-            ast_tree, unused_imports
-        )
-
-    if completely_unused_imports:
-        raise RuntimeError("Failed to remove unused imports")
-
-    # For every import, construct what we would like it to look like with redundant stuff removed, find the old
-    # version of it, and replace it.
-
-    # Iterate from bottom to top of file, so we don't have to re-calculate the linenos etc.
-    for node in sorted(
-        partially_unused_imports,
-        key=lambda n: (n.lineno, n.col_offset, n.end_lineno, n.end_col_offset),
-        reverse=True,
-    ):
-        start, end = core.get_charnos(node, source)
-        code = source[start:end]
-        replacement = _construct_import_statement(node, unused_imports)
-        logger.debug("Replacing:\n{old}\nWith:\n{new}", old=code, new=replacement)
-        source = source[:start] + replacement + source[end:]
-
-    return source
-
-
+@processing.fix
 def remove_unused_imports(source: str) -> str:
     """Remove unused imports from source code.
 
     Args:
         source (str): Python source code
 
     Returns:
         str: Source code, with added imports removed
     """
-    ast_tree = core.parse(source)
-    unused_imports = _get_unused_imports(ast_tree)
-    if unused_imports:
-        source = _remove_unused_imports(ast_tree, source, unused_imports)
-
-    return source
+    root = core.parse(source)
+    unused_imports = _get_unused_imports(root)
+    completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
+        root, unused_imports
+    )
 
+    for node in completely_unused_imports:
+        yield node, None
 
-def fix_tabs(source: str) -> str:
-    """Replace tabs with 4 spaces in source code
+    # For every import, construct what we would like it to look like with redundant stuff removed, find the old
+    # version of it, and replace it.
 
-    Args:
-        source (str): Python source code
+    # Iterate from bottom to top of file, so we don't have to re-calculate the linenos etc.
+    for node in partially_unused_imports:
+        yield node, _construct_import_statement(node, unused_imports)
 
-    Returns:
-        str: Formatted source code
-    """
-    return re.sub(r"\t", " " * 4, source)
+    return source
 
 
 def fix_too_many_blank_lines(source: str) -> str:
     # At module level, remove all above 2 blank lines
     source = re.sub(r"(\n\s*){3,}\n", "\n" * 3, source)
 
     # At EOF, remove all newlines and whitespace above 1
@@ -444,27 +301,15 @@
 
     # At non-module (any indented) level, remove all newlines above 1, preserve indent
     source = re.sub(r"(\n\s*){2,}(\n\s+)(?=[^\n\s])", r"\n\g<2>", source)
 
     return source
 
 
-def fix_rmspace(source: str) -> str:
-    """Remove trailing whitespace from source code.
-
-    Args:
-        source (str): Python source code
-
-    Returns:
-        str: Source code, without trailing whitespace
-    """
-    return rmspace.format_str(source)
-
-
-@processing.fix
+@processing.fix(max_iter=1)
 def fix_line_lengths(source: str, *, max_line_length: int = 100) -> str:
     root = core.parse(source)
 
     formatted_nodes = set()
     formatted_ranges = set()
 
     subscopes = []
@@ -511,14 +356,15 @@
 
         new_code = formatting.collapse_trailing_parentheses(new_code)
         if new_code != formatting.collapse_trailing_parentheses(current_code):
             yield source_range, new_code
             formatted_ranges.add(source_range)
 
 
+@processing.fix
 def align_variable_names_with_convention(
     source: str, preserve: Collection[str] = frozenset()
 ) -> str:
     """Align variable names with normal convention
 
     Class names should have CamelCase names
     Non-static variables and functions should have snake_case names
@@ -531,23 +377,181 @@
     Args:
         source (str): Python source code
 
     Returns:
         str: Source code, where all variable names comply with normal convention
     """
     ast_tree = core.parse(source)
-    renamings = _get_variable_name_substitutions(ast_tree, source, preserve)
+    renamings = collections.defaultdict(set)
+    classdefs: List[ast.ClassDef] = []
+    funcdefs: List[ast.FunctionDef] = []
+    for node in parsing.iter_classdefs(ast_tree):
+        name = node.name
+        substitute = style.rename_class(
+            name, private=parsing.is_private(name) or name not in preserve
+        )
+        classdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, source):
+            renamings[refnode].add(substitute)
 
-    if renamings:
-        source = _fix_variable_names(source, renamings, preserve)
+    typevars = set()
+    for node in parsing.iter_typedefs(ast_tree):
+        assert len(node.targets) == 1
+        target = node.targets[0]
+        assert isinstance(target, (ast.Name, ast.Attribute))
+        typevars.add(target)
+        for refnode in _get_uses_of(target, ast_tree, source):
+            typevars.add(refnode)
 
-    return source
+    for node in parsing.iter_funcdefs(ast_tree):
+        name = node.name
+        substitute = style.rename_variable(
+            name, private=parsing.is_private(name) or name not in preserve, static=False
+        )
+        funcdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, source):
+            renamings[refnode].add(substitute)
+
+    for node in parsing.iter_assignments(ast_tree):
+        if node in typevars:
+            substitute = style.rename_class(node.id, private=parsing.is_private(node.id))
+        else:
+            substitute = style.rename_variable(
+                node.id, private=parsing.is_private(node.id), static=True
+            )
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, source):
+            renamings[refnode].add(substitute)
+
+    while funcdefs or classdefs:
+        for partial_tree in classdefs.copy():
+            classdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = style.rename_class(name, private=parsing.is_private(name))
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                # Don't rename magic members, don't rename if there is inheritance.
+                if partial_tree.bases or parsing.is_magic_method(node):
+                    renamings[node] = {name}
+                funcdefs.append(node)
+                substitute = style.rename_variable(
+                    name, private=parsing.is_private(name), static=False
+                )
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                # Don't rename magic members, don't rename if there is inheritance.
+                if partial_tree.bases or (name.startswith("__") and name.endswith("__")):
+                    renamings[node] = {name}
+                substitute = style.rename_variable(
+                    name, private=parsing.is_private(name), static=False
+                )
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+        for partial_tree in funcdefs.copy():
+            funcdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = style.rename_class(name, private=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                funcdefs.append(node)
+                substitute = style.rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                substitute = style.rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, source):
+                    renamings[refnode].add(substitute)
+
+    blacklisted_names = (
+        tracing.get_imported_names(ast_tree)
+        | tracing.get_defined_names(ast_tree)
+        | constants.BUILTIN_FUNCTIONS
+        | constants.PYTHON_KEYWORDS
+    )
+    renamings = {
+        node: list(substitutes)[0]
+        for node, substitutes in renamings.items()
+        if len(substitutes) == 1 and blacklisted_names.isdisjoint(substitutes)
+    }
+    substitute_node_renamings = collections.defaultdict(set)
+    for node, substitute in renamings.items():
+        substitute_node_renamings[substitute].add(node)
+
+    transaction = 0
+    for substitute, nodes in substitute_node_renamings.items():
+        replacements = []
+        for node in nodes:
+            if isinstance(node, ast.Name):
+                if node.id == substitute:
+                    continue
+                replacement = ast.Name(id=substitute)
+            elif isinstance(node, ast.FunctionDef):
+                if node.name == substitute:
+                    continue
+                replacement = ast.FunctionDef(
+                    name=substitute,
+                    args=node.args,
+                    body=node.body,
+                    decorator_list=node.decorator_list,
+                    returns=node.returns,
+                    type_comment=node.type_comment,
+                )
+            elif isinstance(node, ast.AsyncFunctionDef):
+                if node.name == substitute:
+                    continue
+                replacement = ast.AsyncFunctionDef(
+                    name=substitute,
+                    args=node.args,
+                    body=node.body,
+                    decorator_list=node.decorator_list,
+                    returns=node.returns,
+                    type_comment=node.type_comment,
+                )
+            elif isinstance(node, ast.ClassDef):
+                if node.name == substitute:
+                    continue
+                replacement = ast.ClassDef(
+                    name=substitute,
+                    bases=node.bases,
+                    keywords=node.keywords,
+                    body=node.body,
+                    decorator_list=node.decorator_list,
+                )
+            else:
+                logger.error("Renaming not implemented for node {} of type {}", node, type(node))
+                replacements.clear()
+                break
+
+            ast.fix_missing_locations(replacement)
 
+            yield node, replacement, transaction
 
-@processing.fix(restart_on_replace=True)
+        transaction += 1
+
+
+@processing.fix
 def undefine_unused_variables(source: str, preserve: Collection[str] = frozenset()) -> str:
     """Remove definitions of unused variables
 
     Args:
         source (str): Python source code
         preserve (Collection[str], optional): Variable names to preserve
 
@@ -750,37 +754,31 @@
 
     Returns:
         bool: True if the node is a pointless string statement.
     """
     return core.match_template(node, ast.Expr(value=ast.Constant(value=str)))
 
 
+@processing.fix
 def delete_pointless_statements(source: str) -> str:
     """Delete pointless statements with no side effects from code
 
     Args:
         source (str): Python source code.
 
     Returns:
         str: Modified code
     """
     ast_tree = core.parse(source)
-    delete = []
     safe_callables = parsing.safe_callable_names(ast_tree)
     for node in itertools.chain([ast_tree], parsing.iter_bodies_recursive(ast_tree)):
         for i, child in enumerate(node.body):
             if not core.has_side_effect(child, safe_callables):
                 if i > 0 or not _is_pointless_string(child):  # Docstring
-                    delete.append(child)
-
-    if delete:
-        logger.debug("Removing pointless statements")
-        source = processing.remove_nodes(source, delete, ast_tree)
-
-    return source
+                    yield child, None
 
 
 def _iter_unreachable_nodes(body: Iterable[ast.AST]) -> Iterable[ast.AST]:
     after_block = False
     for node in body:
         if after_block:
             yield node
@@ -855,53 +853,55 @@
         internal_usages = set(
             core.walk(def_node, ast.Name(ctx=ast.Load, id=(def_node.name, "self", "cls")))
         )
         if not usages - internal_usages:
             yield def_node, None
 
 
+@processing.fix
 def delete_unreachable_code(source: str) -> str:
     """Find and delete dead code.
 
     Args:
         source (str): Python source code
 
     Returns:
         str: Source code with dead code deleted
     """
     root = core.parse(source)
 
-    delete = set()
+    transaction = 0
     for node in parsing.iter_bodies_recursive(root):
         if not isinstance(node, (ast.If, ast.While)):
-            delete.update(_iter_unreachable_nodes(node.body))
+            for unreachable_node in _iter_unreachable_nodes(node.body):
+                yield unreachable_node, None, transaction
+
+            transaction += 1
             continue
 
         try:
             test_value = core.literal_value(node.test)
         except ValueError:
             continue
 
         if isinstance(node, ast.While) and not test_value:
-            delete.add(node)
+            yield node, None, transaction
             continue
 
         if isinstance(node, ast.If):
             if test_value and node.body:
-                delete.update(node.orelse)
+                for _ in node.orelse:
+                    yield node, None, transaction
             elif not test_value and node.orelse:
-                delete.update(node.body)
+                for _ in node.body:
+                    yield node, None, transaction
             else:
-                delete.add(node)
-
-    if delete:
-        logger.debug("Removing unreachable code")
-        source = processing.remove_nodes(source, delete, root)
+                yield node, None, transaction
 
-    return source
+            transaction += 1
 
 
 def _get_package_names(node: ast.Import | ast.ImportFrom):
     if isinstance(node, ast.ImportFrom):
         return [node.module]
 
     return [alias.name for alias in node.names]
@@ -1036,15 +1036,15 @@
         source = _fix_variable_names(source, node_renamings, preserve)
     if delete:
         source = processing.remove_nodes(source, delete, root)
 
     return source
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def remove_redundant_else(source: str) -> str:
     """Remove redundante else and elif statements in code.
 
     Args:
         source (str): Python source code
 
     Returns:
@@ -1061,16 +1061,16 @@
 
         if core.match_template(node.orelse, [ast.If]):
             (start, end) = core.get_charnos(node.orelse[0], source)
             orelse = source[start:end]
             if orelse.startswith("elif"):  # Regular elif
                 modified_orelse = re.sub("^elif", "if", orelse)
 
-                source = source[:start] + modified_orelse + source[end:]
                 yield core.Range(start, end), modified_orelse
+                continue
 
             # Otherwise it's an else: if:, which is handled below
 
         # else
 
         ranges = [core.get_charnos(child, source) for child in node.orelse]
         start = min((s for (s, _) in ranges))
@@ -1177,29 +1177,27 @@
         return False
     if orelse_blocking and not body_blocking:
         return True
     body_branches = _count_branches(body)
     orelse_branches = _count_branches(orelse)
     if orelse_blocking and body_blocking and body_branches >= 2 * orelse_branches:
         return True
-    if isinstance(orelse[0], (ast.Return, ast.Continue, ast.Break)) and len(body) > 3:
-        return True
 
-    return False
+    return isinstance(orelse[0], (ast.Return, ast.Continue, ast.Break)) and len(body) > 3
 
 
 def _sequential_similar_ifs(source: str, root: ast.AST) -> Collection[ast.If]:
     return set.union(
         set(),
         *map(set, parsing.iter_similar_nodes(root, source, ast.If, count=2, length=15)),
         *map(set, parsing.iter_similar_nodes(root, source, ast.If, count=3, length=10)),
     )
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def _swap_explicit_if_else(source: str) -> str:
     root = core.parse(source)
     sequential_similar_ifs = _sequential_similar_ifs(source, root)
 
     for stmt, body, orelse in _iter_explicit_if_elses(root):
         if isinstance(stmt.test, ast.NamedExpr):
             continue
@@ -1418,18 +1416,20 @@
 @processing.fix
 def replace_for_loops_with_dict_comp(source: str) -> str:
     assign_template = ast.Assign(
         value=core.Wildcard("value", (ast.Dict, ast.DictComp)),
         targets=[ast.Name(id=core.Wildcard("target", str))],
     )
 
+    transaction = 0
     root = core.parse(source)
     for (_, target, value), (n2,) in core.walk_sequence(root, assign_template, ast.For):
         body_node = n2
         generators = []
+        transaction += 1
 
         while core.match_template(
             body_node, (ast.For(body=[object]), ast.If(body=[object], orelse=[]))
         ):
             if isinstance(body_node, ast.If):
                 generators[-1].ifs.append(body_node.test)
             elif isinstance(body_node, ast.For):
@@ -1451,42 +1451,44 @@
         ):
             continue
 
         comp = ast.DictComp(
             key=body_node.targets[0].slice, value=body_node.value, generators=generators
         )
         if core.match_template(value, ast.Dict(values=[], keys=[])):
-            yield value, comp
-            yield n2, None
+            yield value, comp, transaction
+            yield n2, None, transaction
         elif core.match_template(value, ast.Dict(values=list, keys={None})):
-            yield value, ast.Dict(keys=value.keys + [None], values=value.values + [comp])
-            yield n2, None
+            yield value, ast.Dict(keys=value.keys + [None], values=value.values + [comp]), transaction
+            yield n2, None, transaction
         elif core.match_template(value, ast.Dict(values=list, keys=list)):
-            yield value, ast.Dict(keys=[None, None], values=[value, comp])
-            yield n2, None
+            yield value, ast.Dict(keys=[None, None], values=[value, comp]), transaction
+            yield n2, None, transaction
         elif isinstance(value, ast.DictComp):
-            yield value, ast.Dict(keys=[None, None], values=[value, comp])
-            yield n2, None
+            yield value, ast.Dict(keys=[None, None], values=[value, comp]), transaction
+            yield n2, None, transaction
 
 
 @processing.fix
 def replace_for_loops_with_set_list_comp(source: str) -> str:
     assign_template = ast.Assign(
         value=core.Wildcard("value", object), targets=[ast.Name(id=core.Wildcard("target", str))]
     )
     for_template = ast.For(body=[object])
     if_template = ast.If(body=[object], orelse=[])
 
     set_init_template = ast.Call(func=ast.Name(id="set"), args=[], keywords=[])
     list_init_template = ast.List(elts=[])  # list() should have been replaced by [] elsewhere.
 
+    transaction = 0
     root = core.parse(source)
     for (_, target, value), (n2,) in core.walk_sequence(root, assign_template, for_template):
         body_node = n2
         generators = []
+        transaction += 1
 
         while core.match_template(body_node, (for_template, if_template)):
             if isinstance(body_node, ast.If):
                 generators[-1].ifs.append(body_node.test)
             elif isinstance(body_node, ast.For):
                 generators.append(
                     ast.comprehension(
@@ -1515,40 +1517,41 @@
             if core.match_template(value, list_init_template) and (template_match.attr == "append"):
                 comp_type = ast.ListComp
             elif core.match_template(value, set_init_template) and (template_match.attr == "add"):
                 comp_type = ast.SetComp
             else:
                 continue
 
-            yield value, comp_type(elt=body_node.value.args[0], generators=generators)
-            yield n2, None
+            yield value, comp_type(elt=body_node.value.args[0], generators=generators), transaction
+            yield n2, None, transaction
 
         elif core.match_template(body_node, augass_template):
             if isinstance(value, ast.List):
                 replacement = ast.ListComp(elt=body_node.value, generators=generators)
             else:
                 comprehension = ast.GeneratorExp(elt=body_node.value, generators=generators)
                 replacement = ast.Call(func=ast.Name(id="sum"), args=[comprehension], keywords=[])
 
             try:
                 if not core.literal_value(value):
                     if isinstance(body_node.op, ast.Sub):
                         replacement = ast.UnaryOp(op=body_node.op, operand=replacement)
-                    yield value, replacement
-                    yield n2, None
+                    yield value, replacement, transaction
+                    yield n2, None, transaction
                     continue
 
             except ValueError:
                 pass
 
             replacement = ast.BinOp(left=value, op=body_node.op, right=replacement)
-            yield value, replacement
-            yield n2, None
+            yield value, replacement, transaction
+            yield n2, None, transaction
 
 
+@processing.fix
 def inline_math_comprehensions(source: str) -> str:
     root = core.parse(source)
 
     replacements = {}
     blacklist = set()
 
     assign_template = ast.Assign(targets=[core.Wildcard("target", ast.Name)])
@@ -1607,18 +1610,18 @@
                         replacements[use] = value
                     break
 
     for assignment in blacklist:
         if assignment in replacements:
             del replacements[assignment]
 
-    return processing.replace_nodes(source, replacements)
+    yield from replacements.items()
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def simplify_transposes(source: str) -> str:
     find = "zip(*zip(*{{value}}))"
     replace = "{{value}}"
     yield from processing.find_replace(source, find, replace)
 
     find = "zip(*{{value}}.T)"
     replace = "{{value}}"
@@ -1656,15 +1659,15 @@
     for node in filter(parsing.is_transpose_operation, itertools.chain(calls, attributes)):
         first_transpose_target = parsing.transpose_target(node)
         if parsing.is_transpose_operation(first_transpose_target):
             second_transpose_target = parsing.transpose_target(first_transpose_target)
             yield node, second_transpose_target
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def remove_dead_ifs(source: str) -> str:
     root = core.parse(source)
 
     for node in core.walk(root, (ast.If, ast.While, ast.IfExp)):
         try:
             value = core.literal_value(node.test)
         except ValueError:
@@ -1770,22 +1773,23 @@
             continue
 
         if isinstance(node, ast.DictComp):
             yield (node, ast.Dict(keys=[], values=[]))
             continue
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def delete_commented_code(source: str) -> str:
     matches = list(re.finditer(r"(?<![^\n])(\s*(#.*))+", source))
     root = core.parse(source)
-    code_string_ranges = {
+    code_ranges = [
         core.get_charnos(node, source)
         for node in core.walk(root, (ast.Constant(value=str), ast.JoinedStr))
-    }
+    ]
+    removed_ranges = []
     for commented_block in matches:
         start = commented_block.start()
         end = commented_block.end()
         start_offset = 0
         end_offset = 0
 
         line_lengths = [len(line) for line in commented_block.group().splitlines(keepends=True)]
@@ -1794,21 +1798,19 @@
             for se in range(len(line_lengths)):
                 if si + se >= len(line_lengths):
                     continue
 
                 start_offset = sum(line_lengths[:si]) if si > 0 else 0
                 end_offset = sum(line_lengths[-se:]) if se > 0 else 0
 
-                selection_end = end - end_offset
-                selection_start = start + start_offset
+                removed_range = core.Range(start + start_offset, end - end_offset)
 
-                if any(
-                    node_start <= selection_end and selection_start <= node_end
-                    for node_start, node_end in code_string_ranges
-                ):
+                if any(removed_range & other for other in removed_ranges):
+                    continue
+                if any(removed_range & other for other in code_ranges):
                     continue
 
                 uncommented_block = re.sub(
                     r"(?<![^\n])(\s*#)", "", source[start + start_offset : end - end_offset]
                 )
                 indentation_lengths = [
                     x.end() - x.start() for x in re.finditer("(?<![^\n]) +", uncommented_block)
@@ -1851,15 +1853,16 @@
                 if any(
                     name.id in {"pylint", "mypy", "flake8", "noqa", "type"}
                     for annassign in core.walk(parsed_content, ast.AnnAssign)
                     for name in core.walk(annassign, ast.Name)
                 ):
                     continue
 
-                yield core.Range(start + start_offset, end - end_offset), None
+                yield removed_range, None
+                removed_ranges.append(removed_range)
 
 
 @processing.fix
 def replace_with_filter(source: str) -> str:
     find_positive = """
     for {{target}} in {{iter}}:
         if {{target}}:
@@ -1961,20 +1964,22 @@
 def implicit_defaultdict(source: str) -> str:
     assign_template = ast.Assign(
         targets=[core.Wildcard("target", ast.Name)],
         value=core.Wildcard("value", ast.Dict(keys=[], values=[])),
     )
     if_template = ast.If(body=[object], orelse=[])
 
+    transaction = 0
     root = core.parse(source)
     for (_, target, value), (n2,) in core.walk_sequence(root, assign_template, ast.For):
         loop_replacements = {}
         loop_removals = set()
         subscript_calls = set()
         consistent = True
+        transaction += 1
 
         for (condition,), (append,) in core.walk_sequence(n2, if_template, ast.Expr):
             try:
                 (key, obj, negative) = _get_contains_args(condition.test)
                 (f_obj, f_key, f_value) = _get_assign_functions(condition.body[0])
                 (t_obj, t_call, t_key, _) = _get_subscript_functions(append)
             except ValueError:
@@ -2040,31 +2045,36 @@
             }:
                 loop_replacements[condition] = on_true
                 continue
 
         if not consistent:
             continue
 
+        replacements = []
+
         if subscript_calls and subscript_calls <= {"add", "update"}:
-            yield from loop_replacements.items()
-            yield from zip(loop_removals, itertools.repeat(None))
-            yield value, ast.Call(
+            replacements.extend(loop_replacements.items())
+            replacements.extend(zip(loop_removals, itertools.repeat(None)))
+            replacements.append((value, ast.Call(
                 func=ast.Attribute(value=ast.Name(id="collections"), attr="defaultdict"),
                 args=[ast.Name(id="set")],
                 keywords=[],
-            )
+            )))
 
         if subscript_calls and subscript_calls <= {"append", "extend"}:
-            yield from loop_replacements.items()
-            yield from zip(loop_removals, itertools.repeat(None))
-            yield value, ast.Call(
+            replacements.extend(loop_replacements.items())
+            replacements.extend(zip(loop_removals, itertools.repeat(None)))
+            replacements.append((value, ast.Call(
                 func=ast.Attribute(value=ast.Name(id="collections"), attr="defaultdict"),
                 args=[ast.Name(id="list")],
                 keywords=[],
-            )
+            )))
+
+        for before, after in replacements:
+            yield before, after, transaction
 
 
 @processing.fix
 def _replace_lambda_with_literal(source: str) -> str:
     for find, replace in (
         ("lambda: []", "list"),
         ("lambda: {}", "dict"),
@@ -2114,19 +2124,18 @@
 
         if not core.match_template(call_keywords, expected_call_keywords):
             continue
 
         yield replacement_range, replacement
 
 
+@processing.fix
 def simplify_redundant_lambda(source: str) -> str:
-    source = _replace_lambda_with_literal(source)
-    source = _replace_lambda_with_function(source)
-
-    return source
+    yield from _replace_lambda_with_literal._fix_func(source)
+    yield from _replace_lambda_with_function._fix_func(source)
 
 
 def _is_same_code(*nodes: ast.AST) -> bool:
     return len({core.unparse(node) for node in nodes}) == 1
 
 
 def _all_branches(
@@ -2284,15 +2293,15 @@
             and code[0] in "'\""
             and "\\" in code
             and not any(sequence in code for sequence in valid_escape_sequences)
         ):
             yield node, "r" + code
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def replace_filter_lambda_with_comp(source: str) -> str:
     """Replace filter(lambda ..., iterable) with equivalent list comprehension
 
     Args:
         source (str): Python source code
 
     Returns:
@@ -2317,15 +2326,15 @@
     ):
         if any(replacement_range & for_range for for_range in for_ranges):
             continue
 
         yield replacement_range, replacement
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def replace_map_lambda_with_comp(source: str) -> str:
     """Replace map(lambda ..., iterable) with equivalent list comprehension
 
     Args:
         source (str): Python source code
 
     Returns:
@@ -2368,15 +2377,15 @@
             yield node, ast.Compare(
                 left=compare.left,
                 ops=[constants.REVERSE_OPERATOR_MAPPING[type(compare.ops[0])]()],
                 comparators=compare.comparators,
             )
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def merge_chained_comps(source: str) -> str:
     root = core.parse(source)
 
     template = ast.AST(
         elt=object,
         generators=[
             ast.comprehension(
@@ -2409,15 +2418,15 @@
                     ifs=template_match.ifs_inner + template_match.ifs_outer,
                     is_async=0,
         )],)
 
         yield template_match.root, replacement
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def remove_redundant_comprehension_casts(source: str) -> str:
     root = core.parse(source)
 
     template = ast.Call(
         func=ast.Name(id=core.Wildcard("func", ("list", "set", "iter"))),
         args=[core.Wildcard("comp", (ast.GeneratorExp, ast.ListComp, ast.SetComp))],
         keywords=[],
@@ -2445,15 +2454,15 @@
             yield node, comp
         if func == "set":
             yield node, equivalent_setcomp
         if func in {"list", "iter"}:
             yield node, ast.Call(func=ast.Name(id=func), args=[equivalent_setcomp], keywords=[])
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def remove_redundant_chain_casts(source: str) -> str:
     root = core.parse(source)
 
     template = ast.Call(
         func=ast.Name(id=core.Wildcard("func_outer", ("list", "set", "iter", "tuple"))),
         args=[
             ast.Call(
@@ -2494,26 +2503,26 @@
             targets=[
                 ast.Subscript(
                     value=target_template, slice=core.Wildcard("key", object, common=False)
             )],
             value=core.Wildcard("value", object, common=False),
     ),]
 
-    for first, *matches in core.walk_sequence(root, *template, expand_last=True):
+    for transaction, (first, *matches) in enumerate(core.walk_sequence(root, *template, expand_last=True)):
         replacement = ast.Assign(
             targets=[first.target],
             value=ast.Dict(
                 keys=first.keys + [m.key for m in matches],
                 values=first.values + [m.value for m in matches],
             ),
             lineno=first.target.lineno,
         )
-        yield first.root, replacement
+        yield first.root, replacement, transaction
         for m in matches:
-            yield m.root, None
+            yield m.root, None, transaction
 
 
 @processing.fix
 def replace_dict_update_with_dict_literal(source: str) -> str:
     root = core.parse(source)
 
     target_template = core.Wildcard("target", ast.Name(id=str))
@@ -2525,26 +2534,26 @@
         ast.Assign(targets=[target_template], value=value_template),
         ast.Expr(
             value=ast.Call(
                 func=ast.Attribute(value=target_template),
                 args=[core.Wildcard("other", object, common=False)],
     )),]
 
-    for first, *matches in core.walk_sequence(root, *template, expand_last=True):
+    for transaction, (first, *matches) in enumerate(core.walk_sequence(root, *template, expand_last=True)):
         replacement = ast.Assign(
             targets=[first.target],
             value=ast.Dict(
                 keys=first.keys + [None] * len(matches),
                 values=first.values + [m.other for m in matches],
             ),
             lineno=first.target.lineno,
         )
-        yield first.root, replacement
+        yield first.root, replacement, transaction
         for m in matches:
-            yield m.root, None
+            yield m.root, None, transaction
 
 
 @processing.fix
 def replace_dictcomp_assign_with_dict_literal(source: str) -> str:
     root = core.parse(source)
 
     target_template = core.Wildcard("target", ast.Name(id=str))
@@ -2554,26 +2563,26 @@
             targets=[
                 ast.Subscript(
                     value=target_template, slice=core.Wildcard("key", object, common=False)
             )],
             value=core.Wildcard("value", object, common=False),
     ),]
 
-    for first, *matches in core.walk_sequence(root, *template, expand_last=True):
+    for transaction, (first, *matches) in enumerate(core.walk_sequence(root, *template, expand_last=True)):
         replacement = ast.Assign(
             targets=[first.target],
             value=ast.Dict(
                 keys=[None] + [m.key for m in matches],
                 values=[first.root.value] + [m.value for m in matches],
             ),
             lineno=first.target.lineno,
         )
-        yield first.root, replacement
+        yield first.root, replacement, transaction
         for m in matches:
-            yield m.root, None
+            yield m.root, None, transaction
 
 
 @processing.fix
 def replace_dictcomp_update_with_dict_literal(source: str) -> str:
     root = core.parse(source)
 
     target_template = core.Wildcard("target", ast.Name(id=str))
@@ -2581,29 +2590,104 @@
         ast.Assign(targets=[target_template], value=ast.DictComp),
         ast.Expr(
             value=ast.Call(
                 func=ast.Attribute(value=target_template),
                 args=[core.Wildcard("other", object, common=False)],
     )),]
 
-    for first, *matches in core.walk_sequence(root, *template, expand_last=True):
+    for transaction, (first, *matches) in enumerate(core.walk_sequence(root, *template, expand_last=True)):
         replacement = ast.Assign(
             targets=[first.target],
             value=ast.Dict(
                 keys=[None] * (1 + len(matches)),
                 values=[first.root.value] + [m.other for m in matches],
             ),
             lineno=first.target.lineno,
         )
-        yield first.root, replacement
+        yield first.root, replacement, transaction
         for m in matches:
-            yield m.root, None
+            yield m.root, None, transaction
+
 
+def _is_recursive_binop_chain(node: ast.AST, op: ast.AST) -> bool:
+    if isinstance(node, ast.BinOp):
+        return isinstance(node.op, op) and _is_recursive_binop_chain(node.right, op)
 
-@processing.fix(restart_on_replace=True)
+    return True
+
+
+@processing.fix
+def replace_setcomp_add_with_union(source: str) -> str:
+    find = """
+    {{variable}} = {{something}}
+    for {{target}} in {{iterable}}:
+        {{variable}}.add({{something_else}})
+    """
+    replace = """
+    {{variable}} = {{something}} | {{{something_else}} for {{target}} in {{iterable}}}
+    """
+    find = core.compile_template(find, something=(ast.SetComp, ast.Set, ast.BinOp(op=ast.BitOr)))
+    for before, after, template_match in processing.find_replace(source, find, replace, yield_match=True):
+        if isinstance(template_match.root, ast.BinOp):
+            if _is_recursive_binop_chain(template_match.root, ast.BitOr):
+                yield before, after
+        else:
+            yield before, after
+
+    find = """
+    {{variable}} = {{something}}
+    {{variable}}.update({{something_else}})
+    """
+    replace = """
+    {{variable}} = {{something}} | set({{something_else}})
+    """
+    find = core.compile_template(find, something=(ast.SetComp, ast.Set, ast.BinOp(op=ast.BitOr)))
+    for before, after, template_match in processing.find_replace(source, find, replace, yield_match=True):
+        if isinstance(template_match.root, ast.BinOp):
+            if _is_recursive_binop_chain(template_match.root, ast.BitOr):
+                yield before, after
+        else:
+            yield before, after
+
+
+@processing.fix
+def replace_listcomp_append_with_plus(source: str) -> str:
+    find = """
+    {{variable}} = {{something}}
+    for {{target}} in {{iterable}}:
+        {{variable}}.append({{something_else}})
+    """
+    replace = """
+    {{variable}} = {{something}} + [{{something_else}} for {{target}} in {{iterable}}]
+    """
+    find = core.compile_template(find, something=(ast.ListComp, ast.List, ast.BinOp(op=ast.Add)))
+    for before, after, template_match in processing.find_replace(source, find, replace, yield_match=True):
+        if isinstance(template_match.root, ast.BinOp):
+            if _is_recursive_binop_chain(template_match.root, ast.Add):
+                yield before, after
+        else:
+            yield before, after
+
+    find = """
+    {{variable}} = {{something}}
+    {{variable}}.extend({{something_else}})
+    """
+    replace = """
+    {{variable}} = {{something}} + list({{something_else}})
+    """
+    find = core.compile_template(find, something=(ast.ListComp, ast.List, ast.BinOp(op=ast.Add)))
+    for before, after, template_match in processing.find_replace(source, find, replace, yield_match=True):
+        if isinstance(template_match.root, ast.BinOp):
+            if _is_recursive_binop_chain(template_match.root, ast.Add):
+                yield before, after
+        else:
+            yield before, after
+
+
+@processing.fix
 def simplify_dict_unpacks(source: str) -> str:
     root = core.parse(source)
 
     for node in core.walk(root, ast.Dict):
         if not any((k is None and isinstance(v, ast.Dict) for k, v in zip(node.keys, node.values))):
             continue
 
@@ -2615,15 +2699,15 @@
                 values.extend(v.values)
             else:
                 keys.append(k)
                 values.append(v)
         yield (node, ast.Dict(keys=keys, values=values))
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def simplify_collection_unpacks(source: str) -> str:
     root = core.parse(source)
 
     for node in core.walk(root, (ast.List, ast.Set, ast.Tuple)):
         replacements = False
         if not any((
             core.match_template(
@@ -2711,15 +2795,15 @@
     )
     modify_template = ast.Expr(
         value=ast.Call(
             func=ast.Attribute(value=target_template, attr=("add", "update", "append", "extend")),
             keywords=[],
     ))
     template = [assign_template, modify_template]
-    for node, *matches in core.walk_sequence(root, *template, expand_last=True):
+    for transaction, (node, *matches) in enumerate(core.walk_sequence(root, *template, expand_last=True)):
         assigned_value = node.root.value
         other_elts = []
         for m in matches:
             if m[0].value.func.attr in {"append", "add"}:
                 other_elts.append(m[0].value.args[0])
             elif m[0].value.func.attr in {"extend", "update"}:
                 for arg in m[0].value.args:
@@ -2733,32 +2817,32 @@
             elts = assigned_value.elts + other_elts
 
             if isinstance(assigned_value, ast.List):
                 replacement = ast.List(elts=elts)
             else:
                 replacement = ast.Set(elts=elts)
 
-            yield assigned_value, replacement
+            yield assigned_value, replacement, transaction
             for m in matches:
-                yield m.root, None
+                yield m.root, None, transaction
 
         elif isinstance(assigned_value, (ast.ListComp, ast.SetComp)):
             elts = [ast.Starred(value=assigned_value)] + other_elts
 
             if isinstance(assigned_value, ast.ListComp):
                 replacement = ast.List(elts=elts)
             else:
                 replacement = ast.Set(elts=elts)
 
-            yield assigned_value, replacement
+            yield assigned_value, replacement, transaction
             for m in matches:
-                yield m.root, None
+                yield m.root, None, transaction
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def breakout_starred_args(source: str) -> str:
     root = core.parse(source)
 
     # One element is unique, more than 1 may not be.
     # So, a 1-length set can safely be unpacked, but not a 2-length set.
     starred_arg_template = ast.Starred(value=(ast.List, ast.Tuple, ast.Set(elts=[object])))
     for node in core.walk(root, ast.Call):
@@ -2878,15 +2962,15 @@
     template = (
         ast.SetComp(generators=[comprehension_template]),
         ast.ListComp(generators=[comprehension_template]),
         ast.GeneratorExp(generators=[comprehension_template]),
         ast.DictComp(generators=[comprehension_template]),
     )
 
-    for node, target, value in core.walk_wildcard(root, template):
+    for transaction, (node, target, value) in enumerate(core.walk_wildcard(root, template)):
         subscript_template = core.compile_template(
             "{{value}}[{{target}}]", value=value, target=target
         )
         value_target_subscripts = list(
             core.walk(
                 node,
                 subscript_template,
@@ -2897,19 +2981,20 @@
             continue
 
         node_target_name = f"{core.unparse(value)}_{core.unparse(target)}"
         node_target_name = re.sub("[^a-zA-Z]", "_", node_target_name)
         yield (
             node.generators[0].iter,
             ast.Call(func=ast.Attribute(value=value, attr="items"), args=[], keywords=[]),
+            transaction,
         )
 
-        yield target, ast.Tuple(elts=[target, ast.Name(id=node_target_name)])
+        yield target, ast.Tuple(elts=[target, ast.Name(id=node_target_name)]), transaction
         for subscript_use in value_target_subscripts:
-            yield subscript_use, ast.Name(id=node_target_name)
+            yield subscript_use, ast.Name(id=node_target_name), transaction
 
 
 @processing.fix
 def _items_to_keys(source: str) -> Iterable[Tuple[ast.AST, ast.AST]]:
     root = core.parse(source)
     template = ast.comprehension(
         target=ast.Tuple(elts=[core.Wildcard("target", object), ast.Name(id="_")]),
@@ -2917,19 +3002,19 @@
             func=ast.Attribute(value=core.Wildcard("value", object), attr="items"),
             args=[],
             keywords=[],
         ),
         ifs=core.Wildcard("ifs", list),
         is_async=core.Wildcard("is_async", int),
     )
-    for node, _, _, target, value in core.walk_wildcard(root, template):
-        yield node.target, target
+    for transaction, (node, _, _, target, value) in enumerate(core.walk_wildcard(root, template)):
+        yield node.target, target, transaction
         yield node.iter, ast.Call(
             func=ast.Attribute(value=value, attr="keys"), args=[], keywords=[]
-        )
+        ), transaction
 
 
 @processing.fix
 def _items_to_values(source: str) -> Iterable[Tuple[ast.AST, ast.AST]]:
     root = core.parse(source)
     template = ast.comprehension(
         target=ast.Tuple(elts=[ast.Name(id="_"), core.Wildcard("target", object)]),
@@ -2937,32 +3022,32 @@
             func=ast.Attribute(value=core.Wildcard("value", object), attr="items"),
             args=[],
             keywords=[],
         ),
         ifs=core.Wildcard("ifs", list),
         is_async=core.Wildcard("is_async", int),
     )
-    for node, _, _, target, value in core.walk_wildcard(root, template):
-        yield node.target, target
+    for transaction, (node, _, _, target, value) in enumerate(core.walk_wildcard(root, template)):
+        yield node.target, target, transaction
         yield node.iter, ast.Call(
             func=ast.Attribute(value=value, attr="values"), args=[], keywords=[]
-        )
+        ), transaction
 
 
 @processing.fix
 def _for_keys_to_items(source: str) -> Iterable[Tuple[ast.AST, ast.AST]]:
     root = core.parse(source)
     template = ast.For(
         target=core.Wildcard("target", object),
         iter=ast.Call(
             func=ast.Attribute(value=core.Wildcard("value", object), attr="keys"),
             args=[],
             keywords=[],
     ),)
-    for node, target, value in core.walk_wildcard(root, template):
+    for transaction, (node, target, value) in enumerate(core.walk_wildcard(root, template)):
         subscript_template = core.compile_template(
             "{{value}}[{{target}}]", value=value, target=target
         )
         value_target_subscripts = list(
             core.walk(
                 node,
                 subscript_template,
@@ -2973,55 +3058,56 @@
             continue
 
         node_target_name = f"{core.unparse(value)}_{core.unparse(target)}"
         node_target_name = re.sub("[^a-zA-Z]", "_", node_target_name)
         yield (
             node.iter,
             ast.Call(func=ast.Attribute(value=value, attr="items"), args=[], keywords=[]),
+            transaction,
         )
 
-        yield target, ast.Tuple(elts=[target, ast.Name(id=node_target_name)])
+        yield target, ast.Tuple(elts=[target, ast.Name(id=node_target_name)]), transaction
         for subscript_use in value_target_subscripts:
-            yield subscript_use, ast.Name(id=node_target_name)
+            yield subscript_use, ast.Name(id=node_target_name), transaction
 
 
 @processing.fix
 def _for_items_to_keys(source: str) -> Iterable[Tuple[ast.AST, ast.AST]]:
     root = core.parse(source)
     template = ast.For(
         target=ast.Tuple(elts=[core.Wildcard("target", object), ast.Name(id="_")]),
         iter=ast.Call(
             func=ast.Attribute(value=core.Wildcard("value", object), attr="items"),
             args=[],
             keywords=[],
     ),)
 
-    for node, target, value in core.walk_wildcard(root, template):
-        yield node.target, target
+    for transaction, (node, target, value) in enumerate(core.walk_wildcard(root, template)):
+        yield node.target, target, transaction
         yield node.iter, ast.Call(
             func=ast.Attribute(value=value, attr="keys"), args=[], keywords=[]
-        )
+        ), transaction
 
 
 @processing.fix
 def _for_items_to_values(source: str) -> Iterable[Tuple[ast.AST, ast.AST]]:
     root = core.parse(source)
     template = ast.For(
         target=ast.Tuple(elts=[ast.Name(id="_"), core.Wildcard("target", object)]),
         iter=ast.Call(
             func=ast.Attribute(value=core.Wildcard("value", object), attr="items"),
             args=[],
             keywords=[],
     ),)
 
-    for node, target, value in core.walk_wildcard(root, template):
-        yield node.target, target
+    for transaction, (node, target, value) in enumerate(core.walk_wildcard(root, template)):
+        yield node.target, target, transaction
         yield node.iter, ast.Call(
             func=ast.Attribute(value=value, attr="values"), args=[], keywords=[]
-        )
+        ), transaction
 
 
 def implicit_dict_keys_values_items(source: str) -> str:
     source = _keys_to_items(source)
     source = _items_to_keys(source)
     source = _items_to_values(source)
     source = _for_keys_to_items(source)
@@ -3039,17 +3125,17 @@
     target_template = ast.Tuple(elts=[ast.Name(id="_"), core.Wildcard("target", object)])
 
     template = (
         ast.comprehension(iter=iter_template, target=target_template),
         ast.For(iter=iter_template, target=target_template),
     )
 
-    for node, node_iter, target in core.walk_wildcard(root, template):
-        yield node.iter, node_iter
-        yield node.target, target
+    for transaction, (node, node_iter, target) in enumerate(core.walk_wildcard(root, template)):
+        yield node.iter, node_iter, transaction
+        yield node.target, target, transaction
 
 
 @processing.fix
 def unused_zip_args(source: str) -> str:
     root = core.parse(source)
     iter_template = ast.Call(
         func=core.Wildcard(
@@ -3066,15 +3152,15 @@
 
     template = (
         ast.comprehension(iter=iter_template, target=target_template),
         ast.For(iter=iter_template, target=target_template),
     )
 
     safe_callables = parsing.safe_callable_names(root)
-    for node, elts, func, node_iter in core.walk_wildcard(root, template):
+    for transaction, (node, elts, func, node_iter) in enumerate(core.walk_wildcard(root, template)):
         new_elts = []
         iters = []
         changes = False
 
         # Starred messed with the order of things in slightly complicated ways
         # TODO handle starred args
         if any(isinstance(arg, ast.Starred) for arg in elts):
@@ -3091,22 +3177,22 @@
                 new_elts.append(elt)
                 iters.append(arg)
 
         if not changes:
             continue
 
         if len(new_elts) == 0:  # 0 args used => replace zip with first arg
-            yield node.target, elts[0]
-            yield node.iter, node_iter[0]
+            yield node.target, elts[0], transaction
+            yield node.iter, node_iter[0], transaction
         elif len(new_elts) == 1:  # 1 arg used => replace zip with that arg
-            yield node.target, new_elts[0]
-            yield node.iter, iters[0]
+            yield node.target, new_elts[0], transaction
+            yield node.iter, iters[0], transaction
         elif len(new_elts) > 1:  # > 1 args used => remove unused ones, keep zip
-            yield node.target, ast.Tuple(elts=new_elts)
-            yield node.iter, ast.Call(func=func, args=iters, keywords=[])
+            yield node.target, ast.Tuple(elts=new_elts), transaction
+            yield node.iter, ast.Call(func=func, args=iters, keywords=[]), transaction
 
 
 @processing.fix
 def simplify_assign_immediate_return(source: str) -> str:
     find = """
     {{name}} = {{value}}
     return {{name}}
@@ -3522,59 +3608,59 @@
     find = """
     if {{condition}}:
         return True
     return False
     """
     replace = "return {{condition}}"
 
-    yield from processing.find_replace(source, find, replace)
+    yield from processing.find_replace(source, find, replace, transaction=0)
 
     find = """
     if {{condition}}:
         return False
     return True
     """
     replace = "return not ({{condition}})"
 
-    yield from processing.find_replace(source, find, replace, condition=ast.BoolOp)
+    yield from processing.find_replace(source, find, replace, condition=ast.BoolOp, transaction=1)
 
     find = """
     if {{condition}}:
         return False
     return True
     """
     replace = "return not {{condition}}"
 
-    yield from processing.find_replace(source, find, replace)
+    yield from processing.find_replace(source, find, replace, transaction=2)
 
 
 @processing.fix
 def fix_if_assign(source: str) -> str:
     find = """
     if {{condition}}:
         {{variable}} = True
     else:
         {{variable}} = False
     """
     replace = "{{variable}} = {{condition}}"
 
-    yield from processing.find_replace(source, find, replace)
+    yield from processing.find_replace(source, find, replace, transaction=0)
 
     find = """
     if {{condition}}:
         {{variable}} = False
     else:
         {{variable}} = True
     """
     replace = "{{variable}} = not ({{condition}})"
 
-    yield from processing.find_replace(source, find, replace, condition=ast.BoolOp)
+    yield from processing.find_replace(source, find, replace, condition=ast.BoolOp, transaction=1)
 
     find = """
     if {{condition}}:
         {{variable}} = False
     else:
         {{variable}} = True
     """
     replace = "{{variable}} = not {{condition}}"
 
-    yield from processing.find_replace(source, find, replace)
+    yield from processing.find_replace(source, find, replace, transaction=2)
```

### Comparing `pyrefact-90/pyrefact/formatting.py` & `pyrefact-91/pyrefact/formatting.py`

 * *Files identical despite different names*

### Comparing `pyrefact-90/pyrefact/logs.py` & `pyrefact-91/pyrefact/logs.py`

 * *Files identical despite different names*

### Comparing `pyrefact-90/pyrefact/main.py` & `pyrefact-91/pyrefact/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 import os
 import re
 import sys
 import textwrap
 from pathlib import Path
 from typing import Collection, Iterable, Sequence
 
+import rmspace
+
 from pyrefact import abstractions, fixes
 from pyrefact import logs as logger
 from pyrefact import (
     core,
     formatting,
     object_oriented,
     parsing,
     performance,
     performance_numpy,
     performance_pandas,
+    processing,
     symbolic_math,
     tracing,
 )
 
 MAX_MODULE_PASSES = 5
 MAX_FILE_PASSES = 25
 
@@ -52,19 +55,21 @@
 
     Args:
         source (str): Python source code
 
     Returns:
         str: Modified code
     """
-    source = fixes.deinterpolate_logging_args(source)
-    source = fixes.invalid_escape_sequence(source)
-    source = tracing.fix_starred_imports(source)
-    source = tracing.fix_reimported_names(source)
-    return source
+    chain = processing.chain((
+        fixes.deinterpolate_logging_args,
+        fixes.invalid_escape_sequence,
+        tracing.fix_starred_imports,
+        tracing.fix_reimported_names,
+    ))
+    return chain(source)
 
 
 def _multi_run_fixes(source: str, preserve: Collection[str]) -> str:
     """Fixes that should run over and over until convergence.
 
     Args:
         source (str): Python source code
@@ -107,14 +112,16 @@
     source = fixes.simplify_collection_unpacks(source)
     source = fixes.remove_duplicate_set_elts(source)
     source = fixes.breakout_starred_args(source)
     source = performance_pandas.replace_loc_at_iloc_iat(source)
     source = performance_pandas.replace_iterrows_index(source)
     source = performance_pandas.replace_iterrows_itertuples(source)
     source = fixes.replace_for_loops_with_set_list_comp(source)
+    source = fixes.replace_setcomp_add_with_union(source)
+    source = fixes.replace_listcomp_append_with_plus(source)
     source = fixes.replace_for_loops_with_dict_comp(source)
     source = fixes.implicit_dict_keys_values_items(source)
     source = fixes.replace_dict_assign_with_dict_literal(source)
     source = fixes.replace_dict_update_with_dict_literal(source)
     source = fixes.replace_dictcomp_assign_with_dict_literal(source)
     source = fixes.replace_dictcomp_update_with_dict_literal(source)
     source = fixes.simplify_dict_unpacks(source)
@@ -153,16 +160,16 @@
     preserve: Collection[str] = frozenset(),
     safe: bool = False,
     keep_imports: bool = False,
 ) -> str:
     if re.findall(r"# pyrefact: skip_file", source):
         return source
 
-    source = fixes.fix_tabs(source)
-    source = fixes.fix_rmspace(source)
+    source = source.expandtabs(4)
+    source = rmspace.format_str(source)
     source = fixes.fix_too_many_blank_lines(source)
 
     if not source.strip():
         return source
 
     if core.is_valid_python(source):
         minimum_indent = 0
@@ -227,15 +234,15 @@
         source = fixes.add_missing_imports(source)
         if not keep_imports:
             source = fixes.remove_unused_imports(source)
 
     source = fixes.sort_imports(source)
 
     source = fixes.fix_line_lengths(source)
-    source = fixes.fix_rmspace(source)
+    source = rmspace.format_str(source)
 
     if minimum_indent > 0:
         source = textwrap.indent(source, " " * minimum_indent)
 
     return source
```

### Comparing `pyrefact-90/pyrefact/object_oriented.py` & `pyrefact-91/pyrefact/object_oriented.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
 def _decorators_of_type(node: ast.FunctionDef, name: str) -> Iterable[ast.AST]:
     for decorator in node.decorator_list:
         if isinstance(decorator, ast.Name) and decorator.id == name:
             yield decorator
 
 
+@processing.fix
 def move_staticmethod_static_scope(source: str, preserve: Collection[str]) -> str:
     root = core.parse(source)
 
     attributes_to_preserve = set()
     for name in preserve:
         if "." in name:
             *_, property_name = name.split(".")
@@ -169,45 +170,42 @@
 
             if core.match_template(node, template):
                 replacements[node] = ast.Name(
                     id=moved_function_names[node.attr], ctx=node.ctx, lineno=node.lineno
                 )
 
     if not name_replacements:
-        return source
+        return
 
     if len(name_replacements) != len(set(name_replacements.values())):
-        return source
+        return
 
-    if replacements:
-        source = processing.replace_nodes(source, replacements)
-        root = core.parse(source)
-
-    for classdef in sorted(parsing.iter_classdefs(root), key=lambda cd: cd.lineno, reverse=True):
-        delete = []
-        additions = []
+    transaction = 0
+    for before, after in replacements.items():
+        yield before, after, transaction
 
+    transaction = 1
+    for classdef in parsing.iter_classdefs(root):
         for funcdef in parsing.iter_funcdefs(classdef):
             new_name = name_replacements.get((classdef.name, funcdef.name))
             if new_name is None:
                 continue
+
             staticmethod_decorators = set(_decorators_of_type(funcdef, "staticmethod"))
             static_names.add(new_name)
-            delete.append(funcdef)
-            additions.append(
-                ast.FunctionDef(
-                    name=new_name,
-                    args=funcdef.args,
-                    body=funcdef.body,
-                    decorator_list=[
-                        dec for dec in funcdef.decorator_list if dec not in staticmethod_decorators
-                    ],
-                    type_params=[],
-                    returns=funcdef.returns,
-                    lineno=classdef.lineno - 1,
-            ))
-
-        if delete or additions:
-            source = processing.remove_nodes(source, delete, root)
-            source = processing.insert_nodes(source, reversed(additions))
 
-    return source
+            funcdef_static = ast.FunctionDef(
+                name=new_name,
+                args=funcdef.args,
+                body=funcdef.body,
+                decorator_list=[
+                    dec for dec in funcdef.decorator_list if dec not in staticmethod_decorators
+                ],
+                type_params=[],
+                returns=funcdef.returns,
+                lineno=classdef.lineno - 1,
+                col_offset=classdef.col_offset,
+            )
+            yield funcdef, None, transaction
+            yield None, funcdef_static, transaction
+
+            transaction += 1
```

### Comparing `pyrefact-90/pyrefact/parsing.py` & `pyrefact-91/pyrefact/parsing.py`

 * *Files identical despite different names*

### Comparing `pyrefact-90/pyrefact/performance.py` & `pyrefact-91/pyrefact/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     iter_template = ast.Call(func=ast.Name(id=("iter", "list", "tuple")), args=[object])
     template = (ast.For(iter=iter_template), ast.comprehension(iter=iter_template))
 
     for node in core.walk(root, template):
         yield node.iter, node.iter.args[0]
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def remove_redundant_chained_calls(source: str) -> str:
     root = core.parse(source)
 
     # If outer is present, inner is redundant
     outer_inner_redundancy_mapping = {
         "sorted": {"list", "sorted", "tuple", "iter", "reversed"},
         "list": {"list", "tuple", "iter"},
@@ -194,15 +194,15 @@
             yield node, replacement
 
 
 def _wrap_transpose(node: ast.AST) -> ast.Call:
     return ast.Call(func=ast.Name(id="zip"), args=[ast.Starred(value=node)], keywords=[])
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def _replace_subscript_looping_simple_cases(source: str) -> str:
     yield from processing.find_replace(
         source,
         "[{{sequence}}[{{index}}] for {{index}} in range(len({{sequence}}))]",
         "list({{sequence}})",
     )
     yield from processing.find_replace(
@@ -303,12 +303,11 @@
         else:
             yield comprehension.iter, _wrap_transpose(template_match.target)
 
         for node in target_indexed_nodes:
             yield node, ast.Name(id=new_index_name)
 
 
+@processing.fix
 def replace_subscript_looping(source: str) -> str:
-    source = _replace_subscript_looping_simple_cases(source)
-    source = _replace_subscript_looping_complex_cases(source)
-
-    return source
+    yield from _replace_subscript_looping_simple_cases._fix_func(source)
+    yield from _replace_subscript_looping_complex_cases._fix_func(source)
```

### Comparing `pyrefact-90/pyrefact/performance_numpy.py` & `pyrefact-91/pyrefact/performance_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 from __future__ import annotations
 
 import ast
-from typing import Callable
 
 from pyrefact import core, parsing, processing
 
 
 def _uses_numpy(root: ast.Module) -> bool:
     if "numpy" in parsing.module_dependencies(root):
         return True
 
     # If np.something is referenced anywhere, assume it uses numpy as well.
     template = core.compile_template(("np.{{something}}", "numpy.{{something}}"))
     return any(core.walk(root, template))
 
 
-def _only_if_uses_numpy(f: Callable) -> Callable:
-    def wrapper(source: str) -> str:
-        root = core.parse(source)
-        if not _uses_numpy(root):
-            return source
-
-        return f(source)
-
-    return wrapper
-
-
 def _is_sum_call(call: ast.Call):
     return parsing.is_call(call, ("sum", "np.sum", "numpy.sum"))
 
 
 def _is_zip_product(comp: ast.ListComp | ast.GeneratorExp):
     template = core.compile_template((
         "[{{left}} * {{right}} for {{left}}, {{right}} in zip({{left_iterable}}, {{right_iterable}})]",
@@ -73,27 +61,28 @@
             left, right = target.args
             matmul = _wrap_np_matmul(_wrap_transpose(right), _wrap_transpose(left))
             matmul.func = target.func
             matmul.keywords = target.keywords
             yield node, matmul
 
 
-@_only_if_uses_numpy
 @processing.fix
 def replace_implicit_dot(source: str) -> str:
     root = core.parse(source)
+    if not _uses_numpy(root):
+        return
 
     template = ast.Call(args=[(ast.ListComp, ast.GeneratorExp)], keywords=[])
     for call in core.walk(root, template):
         if _is_sum_call(call) and _is_zip_product(call.args[0]):
             zip_args = call.args[0].generators[0].iter.args
             yield call, _wrap_np_dot(*zip_args)
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def replace_implicit_matmul(source: str) -> str:
     find = """
     for {{i}} in range(len({{left}})):
         for {{j}} in range(len({{right}}[0])):
             for {{k}} in range(len({{right}})):
                 {{result}}[{{i}}][{{j}}] += {{left}}[{{i}}][{{k}}] * {{right}}[{{k}}][{{j}}]
     """
```

### Comparing `pyrefact-90/pyrefact/performance_pandas.py` & `pyrefact-91/pyrefact/performance_pandas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import ast
 
 from pyrefact import core, processing
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def replace_loc_at_iloc_iat(source: str) -> str:
     yield from processing.find_replace(
         source,
         "{{value}}.loc[{{i}}]",
         "{{value}}.at[{{i}}]",
         i=ast.Constant,
+        transaction=0
     )
     yield from processing.find_replace(
         source,
         "{{value}}.loc[{{i}}, {{j}}]",
         "{{value}}.at[{{i}}, {{j}}]",
         i=ast.Constant,
         j=ast.Constant,
+        transaction=1
     )
     yield from processing.find_replace(
         source,
         "{{value}}.iloc[{{i}}]",
         "{{value}}.iat[{{i}}]",
         i=ast.Constant,
+        transaction=2
     )
     yield from processing.find_replace(
         source,
         "{{value}}.iloc[{{i}}, {{j}}]",
         "{{value}}.iat[{{i}}, {{j}}]",
         i=ast.Constant,
         j=ast.Constant,
+        transaction=3
     )
 
 
 @processing.fix
 def replace_iterrows_index(source: str) -> str:
     root = core.parse(source)
 
@@ -50,14 +54,15 @@
     )
 
     for node, new_target, underlying_object in core.walk_wildcard(root, template):
         yield node.target, new_target
         yield node.iter, ast.Attribute(value=underlying_object, attr="index")
 
 
+@processing.fix
 def replace_iterrows_itertuples(source: str) -> str:
     root = core.parse(source)
     replacements = {}
     target_template = ast.Tuple(
         elts=[ast.Name(id="_"), ast.Name(id=core.Wildcard("new_target_id", str))]
     )
     iter_template = ast.Call(
@@ -152,8 +157,9 @@
         )
         node_replacements[node.iter] = new_iter
         node_replacements[node.target] = new_target
 
         replacements.update(node_replacements)
     template = ast.comprehension(target=target_template, iter=iter_template)
 
-    return processing.alter_code(source, root, replacements=replacements)
+    for node, replacement in replacements.items():
+        yield node, replacement, 0
```

### Comparing `pyrefact-90/pyrefact/processing.py` & `pyrefact-91/pyrefact/processing.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 import collections
 import difflib
 import functools
 import heapq
 import re
 import textwrap
 from types import MappingProxyType
-from typing import Callable, Collection, Iterable, Literal, Mapping, NamedTuple, Sequence, Tuple
+from typing import (
+    Any,
+    Callable,
+    Collection,
+    Iterable,
+    Literal,
+    Mapping,
+    NamedTuple,
+    Sequence,
+    Tuple,
+)
 
 from pyrefact import core, formatting, logs as logger
 
 MSG_INFO_REPLACE = """{fix_function_name:<40}: Replacing code:
 {old_code}
 * -> *****************
 {new_code}
@@ -27,32 +37,57 @@
 **********************"""
 MSG_ERROR_REMOVE = """{fix_function_name:<40}: Failed to remove code:
 {old_code}
 **********************"""
 
 
 def _log_replacement(old: str, new: str | None, fix_function_name: str, valid: bool) -> None:
-    if new and valid:
+    if new.strip() and valid:
         logger.debug(
             MSG_INFO_REPLACE, fix_function_name=fix_function_name, old_code=old, new_code=new
         )
-    elif new and not valid:
+    elif new.strip() and not valid:
         logger.error(
             MSG_ERROR_REPLACE, fix_function_name=fix_function_name, old_code=old, new_code=new
         )
     elif not new and valid:
         logger.debug(MSG_INFO_REMOVE, fix_function_name=fix_function_name, old_code=old)
     elif not new and not valid:
         logger.error(MSG_ERROR_REMOVE, fix_function_name=fix_function_name, old_code=old)
 
 
 class _Rewrite(NamedTuple):
     old: ast.AST | core.Range  # TODO replace with (start_char, end_char)
     new: ast.AST | str  # "" indicates a removal
 
+    def __hash__(self) -> int:
+        if isinstance(self.old, ast.AST):
+            old_hash = hash((
+                getattr(self.old, "lineno", None),
+                getattr(self.old, "col_offset", None),
+                getattr(self.old, "end_lineno", None),
+                getattr(self.old, "end_col_offset", None),
+                core.unparse(self.old),
+            ))
+        else:
+            old_hash = hash(self.old)
+
+        if isinstance(self.new, ast.AST):
+            new_hash = hash((
+                getattr(self.new, "lineno", None),
+                getattr(self.new, "col_offset", None),
+                getattr(self.new, "end_lineno", None),
+                getattr(self.new, "end_col_offset", None),
+                core.unparse(self.new),
+            ))
+        else:
+            new_hash = hash(self.new)
+
+        return hash((old_hash, new_hash))
+
 
 def _substitute_original_strings(original_source: str, new_source: str) -> str:
     """Ensure consistent string formattings in new and old source.
 
     The reason for this to exist is that, without it, pyrefact will change the string
     formattings of values in a very opinionated, and frankly not very nice way. For
     example, multiline f-strings would be replaced by really long regular strings with
@@ -98,15 +133,15 @@
             and new_formatting not in original_formattings
         ):
             most_common_original_formatting = collections.Counter(original_formattings).most_common(
                 1
             )[0][0]
             replacements[node] = most_common_original_formatting
 
-    return replace_nodes(new_source, replacements)
+    return _replace_nodes(new_source, replacements)
 
 
 def _substitute_original_fstrings(original_source: str, new_source: str) -> str:
     """Ensure consistent string formattings in new and old source.
 
     The reason for this to exist is that, without it, pyrefact will change the string
     formattings of values in a very opinionated, and frankly not very nice way. For
@@ -142,15 +177,15 @@
             and new_formatting not in original_formattings
         ):
             most_common_original_formatting = collections.Counter(original_formattings).most_common(
                 1
             )[0][0]
             replacements[node] = most_common_original_formatting
 
-    return replace_nodes(new_source, replacements)
+    return _replace_nodes(new_source, replacements)
 
 
 def remove_nodes(source: str, nodes: Iterable[ast.AST], root: ast.Module) -> str:
     """Remove ast nodes from code
 
     Args:
         source (str): Python source code
@@ -288,19 +323,32 @@
         else:
             pass_candidate = source[: old.start] + "pass" + source[old.end :]
             if core.is_valid_python(pass_candidate):
                 choice = pass_candidate
             else:
                 choice = candidate
 
+        if not core.is_valid_python(choice):
+            new_code_lines = new_code.splitlines(keepends=True)
+            for extra_indent in range(0, 16, 4):
+                candidate = (
+                    source[: old.start]
+                    + new_code_lines[0]
+                    + "".join(" " * extra_indent + l for l in new_code_lines[1:])
+                    + source[old.end :]
+                )
+                if core.is_valid_python(candidate):
+                    choice = candidate
+                    break
+
         new_source, old, new = _minimize_whitespace_line_differences(source, choice)
         valid = core.is_valid_python(new_source)
         _log_replacement(old, new, fix_function_name, valid)
 
-        if not core.is_valid_python(new_source):
+        if not valid:
             return source
 
         return new_source
 
     lines = new_code.splitlines(keepends=True)
     indent = getattr(old, "col_offset", getattr(new, "col_offset", 0))
     indents = {**{i: indent for i in range(len(lines))}, 0: len(code) - len(code.lstrip(" "))}
@@ -336,21 +384,21 @@
         if core.is_valid_python(pass_candidate):
             candidate = pass_candidate
 
     new_source, old, new = _minimize_whitespace_line_differences(source, candidate)
     valid = core.is_valid_python(new_source)
     _log_replacement(old, new, fix_function_name, valid)
 
-    if not core.is_valid_python(new_source):
+    if not valid:
         return source
 
     return new_source
 
 
-def replace_nodes(source: str, replacements: Mapping[ast.AST, ast.AST | str]) -> str:
+def _replace_nodes(source: str, replacements: Mapping[ast.AST, ast.AST | str]) -> str:
     rewrites = sorted(
         replacements.items(),
         key=lambda tup: (
             tup[0].lineno,
             tup[0].end_lineno,
             getattr(tup[0], "col_offset", 0),
             getattr(tup[0], "end_col_offset", 0),
@@ -360,15 +408,15 @@
     for old, new in rewrites:
         rewrite = _Rewrite(old, new)
         source = _do_rewrite(source, rewrite)
 
     return source
 
 
-def insert_nodes(source: str, additions: Collection[ast.AST]) -> str:
+def _insert_nodes(source: str, additions: Collection[ast.AST]) -> str:
     """Insert ast nodes in python source code.
 
     Args:
         source (str): Python source code before insertions.
         additions (Collection[ast.AST]): Ast nodes to add. Linenos must be accurate.
 
     Returns:
@@ -383,15 +431,14 @@
         lines = (
             lines[: node.lineno]
             + ["\n"]
             + [" " * col_offset + line for line in addition.splitlines(keepends=True)]
             + ["\n"] * (not addition.endswith("\n"))
             + lines[node.lineno :]
         )
-
     return "".join(lines)
 
 
 def alter_code(
     source: str,
     root: ast.AST,
     *,
@@ -459,19 +506,19 @@
             (x, y),
             )
             for x, y in replacements.items()
     ),]
     # a < d => deletions will go before additions if same lineno and reversed sorting.
     for *_, action, _, value in sorted(actions, reverse=True):
         if action == "add":
-            source = insert_nodes(source, [value])
+            source = _insert_nodes(source, [value])
         elif action == "delete":
             source = remove_nodes(source, [value], root)
         elif action == "replace":
-            source = replace_nodes(source, {value[0]: value[1]})
+            source = _replace_nodes(source, {value[0]: value[1]})
         else:
             raise ValueError(f"Invalid action: {action}")
 
     source = _substitute_original_strings(original_source, source)
     source = _substitute_original_fstrings(original_source, source)
 
     return source
@@ -484,87 +531,191 @@
 
     if old is not None:
         return core.get_charnos(old, source)
 
     return core.get_charnos(new, source)
 
 
-def fix(*maybe_func, restart_on_replace: bool = False, sort_order: bool = True) -> Callable:
+def _schedule_rewrites(
+    source: str, funcs: Iterable[Tuple[Callable, Sequence, Mapping]]
+) -> Sequence[Tuple[Any, Callable]]:
+    default_transaction = {"count": -100000000}
+
+    def fill_transaction(tup) -> Tuple[ast.AST, ast.AST, int]:
+        default_transaction["count"] += 1
+        if len(tup) == 3:
+            before, after, transaction = tup
+        elif len(tup) == 2:
+            before, after = tup
+            transaction = default_transaction["count"]
+        else:
+            raise ValueError(f"Invalid tuple: {tup!r}")
+
+        if isinstance(before, ast.AST):
+            before = core.get_charnos(before, source)
+        elif before is None:
+            before = core.get_charnos(after, source)
+
+        if after is None:
+            after = ""
+        return (before, after, transaction)
+
+    overlap_error_format = "Discarding transaction {transaction} due to overlapping rewrite ranges: {range} and {other}"
+    duplicate_error_format = "Discarding duplicate transaction {transaction}."
+    scheduled_rewrites = []
+    transaction_rewrites = collections.defaultdict(list)
+    for k, (func, args, kwargs) in enumerate(funcs):
+        for old, new, transaction in map(fill_transaction, func(*args, **kwargs)):
+            transaction_rewrites[k, transaction, func.__name__].append(_Rewrite(old, new or ""))
+
+        seen_transactions = set()
+        duplicate_transaction_keys = []
+        for key in sorted(transaction_rewrites):
+            transaction = tuple(transaction_rewrites[key])
+            if transaction in seen_transactions:
+                duplicate_transaction_keys.append(key)
+
+            seen_transactions.add(transaction)
+
+        for key in duplicate_transaction_keys:
+            logger.error(duplicate_error_format.format(transaction=key))
+            del transaction_rewrites[key]
+
+        for transaction in sorted(transaction_rewrites):
+            if transaction[0] != k:
+                continue
+
+            rewrites = transaction_rewrites[transaction]
+            rewrites = sorted(
+                ((_get_charnos(rewrite, source), rewrite) for rewrite in rewrites),
+                key=lambda tup: tup[0],
+                reverse=True,
+            )
+            conflicting = False
+            for i, (rewrite_range, rewrite) in enumerate(rewrites):
+                for _, (other, _) in rewrites[i + 1 :]:
+                    if rewrite_range & other:
+                        logger.debug(
+                            overlap_error_format.format(
+                                transaction=transaction,
+                                range=tuple(rewrite_range),
+                                other=tuple(other),
+                        ))
+                        conflicting = True
+                        break
+                for _, (other, _) in scheduled_rewrites:
+                    if rewrite_range & other:
+                        logger.debug(
+                            overlap_error_format.format(
+                                transaction=transaction,
+                                range=tuple(rewrite_range),
+                                other=tuple(other),
+                        ))
+                        conflicting = True
+                        break
+                if conflicting:
+                    break
+
+            if not conflicting:
+                scheduled_rewrites.extend(((transaction, r) for r in rewrites))
+    if transaction_rewrites and (not scheduled_rewrites):
+        logger.error("{} transactions found, but all were conflicting.", len(transaction_rewrites))
+
+    scheduled_rewrites.sort(key=lambda tup: (tup[1][0], tup[0]), reverse=True)
+    return scheduled_rewrites
+
+
+def _apply_rewrites(source: str, rewrites: Sequence[Tuple[Any, Callable]]) -> str:
+    for (*_, fix_func_name), (rewrite_range, rewrite) in rewrites:
+        source = _do_rewrite(source, rewrite, fix_function_name=fix_func_name)
+
+    return source
+
+
+def fix(*maybe_func, max_iter: int = 5) -> Callable:
     """Convert an iterator of (before, after) asts to a function that fixes source code.
 
     Args:
         maybe_func (Callable): Function to fix source code. If not provided, this is a decorator.
-        restart_on_replace (bool, optional): If True, restarts the rewrite loop on replacements.
-            This is needed when a replacement may alter the code in a way that makes it hard for
-            the rewriter to properly place the next rewrite. Defaults to False.
-        sort_order (bool, optional): If True, sorts the rewrites by line number and col_offset.
+        max_iter (int, optional): Maximum number of iterations to run the rewrite loop. Defaults to 5.
     """
 
     def fix_decorator(func: Callable) -> Callable:
         @functools.wraps(func)
         def wrapper(source, *args, **kwargs):
-            # Track rewrite history as an infinite loop guard
-            history = set()
-            for _ in range(1000):  # Max 1000 iterations
-                if restart_on_replace:
-                    try:
-                        old, new = next(
-                            r for r in func(source, *args, **kwargs) if r not in history
-                        )
-                        rewrite = _Rewrite(old, new or "")
-                        history.add(rewrite)
-                        source = _do_rewrite(source, rewrite, fix_function_name=func.__name__)
-                    except StopIteration:
-                        return source
-
-                    continue
-
-                rewrites = (_Rewrite(old, new or "") for old, new in func(source, *args, **kwargs))
-                if sort_order:
-                    rewrites = sorted(
-                        ((_get_charnos(rewrite, source), rewrite) for rewrite in rewrites),
-                        key=lambda tup: tup[0],
-                        reverse=True,
-                    )
-
-                rewritten_ranges = []
-                for rewrite_range, rewrite in rewrites:
-                    if any(rewrite_range & other for other in rewritten_ranges):
-                        logger.debug(
-                            "Found rewrite that overlaps with previous rewrite. Restarting @fix loop."
-                        )
-                        break
+            history = {source}
+            for _ in range(max_iter):
+                scheduled_rewrites = _schedule_rewrites(source, [[func, [source, *args], kwargs]])
+                source = _apply_rewrites(source, scheduled_rewrites)
 
-                    source = _do_rewrite(source, rewrite, fix_function_name=func.__name__)
-                    rewritten_ranges.append(rewrite_range)
-                else:
-                    return source
+                if source in history:
+                    break
 
             return source
 
+        wrapper._fix_func = func
         return wrapper
 
     if not maybe_func:
         return fix_decorator
 
     if len(maybe_func) == 1 and callable(maybe_func[0]):
         return fix_decorator(maybe_func[0])
 
     raise ValueError(f"Exactly 1 or 0 arguments must be given as maybe_func, not {len(maybe_func)}")
 
 
+def _build_chain(source, preserve, fix_funcs) -> Sequence[Tuple[Callable, Sequence, Mapping]]:
+    funcs = []
+    for func in fix_funcs:
+        if hasattr(func, "_fix_func"):
+            func = func._fix_func
+
+        args = [arg for arg in func.__code__.co_varnames if arg in {"source", "preserve"}]
+        if args == ["source"]:
+            funcs.append((func, [source], {}))
+        elif args == ["source", "preserve"]:
+            funcs.append((func, [source], {"preserve": preserve}))
+        else:
+            raise NotImplementedError(
+                f"Cannot chain fix function {func.__name__} with unrecognized args: {args}."
+            )
+
+    return funcs
+
+
+def chain(fix_funcs: Iterable[Callable], max_iter: int = 10) -> Callable:
+    fix_funcs = tuple(fix_funcs)
+
+    def func_chain(source, preserve=frozenset()):
+        history = {source}
+        preserve = frozenset(preserve)
+        for _ in range(max_iter):
+            # Chain must be rebuilt on each iteration, since the source argument will change.
+            funcs = _build_chain(source, preserve, fix_funcs)
+            scheduled_rewrites = _schedule_rewrites(source, funcs)
+            source = _apply_rewrites(source, scheduled_rewrites)
+            if source in history:
+                break
+
+        return source
+
+    return func_chain
+
+
 def find_replace(
     source: str,
     find: str | ast.AST,
     replace: str,
     *,
     root: ast.AST = None,
     expand_first: bool = None,
     expand_last: bool = None,
     yield_match: bool = False,
+    transaction: int = None,
     **callables_or_templates,
 ) -> Iterable[core.Range, str]:
     """Swap a find with a replacement.
 
     Args:
         source (str): Python source code.
         root (ast.AST): Parsed AST to search. If not provided, source is parsed.
@@ -625,11 +776,14 @@
         template_replacement = core.format_template(replace, combined_match, **callables)
 
         indentation = formatting.indentation_level(source[range_start:range_end])
 
         template_replacement = textwrap.dedent(template_replacement)
         template_replacement = textwrap.indent(template_replacement, " " * indentation)
 
+        item = [replacement_range, template_replacement]
+        if transaction is not None:
+            item.append(transaction)
         if yield_match:
-            yield replacement_range, template_replacement, combined_match
-        else:
-            yield replacement_range, template_replacement
+            item.append(combined_match)
+
+        yield tuple(item)
```

### Comparing `pyrefact-90/pyrefact/style.py` & `pyrefact-91/pyrefact/style.py`

 * *Files identical despite different names*

### Comparing `pyrefact-90/pyrefact/symbolic_math.py` & `pyrefact-91/pyrefact/symbolic_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         elif isinstance(operator, ast.GtE):
             yield node, ast.Constant(value=left >= right, kind=None)
 
         elif isinstance(operator, ast.LtE):
             yield node, ast.Constant(value=left <= right, kind=None)
 
 
-@processing.fix(restart_on_replace=True)
+@processing.fix
 def simplify_boolean_expressions_symmath(source: str) -> str:
     root = core.parse(source)
     for node in core.walk(root, (ast.BoolOp, ast.UnaryOp)):
         try:
             simplified = _simplify_ast_boolop(node)
         except ValueError:
             continue
@@ -834,9 +834,7 @@
                 keywords=[],
             )
 
         else:
             yield comp.iter, ast.Call(
                 func=ast.Name(id="range"), args=[ast.Constant(value=stop, kind=None)], keywords=[]
             )
-
-        return
```

### Comparing `pyrefact-90/pyrefact/tracing.py` & `pyrefact-91/pyrefact/tracing.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,26 +315,33 @@
 
         if isinstance(node, ast.NamedExpr) and core.match_template(node.target, ast.Name(id=name)):
             return _TraceResult(core.get_code(node, source), node.lineno, node)
 
     return None
 
 
+def get_defined_names(root: ast.Module) -> Collection[str]:
+    """Get names defined in scope, excluding imports."""
+    return (
+        {node.id for node in core.walk(root, ast.Name(ctx=ast.Store))}
+        | {node.name for node in core.walk(root, (ast.FunctionDef, ast.AsyncFunctionDef))}
+        | {node.name for node in core.walk(root, ast.ClassDef)}
+        | {node.arg for node in core.walk(root, ast.arg)}
+    )
+
+
+def _get_referenced_names(root: ast.Module) -> Collection[str]:
+    return {node.id for node in core.walk(root, ast.Name(ctx=ast.Load))}
+
+
 def get_undefined_variables(source: str) -> Collection[str]:
     root = core.parse(source)
     imported_names = get_imported_names(root)
-    defined_names = set()
-    referenced_names = set()
-    for node in core.walk(root, ast.Name):
-        if isinstance(node.ctx, ast.Load):
-            referenced_names.add(node.id)
-        elif isinstance(node.ctx, ast.Store):
-            defined_names.add(node.id)
-    for node in core.walk(root, ast.arg):
-        defined_names.add(node.arg)
+    defined_names = get_defined_names(root)
+    referenced_names = _get_referenced_names(root)
 
     return (
         referenced_names
         - defined_names
         - imported_names
         - {name.split(".")[0] for name in imported_names}
         - constants.BUILTIN_FUNCTIONS
@@ -379,26 +386,24 @@
 
     # Remove remaining starred imports
     for node in core.filter_nodes(root.body, template):
         if not core.match_template(node, tuple(starred_import_name_mapping)):
             yield node, None
 
 
+@processing.fix
 def fix_reimported_names(source: str) -> str:
     """Remove reimported names from imports."""
 
     root = core.parse(source)
 
     all_template = ast.Assign(
         targets=[ast.Name(id="__all__")], value=ast.List(elts={ast.Constant(value=str)})
     )
     module_from_imports = collections.defaultdict(set)
-    additions = set()
-    removals = set()
-    replacements = {}
 
     import_insert_lineno = min(
         (node.lineno for node in core.walk(root, (ast.ImportFrom, ast.Import))), default=-1
     )
     if import_insert_lineno == -1:
         return source  # No imports, nothing to do
 
@@ -458,36 +463,26 @@
                         if alias.asname == name or (alias.asname is None and alias.name == name)
                     )
                     if asname == original_name:
                         new_alias = ast.alias(name=original_name, asname=None)
                     else:
                         new_alias = ast.alias(name=original_name, asname=asname)
 
-                    additions.add(ast.Import(names=[new_alias]), lineno=import_insert_lineno)
+                    yield None, ast.Import(names=[new_alias], lineno=import_insert_lineno)
                 else:
                     node_names.append(alias)
             else:
                 node_names.append(alias)
 
         if node_names != node.names:
             if node_names:
-                replacements[node] = ast.ImportFrom(
-                    module=node.module, names=node_names, level=node.level
-                )
+                yield node, ast.ImportFrom(module=node.module, names=node_names, level=node.level)
             else:
-                removals.add(node)
+                yield node, None
 
     for module, aliases in module_from_imports.items():
-        additions.add(
-            ast.ImportFrom(
-                module=module,
-                names=sorted(aliases, key=lambda alias: alias.name),
-                level=0,
-                lineno=import_insert_lineno,
-        ))
-
-    if additions or removals or replacements:
-        source = processing.alter_code(
-            source, root, additions=additions, removals=removals, replacements=replacements
+        yield None, ast.ImportFrom(
+            module=module,
+            names=sorted(aliases, key=lambda alias: alias.name),
+            level=0,
+            lineno=import_insert_lineno,
         )
-
-    return source
```

### Comparing `pyrefact-90/pyrefact.egg-info/PKG-INFO` & `pyrefact-91/pyrefact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefact
-Version: 90
+Version: 91
 Summary: Automated Python refactoring
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2022 OlleLindgren
```

### Comparing `pyrefact-90/pyrefact.egg-info/SOURCES.txt` & `pyrefact-91/pyrefact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrefact-90/tests/testing_infra.py` & `pyrefact-91/tests/testing_infra.py`

 * *Files identical despite different names*

