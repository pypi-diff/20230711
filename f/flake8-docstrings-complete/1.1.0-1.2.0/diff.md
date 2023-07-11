# Comparing `tmp/flake8_docstrings_complete-1.1.0.tar.gz` & `tmp/flake8_docstrings_complete-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_docstrings_complete-1.1.0.tar", max compression
+gzip compressed data, was "flake8_docstrings_complete-1.2.0.tar", max compression
```

## Comparing `flake8_docstrings_complete-1.1.0.tar` & `flake8_docstrings_complete-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/LICENSE
--rw-r--r--   0        0        0    34796 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/README.md
--rw-r--r--   0        0        0    20172 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/__init__.py
--rw-r--r--   0        0        0     5216 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/args.py
--rw-r--r--   0        0        0    11700 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/attrs.py
--rw-r--r--   0        0        0      177 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/constants.py
--rw-r--r--   0        0        0     5723 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/docstring.py
--rw-r--r--   0        0        0     6325 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/raises.py
--rw-r--r--   0        0        0      953 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/types_.py
--rw-r--r--   0        0        0     1560 2023-01-26 02:38:17.145496 flake8_docstrings_complete-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    37245 1970-01-01 00:00:00.000000 flake8_docstrings_complete-1.1.0/setup.py
--rw-r--r--   0        0        0    35955 1970-01-01 00:00:00.000000 flake8_docstrings_complete-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/LICENSE
+-rw-r--r--   0        0        0    35045 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/README.md
+-rw-r--r--   0        0        0    20172 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/__init__.py
+-rw-r--r--   0        0        0     5216 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/args.py
+-rw-r--r--   0        0        0    12029 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/attrs.py
+-rw-r--r--   0        0        0      177 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/constants.py
+-rw-r--r--   0        0        0     5723 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/docstring.py
+-rw-r--r--   0        0        0     6325 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/raises.py
+-rw-r--r--   0        0        0      953 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/types_.py
+-rw-r--r--   0        0        0     1560 2023-07-11 15:43:25.978160 flake8_docstrings_complete-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    36004 1970-01-01 00:00:00.000000 flake8_docstrings_complete-1.2.0/PKG-INFO
```

### Comparing `flake8_docstrings_complete-1.1.0/LICENSE` & `flake8_docstrings_complete-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/README.md` & `flake8_docstrings_complete-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1420,14 +1420,24 @@
     def bar(self):
         return "bar"
 
 class FooClass:
     """Perform foo action.
 
     Attrs:
+    """
+
+    @functools.cached_property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
         bar: The value to perform the foo action on.
     """
     bar = "bar"
     baz = "baz"
 ```
 
 These examples can be fixed by adding the missing attributes to the attributes
@@ -1462,14 +1472,25 @@
         return "bar"
 
 class FooClass:
     """Perform foo action.
 
     Attrs:
         bar: The value to perform the foo action on.
+    """
+
+    @functools.cached_property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
         baz: The alternate value to perform the foo action on.
     """
     bar = "bar"
     baz = "baz"
 ```
 
 ### Fix DCO064
@@ -1645,10 +1666,9 @@
    and any characters within round brackets followed by a colon.
 3. The section ends if any line with zero or more whitespace characters is
    encountered or the end of the docstring is reached.
 
 ## Future Ideas:
 
 - Check that argument, exceptions and attributes have non-empty description.
-- Check that arguments, exceptions and attributes are only documented once.
 - Check that arguments, exceptions and attributes have meaningful descriptions.
 - Check other other PEP257 conventions
```

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/__init__.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/args.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/args.py`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/attrs.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,31 @@
     Args:
         node: The node to check.
 
     Returns:
         Whether the node is a property decorator.
     """
     if isinstance(node, ast.Name):
-        return node.id == "property"
+        return node.id in {"property", "cached_property"}
 
     # Handle call
     if isinstance(node, ast.Call):
         return is_property_decorator(node=node.func)
 
-    return False
+    # Handle attr
+    if isinstance(node, ast.Attribute):
+        value = node.value
+        return (
+            node.attr == "cached_property"
+            and isinstance(value, ast.Name)
+            and value.id == "functools"
+        )
+
+    # There is no valid syntax that gets to here
+    return False  # pragma: nocover
 
 
 def _get_class_target_name(target: ast.expr) -> ast.Name | None:
     """Get the name of the target for an assignment on the class.
 
     Args:
         target: The target node of an assignment expression.
```

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/docstring.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/docstring.py`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/raises.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/raises.py`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/flake8_docstrings_complete/types_.py` & `flake8_docstrings_complete-1.2.0/flake8_docstrings_complete/types_.py`

 * *Files identical despite different names*

### Comparing `flake8_docstrings_complete-1.1.0/pyproject.toml` & `flake8_docstrings_complete-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-docstrings-complete"
-version = "1.1.0"
+version = "1.2.0"
 description = "A linter that checks docstrings are complete"
 authors = ["David Andersson <david@jdkandersson.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "flake8_docstrings_complete"}]
 classifiers = [
     "Framework :: Flake8",
```

### Comparing `flake8_docstrings_complete-1.1.0/setup.py` & `flake8_docstrings_complete-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,1699 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flake8-docstrings-complete
+Version: 1.2.0
+Summary: A linter that checks docstrings are complete
+License: Apache 2.0
+Author: David Andersson
+Author-email: david@jdkandersson.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Environment :: Console
+Classifier: Framework :: Flake8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: flake8 (>=5)
+Description-Content-Type: text/markdown
 
-packages = \
-['flake8_docstrings_complete']
+# flake8-docstrings-complete
 
-package_data = \
-{'': ['*']}
+Linter that checks docstrings of functions, methods and classes. It should be
+used in conjunction with `pydocstyle` (or `flake8-docstrings`) as the linter
+assumes that the docstrings already pass `pydocstyle` checks. This
+[blog post](https://jdkandersson.com/2023/01/07/writing-great-docstrings-in-python/)
+discusses how to write great docstrings and the motivation for this linter!
 
-install_requires = \
-['flake8>=5']
-
-entry_points = \
-{'flake8.extension': ['DCO = flake8_docstrings_complete:Plugin']}
-
-setup_kwargs = {
-    'name': 'flake8-docstrings-complete',
-    'version': '1.1.0',
-    'description': 'A linter that checks docstrings are complete',
-    'long_description': '# flake8-docstrings-complete\n\nLinter that checks docstrings of functions, methods and classes. It should be\nused in conjunction with `pydocstyle` (or `flake8-docstrings`) as the linter\nassumes that the docstrings already pass `pydocstyle` checks. This\n[blog post](https://jdkandersson.com/2023/01/07/writing-great-docstrings-in-python/)\ndiscusses how to write great docstrings and the motivation for this linter!\n\n## Getting Started\n\n```shell\npython -m venv venv\nsource ./venv/bin/activate\npip install flake8 flake8-docstrings flake8-docstrings-complete\nflake8 source.py\n```\n\nOn the following code where the `foo` function has the `bar` and `baz`\narguments where the `baz` argument is missing from the `Args` section in the\ndocstring:\n\n```Python\n# source.py\ndef foo(bar, baz):\n    """Perform foo action on bar.\n\n    Args:\n        bar: The value to perform the foo action on.\n    """\n```\n\nThis will produce warnings such as:\n\n```shell\nflake8 test_source.py\nsource.py:2:14: DCO023 "baz" argument should be described in the docstring, more information: https://github.com/jdkandersson/flake8-docstrings-complete#fix-dco023\n```\n\nThis can be resolved by adding the `baz` argument to the `Args` section:\n\n```Python\n# source.py\ndef foo(bar, baz):\n    """Perform foo action on bar.\n\n    Args:\n        bar: The value to perform the foo action on.\n        baz: The modifier to the foo action.\n    """\n```\n\n`flake8-docstrings-complete` adds the following checks to complement\n`pydocstyle`:\n\n1. If a function/ method has arguments, that the arguments section is included.\n2. If a function/ method has arguments, that all function/ method arguments are\n   in the argument section.\n3. If an arguments section is in the function/ method docstring, the argument\n   section contains no arguments the function/ method doesn\'t have.\n4. Function/ method arguments are only documented once.\n5. If a function/ method has a return statement with a value, the return value\n   section is included.\n6. If a function/ method has a yield statement with a value, the yield value\n   section is included.\n7. If a function/ method raises an exception, the raises section is included\n   with a description for each exception that is raised.\n8. Each raised exception is only described once.\n9. If a class has public attributes, that the attributes section is included.\n10. If a class has public attributes, that all public attributes are in the\n   attributes section.\n11. If an attributes section is in the class docstring, the attributes section\n   contains no attributes the class doesn\'t have.\n12. Class attributes are only documented once.\n13. Any of the sections being checked are not present multiple times.\n\nNote:\n\n- `self` and `cls` are not counted as arguments.\n- `test_.*` methods are skipped in `test_.*\\.py` files (function and file names\n  are configurable).\n- functions with a `@fixture` et al dectorator in `conftest.py` and\n  `test_.*\\.py` files are skipped (function and fixture file names are\n  configurable)\n\n## Configuration\n\nThe plugin adds the following configurations to `flake8`:\n\n- `--docstrings-complete-test-filename-pattern`: The filename pattern for test\n  files. Defaults to `test_.*\\.py`.\n- `--docstrings-complete-test-function-pattern`: The function name pattern for\n  test functions. Defaults to `test_.*`.\n- `--docstrings-complete-fixture-filename-pattern`: The filename pattern for\n  fixture files. Defaults to `conftest\\.py`.\n- `--docstrings-complete-fixture-decorator-pattern`: The decorator name pattern\n  for fixture functions. Defaults to `(^|\\.)fixture$`.\n\n## Rules\n\nA few rules have been defined to allow for selective suppression:\n\n- `DCO010`: docstring missing on a function/ method/ class.\n- `DCO020`: function/ method has one or more arguments and the docstring does\n  not have an arguments section.\n- `DCO021`: function/ method with no arguments and the docstring has an\n  arguments section.\n- `DCO022`: function/ method with one or more arguments and the docstring has\n  multiple arguments sections.\n- `DCO023`: function/ method has one or more arguments not described in the\n  docstring.\n- `DCO024`: function/ method has one or more arguments described in the\n  docstring which are not arguments of the function/ method.\n- `DCO025`: function/ method has one or more arguments described in the\n  docstring multiple times.\n- `DCO030`: function/ method that returns a value does not have the returns\n  section in the docstring.\n- `DCO031`: function/ method that does not return a value has the returns\n  section in the docstring.\n- `DCO032`: function/ method that returns a value and the docstring has\n  multiple returns sections.\n- `DCO040`: function/ method that yields a value does not have the yields\n  section in the docstring.\n- `DCO041`: function/ method that does not yield a value has the yields\n  section in the docstring.\n- `DCO042`: function/ method that yields a value and the docstring has\n  multiple yields sections.\n- `DCO050`: function/ method raises one or more exceptions and the docstring\n  does not have a raises section.\n- `DCO051`: function/ method that raises no exceptions and the docstring has a\n  raises section.\n- `DCO052`: function/ method that raises one or more exceptions and the\n  docstring has multiple raises sections.\n- `DCO053`: function/ method that raises one or more exceptions where one or\n  more of the exceptions is not described in the docstring.\n- `DCO054`: function/ method has one or more exceptions described in the\n  docstring which are not raised in the function/ method.\n- `DCO055`: function/ method that has a raise without an exception has an empty\n  raises section in the docstring.\n- `DCO056`: function/ method has one or more exceptions described in the\n  docstring multiple times.\n- `DCO060`: class has one or more public attributes and the docstring does not\n  have an attributes section.\n- `DCO061`: class with no attributes and the docstring has an attributes\n  section.\n- `DCO062`: class with one or more attributes and the docstring has multiple\n  attributes sections.\n- `DCO063`: class has one or more public attributes not described in the\n  docstring.\n- `DCO064`: class has one or more attributes described in the docstring which\n  are not attributes of the class.\n- `DCO065`: class has one or more attributes described in the docstring\n  multiple times.\n\n### Fix DCO010\n\nThis linting rule is triggered by a function/ method/ class without a\ndocstring. For example:\n\n```Python\ndef foo():\n    pass\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n        pass\n\nclass FooClass:\n    """Perform foo action."""\n    def foo(self):\n        pass\n```\n\nThis example can be fixed by adding a docstring:\n\n```Python\ndef foo():\n    """Perform foo action."""\n\nclass FooClass:\n    """Perform foo action."""\n    def foo(self):\n        """Perform foo action."""\n```\n\n### Fix DCO020\n\nThis linting rule is triggered by a function/ method that has one or more\narguments with a docstring that does not have an arguments section. For\nexample:\n\n```Python\ndef foo(bar):\n    """Perform foo action."""\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action."""\n```\n\nThese examples can be fixed by adding the arguments section and describing all\narguments in the arguments section:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar):\n    """Perform foo action.\n\n    Arguments:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar):\n    """Perform foo action.\n\n    Parameters:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\n### Fix DCO021\n\nThis linting rule is triggered by a function/ method that has no arguments with\na docstring that has an arguments section. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo():\n    """Perform foo action.\n\n    Arguments:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo():\n    """Perform foo action.\n\n    Parameters:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\nThese examples can be fixed by removing the arguments section:\n\n```Python\ndef foo():\n    """Perform foo action."""\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n```\n\n### Fix DCO022\n\nThis linting rule is triggered by a function/ method that has one or more\narguments and a docstring that has multiple arguments sections. For example:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n\n    Arguments:\n        bar: the value to perform the foo action on.\n\n    Parameters:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\nThese examples can be fixed by removing the additional arguments sections:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar):\n    """Perform foo action.\n\n    Arguments:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar):\n    """Perform foo action.\n\n    Parameters:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\n### Fix DCO023\n\nThis linting rule is triggered by a function/ method that has one or more\narguments where one or more of those arguments is not described in the\ndocstring. For example:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n    """\n\ndef foo(bar, baz):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n        """\n```\n\nThese examples can be fixed by adding the missing arguments to the arguments\nsection:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\ndef foo(bar, baz):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n        baz: the modifier to the foo action.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\n### Fix DCO024\n\nThis linting rule is triggered by a function/ method that has one or more\narguments and a docstring that describes one or more arguments where on or more\nof the described arguments are not arguments of the function/ method. For\nexample:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n        baz: the modifier to the foo action.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n            baz: the modifier to the foo action.\n        """\n```\n\nThese examples can be fixed by removing the arguments the function/ method\ndoesn\'t have from the docstring:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\n### Fix DCO025\n\nThis linting rule is triggered by a function/ method that has one or more\narguments and a docstring that describes one or more arguments where on or more\nof the described arguments are described multiple times. For example:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n            bar: the value to perform the foo action on.\n        """\n```\n\nThese examples can be fixed by removing the duplicate arguments from the docstring:\n\n```Python\ndef foo(bar):\n    """Perform foo action.\n\n    Args:\n        bar: the value to perform the foo action on.\n    """\n\nclass FooClass:\n    def foo(self, bar):\n        """Perform foo action.\n\n        Args:\n            bar: the value to perform the foo action on.\n        """\n```\n\n### Fix DCO030\n\nThis linting rule is triggered by a function/ method that has at least one\nreturn statement with a value and does not have a returns section in the\ndocstring. For example:\n\n```Python\ndef foo():\n    """Return bar."""\n    return "bar"\n\nclass FooClass:\n    def foo(self):\n        """Return bar."""\n        return "bar"\n```\n\nThese examples can be fixed by adding the returns section:\n\n```Python\ndef foo():\n    """Return bar.\n\n    Return:\n        bar.\n    """\n    return "bar"\n\ndef foo():\n    """Return bar.\n\n    Returns:\n        bar.\n    """\n    return "bar"\n\nclass FooClass:\n    def foo(self):\n        """Return bar.\n\n        Returns:\n            bar.\n        """\n        return "bar"\n```\n\n### Fix DCO031\n\nThis linting rule is triggered by a function/ method that has no return\nstatement with a value and has a returns section in the\ndocstring. For example:\n\n```Python\ndef foo():\n    """Return bar.\n\n    Returns:\n        bar.\n    """\n    pass\n\nclass FooClass:\n    def foo(self):\n        """Return bar.\n\n        Returns:\n            bar.\n        """\n        pass\n```\n\nThese examples can be fixed by removing the returns section:\n\n```Python\ndef foo():\n    """Take foo action."""\n    pass\n\nclass FooClass:\n    def foo(self):\n        """Take foo action."""\n        pass\n```\n\n### Fix DCO032\n\nThis linting rule is triggered by a function/ method that returns a value and\nhas a docstring that has multiple returns sections. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Returns:\n        bar.\n\n    Returns:\n        bar.\n    """\n    return "bar"\n\ndef foo():\n    """Perform foo action.\n\n    Returns:\n        bar.\n\n    Return:\n        bar.\n    """\n    return "bar"\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Returns:\n            bar.\n\n        Returns:\n            bar.\n        """\n        return "bar"\n```\n\nThese examples can be fixed by removing the additional returns sections:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Returns:\n        bar.\n    """\n    return "bar"\n\ndef foo():\n    """Perform foo action.\n\n    Returns:\n        bar.\n    """\n    return "bar"\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Returns:\n            bar.\n        """\n        return "bar"\n```\n\n### Fix DCO040\n\nThis linting rule is triggered by a function/ method that has at least one\nyield statement with a value or a yield from statement and does not have a\nyields section in the docstring. For example:\n\n```Python\ndef foo():\n    """Yield bar."""\n    yield "bar"\n\ndef foo():\n    """Yield bar."""\n    yield from ("bar",)\n\nclass FooClass:\n    def foo(self):\n        """Yield bar."""\n        yield "bar"\n```\n\nThese examples can be fixed by adding the yields section:\n\n```Python\ndef foo():\n    """Yield bar.\n\n    Yield:\n        bar.\n    """\n    yield "bar"\n\ndef foo():\n    """Yield bar.\n\n    Yields:\n        bar.\n    """\n    yield "bar"\n\ndef foo():\n    """Yield bar.\n\n    Yields:\n        bar.\n    """\n    yield from ("bar",)\n\nclass FooClass:\n    def foo(self):\n        """Yield bar.\n\n        Yields:\n            bar.\n        """\n        yield "bar"\n```\n\n### Fix DCO041\n\nThis linting rule is triggered by a function/ method that has no yield\nstatement with a value nor a yield from statement and has a yields section\nin the docstring. For example:\n\n```Python\ndef foo():\n    """Yield bar.\n\n    Yields:\n        bar.\n    """\n    pass\n\nclass FooClass:\n    def foo(self):\n        """Yield bar.\n\n        Yields:\n            bar.\n        """\n        pass\n```\n\nThese examples can be fixed by:\n\n```Python\ndef foo():\n    """Take foo action."""\n    pass\n\nclass FooClass:\n    def foo(self):\n        """Take foo action."""\n        pass\n```\n\n### Fix DCO042\n\nThis linting rule is triggered by a function/ method that yields a value and\nhas a docstring that has multiple yields sections. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n\n    Yields:\n        bar.\n    """\n    yield "bar"\n\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n\n    Yields:\n        bar.\n    """\n    yield from ("bar",)\n\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n\n    Yield:\n        bar.\n    """\n    yield "bar"\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Yields:\n            bar.\n\n        Yields:\n            bar.\n        """\n        yield "bar"\n```\n\nThese examples can be fixed by removing the additional yields sections:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n    """\n    yield "bar"\n\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n    """\n    yield from ("bar",)\n\ndef foo():\n    """Perform foo action.\n\n    Yields:\n        bar.\n    """\n    yield "bar"\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Yields:\n            bar.\n        """\n        yield "bar"\n```\n\n### Fix DCO050\n\nThis linting rule is triggered by a function/ method that raises one or more\nexceptions and a docstring that does not have a raises section. For example:\n\n```Python\ndef foo():\n    """Perform foo action."""\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n        raise BarError\n```\n\nThese examples can be fixed by adding the raises section and describing all\nraised exceptions in it:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\ndef foo():\n    """Perform foo action.\n\n    Raise:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\n### Fix DCO051\n\nThis linting rule is triggered by a function/ method that raises no exceptions\nwith a docstring that has a raises section. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n\ndef foo():\n    """Perform foo action.\n\n    Raise:\n        BarError: the value to perform the foo action on was wrong.\n    """\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n```\n\nThese examples can be fixed by removing the raises section:\n\n```Python\ndef foo():\n    """Perform foo action."""\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n```\n\n### Fix DCO052\n\nThis linting rule is triggered by a function/ method that raises one or more\nexceptions with a docstring that has multiple raises sections. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n\n    Raise:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\nThese examples can be fixed by removing the additional raises sections:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\ndef foo():\n    """Perform foo action.\n\n    Raise:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\n### Fix DCO053\n\nThis linting rule is triggered by a function/ method that raises one or more\nexceptions where one or more of those exceptions is not described in the\ndocstring. For example:\n\n```Python\ndef foo():\n    """Perform foo action."""\n    raise BarError\n\ndef foo(bar, baz):\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n    raise BazError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n        raise BarError\n```\n\nThese examples can be fixed by describing the additional exceptions in the\ndocstring:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\ndef foo(bar, baz):\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n        BazError: the alternate value to perform the foo action on was wrong.\n    """\n    raise BarError\n    raise BazError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\n### Fix DCO054\n\nThis linting rule is triggered by a function/ method that raises one or more\nexceptions and a docstring that describes one or more exceptions where on or\nmore of the described exceptions are not raised by the function/ method. For\nexample:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n        BazError: the alternate value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n            BazError: the alternate value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\nThese examples can be fixed by removing the exception that is not raised from\nthe docstring:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\n### Fix DCO055\n\nThis linting rule is triggered by a function/ method that has a `raise`\nstatement without an exception (typically re-raising exceptions) and the raises\nsection is not included or is empty. For example:\n\n```Python\ndef foo():\n    """Perform foo action."""\n    try:\n        bar()\n    except BarError:\n        raise\n\ndef foo():\n    """Perform foo action.\n\n    Raises:\n    """\n    try:\n        bar()\n    except BarError:\n        raise\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action."""\n        try:\n            bar()\n        except BarError:\n            raise\n```\n\nThese examples can be fixed by describing at least one exception in the raises\nsection:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    try:\n        bar()\n    except BarError:\n        raise\n\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    try:\n        bar()\n    except BarError:\n        raise\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        try:\n            bar()\n        except BarError:\n            raise\n```\n\n### Fix DCO056\n\nThis linting rule is triggered by a function/ method that raises one or more\nexceptions and a docstring that describes one or more exceptions where on or\nmore of the described exceptions are described multiple times. For example:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\nThese examples can be fixed by removing the duplicate descriptions from the\ndocstring:\n\n```Python\ndef foo():\n    """Perform foo action.\n\n    Raises:\n        BarError: the value to perform the foo action on was wrong.\n    """\n    raise BarError\n\nclass FooClass:\n    def foo(self):\n        """Perform foo action.\n\n        Raises:\n            BarError: the value to perform the foo action on was wrong.\n        """\n        raise BarError\n```\n\n### Fix DCO060\n\nThis linting rule is triggered by a class that has one or more public\nattributes with a docstring that does not have an attributes section. For\nexample:\n\n```Python\nclass FooClass:\n    """Perform foo action."""\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action."""\n\n    def __init__(self):\n        self.bar = "bar"\n\nclass FooClass:\n    """Perform foo action."""\n\n    def bar(self):\n        self.baz = "baz"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n    baz = "baz"\n```\n\nThese examples can be fixed by adding the attributes section and describing all\nattributes in the attributes section:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n\n    def __init__(self):\n        self.bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        baz: The value to perform the foo action on.\n    """\n\n    def bar(self):\n        self.baz = "baz"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n        baz: The alternate value to perform the foo action on.\n    """\n    bar = "bar"\n    baz = "baz"\n```\n\n### Fix DCO061\n\nThis linting rule is triggered by a class that has no attributes with a\ndocstring that has an attributes section. For example:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n    """\n\n    def __init__(self):\n        self._bar = "bar"\n```\n\nThese examples can be fixed by removing the attributes section:\n\n```Python\nclass FooClass:\n    """Perform foo action."""\n\nclass FooClass:\n    """Perform foo action."""\n\n    def __init__(self):\n        self._bar = "bar"\n```\n\n### Fix DCO062\n\nThis linting rule is triggered by a class that has one or more attributes and\na docstring that has multiple attributes sections. For example:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n```\n\nThese examples can be fixed by removing the additional attributes sections:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n```\n\n### Fix DCO063\n\nThis linting rule is triggered by a class that has one or more public\nattributes where one or more of those public attributes is not described in the\ndocstring. For example:\n\n```Python\nclass FooClass:\n    """Perform foo action."""\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n    """\n\n    @property\n    def bar(self):\n        return "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n    baz = "baz"\n```\n\nThese examples can be fixed by adding the missing attributes to the attributes\nsection:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attributes:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\n    @property\n    def bar(self):\n        return "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n        baz: The alternate value to perform the foo action on.\n    """\n    bar = "bar"\n    baz = "baz"\n```\n\n### Fix DCO064\n\nThis linting rule is triggered by a class that has one or more attributes and a\ndocstring that describes one or more attributes where on or more\nof the described attributes are not attributes of the class. For example:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        _bar: The value to perform the foo action on.\n    """\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n        baz: The alternate value to perform the foo action on.\n    """\n    bar = "bar"\n```\n\nThese examples can be fixed by removing the attributes the class doesn\'t have\nfrom the docstring:\n\n```Python\nclass FooClass:\n    """Perform foo action."""\n\nclass FooClass:\n    """Perform foo action."""\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\n    def __init__(self):\n        """Construct."""\n        self.bar = "bar"\n```\n\n### Fix DCO065\n\nThis linting rule is triggered by a class that has one or more attributes and a\ndocstring that describes one or more attributes where on or more\nof the described attributes are described multiple times. For example:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n        bar: The value to perform the foo action on.\n    """\n\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n        bar: The value to perform the foo action on.\n    """\n\n    def __init__(self):\n        """Construct."""\n        self.bar = "bar"\n```\n\nThese examples can be fixed by removing the duplicate descriptions from the\ndocstring:\n\n```Python\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\n    bar = "bar"\n\nclass FooClass:\n    """Perform foo action.\n\n    Attrs:\n        bar: The value to perform the foo action on.\n    """\n\n    def __init__(self):\n        """Construct."""\n        self.bar = "bar"\n```\n\n## Docstring Examples\n\nExamples of function/ method and class docstrings are:\n\n```Python\ndef foo(bar):\n    """Perform the foo actions on bar.\n\n    Args:\n        bar: the value to perform the foo actions on.\n\n    Returns:\n        bar after applying to foo action to it.\n\n    Yields:\n        All the foo actions that have been performed.\n\n    Raises:\n        FooError: an error occurred whilst performing the foo action.\n    """\n\nclass Foo:\n    """Foo object.\n\n    Attrs:\n        bar: the value to perform the foo actions on.\n    """\n\n    def __init__(self, bar):\n        """Construct.\n\n        Args:\n            bar: the value to perform the foo actions on.\n        """\n        self.bar = bar\n```\n\n## Sections\n\nThere are several alternative names for each of the sections which are captured\ncase-insensitive:\n\n- arguments: `Args`, `Arguments`, `Parameters`\n- return value: `Return`, `Returns`\n- yield value: `Yield`, `Yields`\n- raise: `Raises`\n- attributes: `Attrs`, `Attributes`\n\nSection information is extracted using the following algorithm:\n\n1. Look for a line that has zero or more whitespace characters, followed by a\n   section name (non-case-sensistive) followed by a colon.\n2. Look for any sub-sections on a line which starts with zero or more\n   whitespace characters followed by a word, optionally followed by whitespace\n   and any characters within round brackets followed by a colon.\n3. The section ends if any line with zero or more whitespace characters is\n   encountered or the end of the docstring is reached.\n\n## Future Ideas:\n\n- Check that argument, exceptions and attributes have non-empty description.\n- Check that arguments, exceptions and attributes are only documented once.\n- Check that arguments, exceptions and attributes have meaningful descriptions.\n- Check other other PEP257 conventions\n',
-    'author': 'David Andersson',
-    'author_email': 'david@jdkandersson.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+## Getting Started
 
+```shell
+python -m venv venv
+source ./venv/bin/activate
+pip install flake8 flake8-docstrings flake8-docstrings-complete
+flake8 source.py
+```
+
+On the following code where the `foo` function has the `bar` and `baz`
+arguments where the `baz` argument is missing from the `Args` section in the
+docstring:
+
+```Python
+# source.py
+def foo(bar, baz):
+    """Perform foo action on bar.
+
+    Args:
+        bar: The value to perform the foo action on.
+    """
+```
+
+This will produce warnings such as:
+
+```shell
+flake8 test_source.py
+source.py:2:14: DCO023 "baz" argument should be described in the docstring, more information: https://github.com/jdkandersson/flake8-docstrings-complete#fix-dco023
+```
+
+This can be resolved by adding the `baz` argument to the `Args` section:
+
+```Python
+# source.py
+def foo(bar, baz):
+    """Perform foo action on bar.
+
+    Args:
+        bar: The value to perform the foo action on.
+        baz: The modifier to the foo action.
+    """
+```
+
+`flake8-docstrings-complete` adds the following checks to complement
+`pydocstyle`:
+
+1. If a function/ method has arguments, that the arguments section is included.
+2. If a function/ method has arguments, that all function/ method arguments are
+   in the argument section.
+3. If an arguments section is in the function/ method docstring, the argument
+   section contains no arguments the function/ method doesn't have.
+4. Function/ method arguments are only documented once.
+5. If a function/ method has a return statement with a value, the return value
+   section is included.
+6. If a function/ method has a yield statement with a value, the yield value
+   section is included.
+7. If a function/ method raises an exception, the raises section is included
+   with a description for each exception that is raised.
+8. Each raised exception is only described once.
+9. If a class has public attributes, that the attributes section is included.
+10. If a class has public attributes, that all public attributes are in the
+   attributes section.
+11. If an attributes section is in the class docstring, the attributes section
+   contains no attributes the class doesn't have.
+12. Class attributes are only documented once.
+13. Any of the sections being checked are not present multiple times.
+
+Note:
+
+- `self` and `cls` are not counted as arguments.
+- `test_.*` methods are skipped in `test_.*\.py` files (function and file names
+  are configurable).
+- functions with a `@fixture` et al dectorator in `conftest.py` and
+  `test_.*\.py` files are skipped (function and fixture file names are
+  configurable)
+
+## Configuration
+
+The plugin adds the following configurations to `flake8`:
+
+- `--docstrings-complete-test-filename-pattern`: The filename pattern for test
+  files. Defaults to `test_.*\.py`.
+- `--docstrings-complete-test-function-pattern`: The function name pattern for
+  test functions. Defaults to `test_.*`.
+- `--docstrings-complete-fixture-filename-pattern`: The filename pattern for
+  fixture files. Defaults to `conftest\.py`.
+- `--docstrings-complete-fixture-decorator-pattern`: The decorator name pattern
+  for fixture functions. Defaults to `(^|\.)fixture$`.
+
+## Rules
+
+A few rules have been defined to allow for selective suppression:
+
+- `DCO010`: docstring missing on a function/ method/ class.
+- `DCO020`: function/ method has one or more arguments and the docstring does
+  not have an arguments section.
+- `DCO021`: function/ method with no arguments and the docstring has an
+  arguments section.
+- `DCO022`: function/ method with one or more arguments and the docstring has
+  multiple arguments sections.
+- `DCO023`: function/ method has one or more arguments not described in the
+  docstring.
+- `DCO024`: function/ method has one or more arguments described in the
+  docstring which are not arguments of the function/ method.
+- `DCO025`: function/ method has one or more arguments described in the
+  docstring multiple times.
+- `DCO030`: function/ method that returns a value does not have the returns
+  section in the docstring.
+- `DCO031`: function/ method that does not return a value has the returns
+  section in the docstring.
+- `DCO032`: function/ method that returns a value and the docstring has
+  multiple returns sections.
+- `DCO040`: function/ method that yields a value does not have the yields
+  section in the docstring.
+- `DCO041`: function/ method that does not yield a value has the yields
+  section in the docstring.
+- `DCO042`: function/ method that yields a value and the docstring has
+  multiple yields sections.
+- `DCO050`: function/ method raises one or more exceptions and the docstring
+  does not have a raises section.
+- `DCO051`: function/ method that raises no exceptions and the docstring has a
+  raises section.
+- `DCO052`: function/ method that raises one or more exceptions and the
+  docstring has multiple raises sections.
+- `DCO053`: function/ method that raises one or more exceptions where one or
+  more of the exceptions is not described in the docstring.
+- `DCO054`: function/ method has one or more exceptions described in the
+  docstring which are not raised in the function/ method.
+- `DCO055`: function/ method that has a raise without an exception has an empty
+  raises section in the docstring.
+- `DCO056`: function/ method has one or more exceptions described in the
+  docstring multiple times.
+- `DCO060`: class has one or more public attributes and the docstring does not
+  have an attributes section.
+- `DCO061`: class with no attributes and the docstring has an attributes
+  section.
+- `DCO062`: class with one or more attributes and the docstring has multiple
+  attributes sections.
+- `DCO063`: class has one or more public attributes not described in the
+  docstring.
+- `DCO064`: class has one or more attributes described in the docstring which
+  are not attributes of the class.
+- `DCO065`: class has one or more attributes described in the docstring
+  multiple times.
+
+### Fix DCO010
+
+This linting rule is triggered by a function/ method/ class without a
+docstring. For example:
+
+```Python
+def foo():
+    pass
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+        pass
+
+class FooClass:
+    """Perform foo action."""
+    def foo(self):
+        pass
+```
+
+This example can be fixed by adding a docstring:
+
+```Python
+def foo():
+    """Perform foo action."""
+
+class FooClass:
+    """Perform foo action."""
+    def foo(self):
+        """Perform foo action."""
+```
+
+### Fix DCO020
+
+This linting rule is triggered by a function/ method that has one or more
+arguments with a docstring that does not have an arguments section. For
+example:
+
+```Python
+def foo(bar):
+    """Perform foo action."""
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action."""
+```
+
+These examples can be fixed by adding the arguments section and describing all
+arguments in the arguments section:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar):
+    """Perform foo action.
+
+    Arguments:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar):
+    """Perform foo action.
+
+    Parameters:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+### Fix DCO021
+
+This linting rule is triggered by a function/ method that has no arguments with
+a docstring that has an arguments section. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+def foo():
+    """Perform foo action.
+
+    Arguments:
+        bar: the value to perform the foo action on.
+    """
+
+def foo():
+    """Perform foo action.
+
+    Parameters:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+These examples can be fixed by removing the arguments section:
+
+```Python
+def foo():
+    """Perform foo action."""
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+```
+
+### Fix DCO022
+
+This linting rule is triggered by a function/ method that has one or more
+arguments and a docstring that has multiple arguments sections. For example:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+
+    Arguments:
+        bar: the value to perform the foo action on.
+
+    Parameters:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+These examples can be fixed by removing the additional arguments sections:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar):
+    """Perform foo action.
+
+    Arguments:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar):
+    """Perform foo action.
+
+    Parameters:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+### Fix DCO023
+
+This linting rule is triggered by a function/ method that has one or more
+arguments where one or more of those arguments is not described in the
+docstring. For example:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+    """
+
+def foo(bar, baz):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+        """
+```
+
+These examples can be fixed by adding the missing arguments to the arguments
+section:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+def foo(bar, baz):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+        baz: the modifier to the foo action.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+### Fix DCO024
+
+This linting rule is triggered by a function/ method that has one or more
+arguments and a docstring that describes one or more arguments where on or more
+of the described arguments are not arguments of the function/ method. For
+example:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+        baz: the modifier to the foo action.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+            baz: the modifier to the foo action.
+        """
+```
+
+These examples can be fixed by removing the arguments the function/ method
+doesn't have from the docstring:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+### Fix DCO025
+
+This linting rule is triggered by a function/ method that has one or more
+arguments and a docstring that describes one or more arguments where on or more
+of the described arguments are described multiple times. For example:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+            bar: the value to perform the foo action on.
+        """
+```
+
+These examples can be fixed by removing the duplicate arguments from the docstring:
+
+```Python
+def foo(bar):
+    """Perform foo action.
+
+    Args:
+        bar: the value to perform the foo action on.
+    """
+
+class FooClass:
+    def foo(self, bar):
+        """Perform foo action.
+
+        Args:
+            bar: the value to perform the foo action on.
+        """
+```
+
+### Fix DCO030
+
+This linting rule is triggered by a function/ method that has at least one
+return statement with a value and does not have a returns section in the
+docstring. For example:
+
+```Python
+def foo():
+    """Return bar."""
+    return "bar"
+
+class FooClass:
+    def foo(self):
+        """Return bar."""
+        return "bar"
+```
+
+These examples can be fixed by adding the returns section:
+
+```Python
+def foo():
+    """Return bar.
+
+    Return:
+        bar.
+    """
+    return "bar"
+
+def foo():
+    """Return bar.
+
+    Returns:
+        bar.
+    """
+    return "bar"
+
+class FooClass:
+    def foo(self):
+        """Return bar.
+
+        Returns:
+            bar.
+        """
+        return "bar"
+```
+
+### Fix DCO031
+
+This linting rule is triggered by a function/ method that has no return
+statement with a value and has a returns section in the
+docstring. For example:
+
+```Python
+def foo():
+    """Return bar.
+
+    Returns:
+        bar.
+    """
+    pass
+
+class FooClass:
+    def foo(self):
+        """Return bar.
+
+        Returns:
+            bar.
+        """
+        pass
+```
+
+These examples can be fixed by removing the returns section:
+
+```Python
+def foo():
+    """Take foo action."""
+    pass
+
+class FooClass:
+    def foo(self):
+        """Take foo action."""
+        pass
+```
+
+### Fix DCO032
+
+This linting rule is triggered by a function/ method that returns a value and
+has a docstring that has multiple returns sections. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Returns:
+        bar.
+
+    Returns:
+        bar.
+    """
+    return "bar"
+
+def foo():
+    """Perform foo action.
+
+    Returns:
+        bar.
+
+    Return:
+        bar.
+    """
+    return "bar"
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Returns:
+            bar.
+
+        Returns:
+            bar.
+        """
+        return "bar"
+```
+
+These examples can be fixed by removing the additional returns sections:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Returns:
+        bar.
+    """
+    return "bar"
+
+def foo():
+    """Perform foo action.
+
+    Returns:
+        bar.
+    """
+    return "bar"
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Returns:
+            bar.
+        """
+        return "bar"
+```
+
+### Fix DCO040
+
+This linting rule is triggered by a function/ method that has at least one
+yield statement with a value or a yield from statement and does not have a
+yields section in the docstring. For example:
+
+```Python
+def foo():
+    """Yield bar."""
+    yield "bar"
+
+def foo():
+    """Yield bar."""
+    yield from ("bar",)
+
+class FooClass:
+    def foo(self):
+        """Yield bar."""
+        yield "bar"
+```
+
+These examples can be fixed by adding the yields section:
+
+```Python
+def foo():
+    """Yield bar.
+
+    Yield:
+        bar.
+    """
+    yield "bar"
+
+def foo():
+    """Yield bar.
+
+    Yields:
+        bar.
+    """
+    yield "bar"
+
+def foo():
+    """Yield bar.
+
+    Yields:
+        bar.
+    """
+    yield from ("bar",)
+
+class FooClass:
+    def foo(self):
+        """Yield bar.
+
+        Yields:
+            bar.
+        """
+        yield "bar"
+```
+
+### Fix DCO041
+
+This linting rule is triggered by a function/ method that has no yield
+statement with a value nor a yield from statement and has a yields section
+in the docstring. For example:
+
+```Python
+def foo():
+    """Yield bar.
+
+    Yields:
+        bar.
+    """
+    pass
+
+class FooClass:
+    def foo(self):
+        """Yield bar.
+
+        Yields:
+            bar.
+        """
+        pass
+```
+
+These examples can be fixed by:
+
+```Python
+def foo():
+    """Take foo action."""
+    pass
+
+class FooClass:
+    def foo(self):
+        """Take foo action."""
+        pass
+```
+
+### Fix DCO042
+
+This linting rule is triggered by a function/ method that yields a value and
+has a docstring that has multiple yields sections. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+
+    Yields:
+        bar.
+    """
+    yield "bar"
+
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+
+    Yields:
+        bar.
+    """
+    yield from ("bar",)
+
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+
+    Yield:
+        bar.
+    """
+    yield "bar"
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Yields:
+            bar.
+
+        Yields:
+            bar.
+        """
+        yield "bar"
+```
+
+These examples can be fixed by removing the additional yields sections:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+    """
+    yield "bar"
+
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+    """
+    yield from ("bar",)
+
+def foo():
+    """Perform foo action.
+
+    Yields:
+        bar.
+    """
+    yield "bar"
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Yields:
+            bar.
+        """
+        yield "bar"
+```
+
+### Fix DCO050
+
+This linting rule is triggered by a function/ method that raises one or more
+exceptions and a docstring that does not have a raises section. For example:
+
+```Python
+def foo():
+    """Perform foo action."""
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+        raise BarError
+```
+
+These examples can be fixed by adding the raises section and describing all
+raised exceptions in it:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+def foo():
+    """Perform foo action.
+
+    Raise:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+### Fix DCO051
+
+This linting rule is triggered by a function/ method that raises no exceptions
+with a docstring that has a raises section. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+
+def foo():
+    """Perform foo action.
+
+    Raise:
+        BarError: the value to perform the foo action on was wrong.
+    """
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+```
+
+These examples can be fixed by removing the raises section:
+
+```Python
+def foo():
+    """Perform foo action."""
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+```
+
+### Fix DCO052
+
+This linting rule is triggered by a function/ method that raises one or more
+exceptions with a docstring that has multiple raises sections. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+
+    Raise:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+These examples can be fixed by removing the additional raises sections:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+def foo():
+    """Perform foo action.
+
+    Raise:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+### Fix DCO053
+
+This linting rule is triggered by a function/ method that raises one or more
+exceptions where one or more of those exceptions is not described in the
+docstring. For example:
+
+```Python
+def foo():
+    """Perform foo action."""
+    raise BarError
+
+def foo(bar, baz):
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+    raise BazError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+        raise BarError
+```
+
+These examples can be fixed by describing the additional exceptions in the
+docstring:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+def foo(bar, baz):
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+        BazError: the alternate value to perform the foo action on was wrong.
+    """
+    raise BarError
+    raise BazError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+### Fix DCO054
+
+This linting rule is triggered by a function/ method that raises one or more
+exceptions and a docstring that describes one or more exceptions where on or
+more of the described exceptions are not raised by the function/ method. For
+example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+        BazError: the alternate value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+            BazError: the alternate value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+These examples can be fixed by removing the exception that is not raised from
+the docstring:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+### Fix DCO055
+
+This linting rule is triggered by a function/ method that has a `raise`
+statement without an exception (typically re-raising exceptions) and the raises
+section is not included or is empty. For example:
+
+```Python
+def foo():
+    """Perform foo action."""
+    try:
+        bar()
+    except BarError:
+        raise
+
+def foo():
+    """Perform foo action.
+
+    Raises:
+    """
+    try:
+        bar()
+    except BarError:
+        raise
+
+class FooClass:
+    def foo(self):
+        """Perform foo action."""
+        try:
+            bar()
+        except BarError:
+            raise
+```
+
+These examples can be fixed by describing at least one exception in the raises
+section:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    try:
+        bar()
+    except BarError:
+        raise
+
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    try:
+        bar()
+    except BarError:
+        raise
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        try:
+            bar()
+        except BarError:
+            raise
+```
+
+### Fix DCO056
+
+This linting rule is triggered by a function/ method that raises one or more
+exceptions and a docstring that describes one or more exceptions where on or
+more of the described exceptions are described multiple times. For example:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+These examples can be fixed by removing the duplicate descriptions from the
+docstring:
+
+```Python
+def foo():
+    """Perform foo action.
+
+    Raises:
+        BarError: the value to perform the foo action on was wrong.
+    """
+    raise BarError
+
+class FooClass:
+    def foo(self):
+        """Perform foo action.
+
+        Raises:
+            BarError: the value to perform the foo action on was wrong.
+        """
+        raise BarError
+```
+
+### Fix DCO060
+
+This linting rule is triggered by a class that has one or more public
+attributes with a docstring that does not have an attributes section. For
+example:
+
+```Python
+class FooClass:
+    """Perform foo action."""
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action."""
+
+    def __init__(self):
+        self.bar = "bar"
+
+class FooClass:
+    """Perform foo action."""
+
+    def bar(self):
+        self.baz = "baz"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+    baz = "baz"
+```
+
+These examples can be fixed by adding the attributes section and describing all
+attributes in the attributes section:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+
+    def __init__(self):
+        self.bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        baz: The value to perform the foo action on.
+    """
+
+    def bar(self):
+        self.baz = "baz"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+        baz: The alternate value to perform the foo action on.
+    """
+    bar = "bar"
+    baz = "baz"
+```
+
+### Fix DCO061
+
+This linting rule is triggered by a class that has no attributes with a
+docstring that has an attributes section. For example:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+    """
+
+    def __init__(self):
+        self._bar = "bar"
+```
+
+These examples can be fixed by removing the attributes section:
+
+```Python
+class FooClass:
+    """Perform foo action."""
+
+class FooClass:
+    """Perform foo action."""
+
+    def __init__(self):
+        self._bar = "bar"
+```
+
+### Fix DCO062
+
+This linting rule is triggered by a class that has one or more attributes and
+a docstring that has multiple attributes sections. For example:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+```
+
+These examples can be fixed by removing the additional attributes sections:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+```
+
+### Fix DCO063
+
+This linting rule is triggered by a class that has one or more public
+attributes where one or more of those public attributes is not described in the
+docstring. For example:
+
+```Python
+class FooClass:
+    """Perform foo action."""
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+    """
+
+    @property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+    """
+
+    @functools.cached_property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+    baz = "baz"
+```
+
+These examples can be fixed by adding the missing attributes to the attributes
+section:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attributes:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+    @property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+    @functools.cached_property
+    def bar(self):
+        return "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+        baz: The alternate value to perform the foo action on.
+    """
+    bar = "bar"
+    baz = "baz"
+```
+
+### Fix DCO064
+
+This linting rule is triggered by a class that has one or more attributes and a
+docstring that describes one or more attributes where on or more
+of the described attributes are not attributes of the class. For example:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        _bar: The value to perform the foo action on.
+    """
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+        baz: The alternate value to perform the foo action on.
+    """
+    bar = "bar"
+```
+
+These examples can be fixed by removing the attributes the class doesn't have
+from the docstring:
+
+```Python
+class FooClass:
+    """Perform foo action."""
+
+class FooClass:
+    """Perform foo action."""
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+    def __init__(self):
+        """Construct."""
+        self.bar = "bar"
+```
+
+### Fix DCO065
+
+This linting rule is triggered by a class that has one or more attributes and a
+docstring that describes one or more attributes where on or more
+of the described attributes are described multiple times. For example:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+        bar: The value to perform the foo action on.
+    """
+
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+        bar: The value to perform the foo action on.
+    """
+
+    def __init__(self):
+        """Construct."""
+        self.bar = "bar"
+```
+
+These examples can be fixed by removing the duplicate descriptions from the
+docstring:
+
+```Python
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+    bar = "bar"
+
+class FooClass:
+    """Perform foo action.
+
+    Attrs:
+        bar: The value to perform the foo action on.
+    """
+
+    def __init__(self):
+        """Construct."""
+        self.bar = "bar"
+```
+
+## Docstring Examples
+
+Examples of function/ method and class docstrings are:
+
+```Python
+def foo(bar):
+    """Perform the foo actions on bar.
+
+    Args:
+        bar: the value to perform the foo actions on.
+
+    Returns:
+        bar after applying to foo action to it.
+
+    Yields:
+        All the foo actions that have been performed.
+
+    Raises:
+        FooError: an error occurred whilst performing the foo action.
+    """
+
+class Foo:
+    """Foo object.
+
+    Attrs:
+        bar: the value to perform the foo actions on.
+    """
+
+    def __init__(self, bar):
+        """Construct.
+
+        Args:
+            bar: the value to perform the foo actions on.
+        """
+        self.bar = bar
+```
+
+## Sections
+
+There are several alternative names for each of the sections which are captured
+case-insensitive:
+
+- arguments: `Args`, `Arguments`, `Parameters`
+- return value: `Return`, `Returns`
+- yield value: `Yield`, `Yields`
+- raise: `Raises`
+- attributes: `Attrs`, `Attributes`
+
+Section information is extracted using the following algorithm:
+
+1. Look for a line that has zero or more whitespace characters, followed by a
+   section name (non-case-sensistive) followed by a colon.
+2. Look for any sub-sections on a line which starts with zero or more
+   whitespace characters followed by a word, optionally followed by whitespace
+   and any characters within round brackets followed by a colon.
+3. The section ends if any line with zero or more whitespace characters is
+   encountered or the end of the docstring is reached.
+
+## Future Ideas:
+
+- Check that argument, exceptions and attributes have non-empty description.
+- Check that arguments, exceptions and attributes have meaningful descriptions.
+- Check other other PEP257 conventions
 
-setup(**setup_kwargs)
```

