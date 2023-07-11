# Comparing `tmp/pytest-archon-0.0.4.tar.gz` & `tmp/pytest-archon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-archon-0.0.4.tar", last modified: Tue Jan 31 19:26:24 2023, max compression
+gzip compressed data, was "pytest-archon-0.0.5.tar", last modified: Tue Jul 11 21:41:38 2023, max compression
```

## Comparing `pytest-archon-0.0.4.tar` & `pytest-archon-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.894163 pytest-archon-0.0.4/
--rw-r--r--   0 jwb        (502) staff       (20)    11357 2022-11-18 07:32:47.000000 pytest-archon-0.0.4/LICENSE
--rw-r--r--   0 jwb        (502) staff       (20)      111 2022-12-20 12:54:31.000000 pytest-archon-0.0.4/MANIFEST.in
--rw-r--r--   0 jwb        (502) staff       (20)     1637 2023-01-07 18:28:19.000000 pytest-archon-0.0.4/Makefile
--rw-r--r--   0 jwb        (502) staff       (20)     5580 2023-01-31 19:26:24.894001 pytest-archon-0.0.4/PKG-INFO
--rw-r--r--   0 jwb        (502) staff       (20)     4745 2023-01-09 09:39:25.000000 pytest-archon-0.0.4/README.md
--rw-r--r--   0 jwb        (502) staff       (20)     1518 2023-01-07 18:29:39.000000 pytest-archon-0.0.4/pyproject.toml
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.891659 pytest-archon-0.0.4/pytest_archon/
--rw-r--r--   0 jwb        (502) staff       (20)       54 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/__init__.py
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.890041 pytest-archon-0.0.4/pytest_archon/assets/
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.892910 pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/
--rw-r--r--   0 jwb        (502) staff       (20)    34003 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.6.txt
--rw-r--r--   0 jwb        (502) staff       (20)    35238 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.7.txt
--rw-r--r--   0 jwb        (502) staff       (20)    36209 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.8.txt
--rw-r--r--   0 jwb        (502) staff       (20)    16244 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.9.txt
--rw-r--r--   0 jwb        (502) staff       (20)     8307 2023-01-31 19:25:22.000000 pytest-archon-0.0.4/pytest_archon/collect.py
--rw-r--r--   0 jwb        (502) staff       (20)     1061 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/pytest_archon/core_modules.py
--rw-r--r--   0 jwb        (502) staff       (20)      648 2023-01-07 18:29:39.000000 pytest-archon-0.0.4/pytest_archon/failure.py
--rw-r--r--   0 jwb        (502) staff       (20)     1507 2023-01-07 18:29:39.000000 pytest-archon-0.0.4/pytest_archon/plugin.py
--rw-r--r--   0 jwb        (502) staff       (20)        0 2022-12-20 12:54:10.000000 pytest-archon-0.0.4/pytest_archon/py.typed
--rw-r--r--   0 jwb        (502) staff       (20)     8471 2023-01-30 16:54:05.000000 pytest-archon-0.0.4/pytest_archon/rule.py
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.892332 pytest-archon-0.0.4/pytest_archon.egg-info/
--rw-r--r--   0 jwb        (502) staff       (20)     5580 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/PKG-INFO
--rw-r--r--   0 jwb        (502) staff       (20)      807 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/SOURCES.txt
--rw-r--r--   0 jwb        (502) staff       (20)        1 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/dependency_links.txt
--rw-r--r--   0 jwb        (502) staff       (20)       39 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/entry_points.txt
--rw-r--r--   0 jwb        (502) staff       (20)       89 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/requires.txt
--rw-r--r--   0 jwb        (502) staff       (20)       25 2023-01-31 19:26:24.000000 pytest-archon-0.0.4/pytest_archon.egg-info/top_level.txt
--rw-r--r--   0 jwb        (502) staff       (20)       38 2023-01-31 19:26:24.894195 pytest-archon-0.0.4/setup.cfg
--rwxr-xr-x   0 jwb        (502) staff       (20)       92 2022-11-20 12:38:15.000000 pytest-archon-0.0.4/setup.py
-drwxr-xr-x   0 jwb        (502) staff       (20)        0 2023-01-31 19:26:24.893794 pytest-archon-0.0.4/tests/
--rw-r--r--   0 jwb        (502) staff       (20)      484 2023-01-07 16:25:20.000000 pytest-archon-0.0.4/tests/conftest.py
--rw-r--r--   0 jwb        (502) staff       (20)     3156 2022-11-29 17:57:17.000000 pytest-archon-0.0.4/tests/test_ast.py
--rw-r--r--   0 jwb        (502) staff       (20)     3176 2023-01-29 21:45:47.000000 pytest-archon-0.0.4/tests/test_collect.py
--rw-r--r--   0 jwb        (502) staff       (20)      447 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/tests/test_core_modules.py
--rw-r--r--   0 jwb        (502) staff       (20)      469 2022-11-26 08:13:58.000000 pytest-archon-0.0.4/tests/test_docstrings.py
--rw-r--r--   0 jwb        (502) staff       (20)      648 2023-01-07 18:29:39.000000 pytest-archon-0.0.4/tests/test_pytest_fixture.py
--rw-r--r--   0 jwb        (502) staff       (20)     6523 2023-01-31 19:25:22.000000 pytest-archon-0.0.4/tests/test_rule.py
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.184511 pytest-archon-0.0.5/
+-rw-r--r--   0 jwb        (501) staff       (20)    11357 2022-11-18 07:32:47.000000 pytest-archon-0.0.5/LICENSE
+-rw-r--r--   0 jwb        (501) staff       (20)      111 2022-12-20 12:54:31.000000 pytest-archon-0.0.5/MANIFEST.in
+-rw-r--r--   0 jwb        (501) staff       (20)     1637 2023-01-07 18:28:19.000000 pytest-archon-0.0.5/Makefile
+-rw-r--r--   0 jwb        (501) staff       (20)     6572 2023-07-11 21:41:38.184217 pytest-archon-0.0.5/PKG-INFO
+-rw-r--r--   0 jwb        (501) staff       (20)     5701 2023-07-11 21:32:50.000000 pytest-archon-0.0.5/README.md
+-rw-r--r--   0 jwb        (501) staff       (20)     1514 2023-07-10 09:59:36.000000 pytest-archon-0.0.5/pyproject.toml
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.178942 pytest-archon-0.0.5/pytest_archon/
+-rw-r--r--   0 jwb        (501) staff       (20)       54 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/__init__.py
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.175331 pytest-archon-0.0.5/pytest_archon/assets/
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.181875 pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/
+-rw-r--r--   0 jwb        (501) staff       (20)    34003 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.6.txt
+-rw-r--r--   0 jwb        (501) staff       (20)    35238 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.7.txt
+-rw-r--r--   0 jwb        (501) staff       (20)    36209 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.8.txt
+-rw-r--r--   0 jwb        (501) staff       (20)    16244 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.9.txt
+-rw-r--r--   0 jwb        (501) staff       (20)     8307 2023-07-10 09:59:36.000000 pytest-archon-0.0.5/pytest_archon/collect.py
+-rw-r--r--   0 jwb        (501) staff       (20)     1061 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/pytest_archon/core_modules.py
+-rw-r--r--   0 jwb        (501) staff       (20)      648 2023-01-07 18:29:39.000000 pytest-archon-0.0.5/pytest_archon/failure.py
+-rw-r--r--   0 jwb        (501) staff       (20)     1507 2023-01-07 18:29:39.000000 pytest-archon-0.0.5/pytest_archon/plugin.py
+-rw-r--r--   0 jwb        (501) staff       (20)        0 2022-12-20 12:54:10.000000 pytest-archon-0.0.5/pytest_archon/py.typed
+-rw-r--r--   0 jwb        (501) staff       (20)    10049 2023-07-11 21:16:49.000000 pytest-archon-0.0.5/pytest_archon/rule.py
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.180598 pytest-archon-0.0.5/pytest_archon.egg-info/
+-rw-r--r--   0 jwb        (501) staff       (20)     6572 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/PKG-INFO
+-rw-r--r--   0 jwb        (501) staff       (20)      807 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/SOURCES.txt
+-rw-r--r--   0 jwb        (501) staff       (20)        1 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/dependency_links.txt
+-rw-r--r--   0 jwb        (501) staff       (20)       39 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/entry_points.txt
+-rw-r--r--   0 jwb        (501) staff       (20)       89 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/requires.txt
+-rw-r--r--   0 jwb        (501) staff       (20)       25 2023-07-11 21:41:38.000000 pytest-archon-0.0.5/pytest_archon.egg-info/top_level.txt
+-rw-r--r--   0 jwb        (501) staff       (20)       38 2023-07-11 21:41:38.184599 pytest-archon-0.0.5/setup.cfg
+-rwxr-xr-x   0 jwb        (501) staff       (20)       92 2022-11-20 12:38:15.000000 pytest-archon-0.0.5/setup.py
+drwxr-xr-x   0 jwb        (501) staff       (20)        0 2023-07-11 21:41:38.183807 pytest-archon-0.0.5/tests/
+-rw-r--r--   0 jwb        (501) staff       (20)      484 2023-01-07 16:25:20.000000 pytest-archon-0.0.5/tests/conftest.py
+-rw-r--r--   0 jwb        (501) staff       (20)     3156 2022-11-29 17:57:17.000000 pytest-archon-0.0.5/tests/test_ast.py
+-rw-r--r--   0 jwb        (501) staff       (20)     3171 2023-07-10 09:59:36.000000 pytest-archon-0.0.5/tests/test_collect.py
+-rw-r--r--   0 jwb        (501) staff       (20)      447 2022-11-26 08:13:58.000000 pytest-archon-0.0.5/tests/test_core_modules.py
+-rw-r--r--   0 jwb        (501) staff       (20)      468 2023-07-10 09:59:36.000000 pytest-archon-0.0.5/tests/test_docstrings.py
+-rw-r--r--   0 jwb        (501) staff       (20)      648 2023-01-07 18:29:39.000000 pytest-archon-0.0.5/tests/test_pytest_fixture.py
+-rw-r--r--   0 jwb        (501) staff       (20)     7610 2023-07-11 21:16:49.000000 pytest-archon-0.0.5/tests/test_rule.py
```

### Comparing `pytest-archon-0.0.4/LICENSE` & `pytest-archon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/Makefile` & `pytest-archon-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/PKG-INFO` & `pytest-archon-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-archon
-Version: 0.0.4
-Summary: Rule your architecture like a real developer
-Author-email: gaphor@gmail.com, jw@bargsten.org
-License: Apache Software License
-Project-URL: homepage, https://github.com/jwbargsten/pytest-archon
-Project-URL: repository, https://github.com/jwbargsten/pytest-archon
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Framework :: Pytest
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pytest-archon
 
 [![build_and_test](https://github.com/jwbargsten/pytest-archon/actions/workflows/tests.yml/badge.svg)](https://github.com/jwbargsten/pytest-archon/actions/workflows/tests.yml)
 
 `pytest-archon` is a little tool that helps you structure (large) Python projects. This
 tool allows you to define architectural boundaries in your code, also known as
 _forbidden dependencies_.
@@ -105,14 +84,40 @@
         .match("packageX.domain*") # matches packageX.domain and packageX.domain.*
         .should_not_import("packageX*")
         .may_import("packageX.domain.*")
         .check("packageX")
     )
 ```
 
+### `util` module is used at more than one place
+
+You can also supply custom constraints as predicate functions.
+
+If you, for example, have a common or util module, you might want to make sure that it
+is used at least at two places (otherwise it would not make sense to have a separate
+module).
+
+```python
+from pytest_archon import archrule
+
+
+def test_utils_are_shared():
+    def have_at_least_two_users(util_module, direct_imports, all_imports):
+        # iterate through all imports and find modules using the util_module in question
+        users = [k for k, v in all_imports.items() if util_module in v]
+        # return True if more than two modules use the util_module
+        return len(users) > 2
+
+    archrule("util_is_shared").match("pkg.util").should(have_at_least_two_users).check("pkg")
+```
+
+## See also
+
+The blog post [How to tame your Python codebase](https://bargsten.org/wissen/how-to-tame-your-python-codebase/) is also a good overview.
+
 ## Similar projects
 
 - [Archunit](https://www.archunit.org/) (Java)
 - [Dependency Cruiser](https://github.com/sverweij/dependency-cruiser) (Javascript)
 - [import-linter](https://github.com/seddonym/import-linter) (Python)
 - [pytestarch](https://pypi.org/project/pytestarch/) (Python)
 - [Maintain A Clean Architecture With Dependency Rules - sourcery.ai](https://sourcery.ai/blog/dependency-rules/)
```

### Comparing `pytest-archon-0.0.4/pyproject.toml` & `pytest-archon-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-archon"
 description = "Rule your architecture like a real developer"
 authors = [
-    { author = "Arjan Molenaar", email = "gaphor@gmail.com" },
-    { author = "Joachim Bargsten", email = "jw@bargsten.org" }
+    { name = "Arjan Molenaar", email = "gaphor@gmail.com" },
+    { name = "Joachim Bargsten", email = "jw@bargsten.org" }
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache Software License" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.6.txt` & `pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.6.txt`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.7.txt` & `pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.7.txt`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.8.txt` & `pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.8.txt`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/assets/core-module-lists/3.9.txt` & `pytest-archon-0.0.5/pytest_archon/assets/core-module-lists/3.9.txt`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/collect.py` & `pytest-archon-0.0.5/pytest_archon/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import ast
 import os
 import re
 import sys
 from collections import deque
 from functools import lru_cache
 from importlib.util import find_spec
+from logging import getLogger
 from pathlib import Path
 from types import ModuleType
-from typing import Callable, Dict, Iterator, Set, Iterable, Sequence
-from logging import getLogger
+from typing import Callable, Dict, Iterable, Iterator, Sequence, Set
 
 from pytest_archon.core_modules import core_modules
 
 # https://docs.djangoproject.com/en/4.1/_modules/django/utils/module_loading/
 # https://stackoverflow.com/questions/54325116/can-i-handle-imports-in-an-abstract-syntax-tree
 # https://bugs.python.org/issue38721
 # https://github.com/0cjs/sedoc/blob/master/lang/python/importers.md
```

### Comparing `pytest-archon-0.0.4/pytest_archon/core_modules.py` & `pytest-archon-0.0.5/pytest_archon/core_modules.py`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/failure.py` & `pytest-archon-0.0.5/pytest_archon/failure.py`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/plugin.py` & `pytest-archon-0.0.5/pytest_archon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/pytest_archon/rule.py` & `pytest-archon-0.0.5/pytest_archon/rule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
-from dataclasses import dataclass
-import re
 
+import re
+from dataclasses import dataclass
 from fnmatch import fnmatchcase
 from types import ModuleType
+from typing import Callable, Set
+
 
 from pytest_archon.collect import (
     ImportMap,
     collect_imports,
+    recurse_imports,
     walk,
     walk_runtime,
     walk_toplevel,
-    recurse_imports,
 )
 from pytest_archon.failure import add_failure  # type: ignore[import]
 
 
+ConstraintPredicate = Callable[[str, Set[str], ImportMap], bool]
+
+
 @dataclass
 class RulePattern:
     is_regex: bool
     pattern: str
 
     def match(self, k: str):
         if self.is_regex:
@@ -90,14 +95,29 @@
 
         Keep in mind that module dependencies are checked transtively.
 
         E.g. 'mymodule.submodule', 'mymodule.*'
         """
         return RuleConstraints(self.rule, self).should_not_import(*pattern, **kwargs)
 
+    def should(self, pred: ConstraintPredicate, name=None) -> RuleConstraints:
+        """Define a constraint using a supplied function/predicate.
+
+        If the predicate function returns ``False``, the constraint is
+        considered as being violated.
+
+        :param pred: a function with the signature
+            ``pred(module, direct_imports, all_imports)``
+        :type pred: ConstraintPredicate
+        :param name: An optional name for this constraint. If omitted,
+            the name will be inferred from the predicate function.
+        :rtype: RuleConstraints
+        """
+        return RuleConstraints(self.rule, self).should(pred, name)
+
     def should_import(self, *pattern: str, **kwargs) -> RuleConstraints:
         """Define a constraint that the defined modules should
         import modules that match the given pattern.
 
         Keep in mind that module dependencies are checked transtively.
 
         E.g. 'mymodule.submodule', 'mymodule.*'
@@ -115,14 +135,15 @@
 class RuleConstraints:
     def __init__(self, rule: Rule, targets: RuleTargets) -> None:
         self.rule = rule
         self.targets = targets
         self.forbidden: list[RulePattern] = []
         self.required: list[RulePattern] = []
         self.ignored: list[RulePattern] = []
+        self.constraint_preds: list[tuple[ConstraintPredicate, str]] = []
 
     def should_not_import(self, *pattern: str) -> RuleConstraints:
         """Define a constraint that the defined modules should
         not import modules that match the given pattern.
 
         Keep in mind that module dependencies are checked transtively.
 
@@ -138,14 +159,18 @@
         Keep in mind that module dependencies are checked transtively.
 
         E.g. 'mymodule.submodule', 'mymodule.*'
         """
         self.required.extend(_as_rule_patterns(self.rule.use_regex, pattern))
         return self
 
+    def should(self, pred: ConstraintPredicate, name=None):
+        self.constraint_preds.append((pred, name or pred.__name__))
+        return self
+
     def may_import(self, *pattern: str) -> RuleConstraints:
         """Loosen the constraints from should_import and
         should_not_import: modules matching may_import are
         excluded/ignored from the constraint check.
         """
         self.ignored.extend(_as_rule_patterns(self.rule.use_regex, pattern))
         return self
@@ -209,31 +234,46 @@
             import_map = {candidate: all_imports[candidate]} if only_direct_imports else all_imports
 
             for constraint in self._find_required_constraints(candidate, import_map):
                 add_failure(
                     rule_name,
                     rule_comment,
                     f"module '{candidate}' is missing REQUIRED imports matching {constraint}",
+                    ["."],
                 )
 
             for constraint, path in self._find_forbidden_constraints(candidate, import_map):
                 add_failure(
                     rule_name,
                     rule_comment,
-                    f"module '{candidate}' has FORBIDDEN import {path[-1]} (matched by {constraint}) ",
+                    f"module '{candidate}' has FORBIDDEN import {path[-1]} (matched by {constraint})",
                     path,
                 )
 
+            for constraint in self._find_constraint_predicates(candidate, import_map):
+                add_failure(
+                    rule_name,
+                    rule_comment,
+                    f"module '{candidate}' VIOLATED constraint '{constraint}'",
+                    ["."],
+                )
+
     def _find_required_constraints(self, module: str, all_imports: ImportMap):
         for constraint in self.required:
             if not any(
                 imp for path in recurse_imports(module, all_imports) if constraint.match(imp := path[-1])
             ):
                 yield constraint
 
+    def _find_constraint_predicates(self, module: str, all_imports: ImportMap):
+        direct_imports = all_imports[module]
+        for pred, name in self.constraint_preds:
+            if not pred(module, direct_imports, all_imports):
+                yield name
+
     def _find_forbidden_constraints(
         self,
         module: str,
         all_imports: ImportMap,
     ):
         for constraint in self.forbidden:
             yield from (
```

### Comparing `pytest-archon-0.0.4/pytest_archon.egg-info/PKG-INFO` & `pytest-archon-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytest-archon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rule your architecture like a real developer
-Author-email: gaphor@gmail.com, jw@bargsten.org
+Author-email: Arjan Molenaar <gaphor@gmail.com>, Joachim Bargsten <jw@bargsten.org>
 License: Apache Software License
 Project-URL: homepage, https://github.com/jwbargsten/pytest-archon
 Project-URL: repository, https://github.com/jwbargsten/pytest-archon
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -105,14 +105,40 @@
         .match("packageX.domain*") # matches packageX.domain and packageX.domain.*
         .should_not_import("packageX*")
         .may_import("packageX.domain.*")
         .check("packageX")
     )
 ```
 
+### `util` module is used at more than one place
+
+You can also supply custom constraints as predicate functions.
+
+If you, for example, have a common or util module, you might want to make sure that it
+is used at least at two places (otherwise it would not make sense to have a separate
+module).
+
+```python
+from pytest_archon import archrule
+
+
+def test_utils_are_shared():
+    def have_at_least_two_users(util_module, direct_imports, all_imports):
+        # iterate through all imports and find modules using the util_module in question
+        users = [k for k, v in all_imports.items() if util_module in v]
+        # return True if more than two modules use the util_module
+        return len(users) > 2
+
+    archrule("util_is_shared").match("pkg.util").should(have_at_least_two_users).check("pkg")
+```
+
+## See also
+
+The blog post [How to tame your Python codebase](https://bargsten.org/wissen/how-to-tame-your-python-codebase/) is also a good overview.
+
 ## Similar projects
 
 - [Archunit](https://www.archunit.org/) (Java)
 - [Dependency Cruiser](https://github.com/sverweij/dependency-cruiser) (Javascript)
 - [import-linter](https://github.com/seddonym/import-linter) (Python)
 - [pytestarch](https://pypi.org/project/pytestarch/) (Python)
 - [Maintain A Clean Architecture With Dependency Rules - sourcery.ai](https://sourcery.ai/blog/dependency-rules/)
```

### Comparing `pytest-archon-0.0.4/pytest_archon.egg-info/SOURCES.txt` & `pytest-archon-0.0.5/pytest_archon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/tests/test_ast.py` & `pytest-archon-0.0.5/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/tests/test_collect.py` & `pytest-archon-0.0.5/tests/test_collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 from pathlib import Path
 
 from pytest_archon.collect import (
     collect_imports_from_path,
     path_to_module,
+    recurse_imports,
     resolve_module_or_object_by_path,
     resolve_module_or_object_by_spec,
-    recurse_imports,
 )
 
 
 def test_collect_modules(create_testset):
     path = create_testset(("mymodule.py", ""))
     collected = list(name for name, _ in collect_imports_from_path(path, "pkg"))
     assert "pkg.mymodule" in collected
 
 
 def test_collect_with_system_modules(create_testset):
-
     path = create_testset(("mymodule.py", "import sys, os"))
 
     name, imports = next(iter(collect_imports_from_path(path, "pkg")))
 
     assert name == "pkg.mymodule"
     assert "sys" in imports
     assert "os" in imports
 
 
 def test_path_to_module():
     assert path_to_module(Path("a/b/./c/d/../e"), Path("a/b/c")) == "d.e"
 
 
 def test_module_imports_other_module(create_testset):
-
     path = create_testset(("module.py", ""), ("othermodule.py", "import module"))
 
     module_names = {i for name, imports in collect_imports_from_path(path, "pkg") for i in imports}
 
     assert "module" in module_names
     assert "othermodule" not in module_names
 
 
 def test_module_import_from(create_testset):
-
     path = create_testset(("module.py", "val = 1"), ("othermodule.py", "from module import val"))
 
     module_names = {i for name, imports in collect_imports_from_path(path, "pkg") for i in imports}
     assert module_names == {"module"}
 
 
 def test_module_import_nested_modules(create_testset):
-
     path = create_testset(
         ("package/__init__.py", ""),
         ("package/module.py", ""),
         ("package/othermodule.py", "import package.module"),
     )
 
     module_names = {i for name, imports in collect_imports_from_path(path, "package") for i in imports}
 
     assert "package.module" in module_names
     assert "package.othermodule" not in module_names
     assert "othermodule" not in module_names
 
 
 def test_relative_imports(create_testset):
-
     path = create_testset(
         ("package/__init__.py", ""),
         ("package/module.py", "from .importme import val"),
         ("package/importme.py", "val = 1"),
         ("package/sub/__init__.py", ""),
         ("package/sub/deep.py", "from ..importme import val"),
     )
```

### Comparing `pytest-archon-0.0.4/tests/test_pytest_fixture.py` & `pytest-archon-0.0.5/tests/test_pytest_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-archon-0.0.4/tests/test_rule.py` & `pytest-archon-0.0.5/tests/test_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import re
+
 import pytest_archon
 from pytest_archon import archrule
 from pytest_archon.failure import pop_failures
 from pytest_archon.plugin import format_failures
-import re
 
 
 def test_rule_basic():
     (archrule("basic rule").match("*.collect").should_not_import("pytest_archon.rule").check(pytest_archon))
 
 
 def test_rule_exclusion():
@@ -36,14 +37,52 @@
         archrule("rule exclusion")
         .match("pytest_archon.plugin")
         .should_import("pytest_archon.rule")
         .check(pytest_archon)
     )
 
 
+def test_rule_should_check_predicate1():
+    def have_more_than_2_deps(m, di, ai):
+        return len(di) > 2
+
+    (
+        archrule("rule exclusion")
+        .match("pytest_archon.rule")
+        .should(have_more_than_2_deps)
+        .check(pytest_archon)
+    )
+
+
+def test_rule_should_check_predicate2():
+    def have_collect_import(m, di, ai):
+        return "pytest_archon.collect" in di
+
+    (archrule("rule exclusion").match("pytest_archon.rule").should(have_collect_import).check(pytest_archon))
+
+
+def test_failing_predicate(create_testset):
+    def not_include_module_b(m, di, ai):
+        return "abcz.moduleB" not in di
+
+    create_testset(
+        ("abcz/__init__.py", ""),
+        ("abcz/moduleA.py", "import abcz.moduleB"),
+    )
+    (archrule("rule constraint").match("abcz.moduleA").should(not_include_module_b).check("abcz"))
+
+    failures = pop_failures()
+    longrepr = format_failures(failures)
+
+    assert failures
+
+    assert "FAILED Rule 'rule constraint':" in longrepr
+    assert "- module 'abcz.moduleA' VIOLATED constraint 'not_include_module_b'" in longrepr
+
+
 def test_rule_should_import_list():
     (
         archrule("rule exclusion")
         .match("pytest_archon.plugin")
         .should_import("pytest_archon.rule", "pytest")
         .check(pytest_archon)
     )
```

