# Comparing `tmp/jinja2_jsonschema-0.2.0.tar.gz` & `tmp/jinja2_jsonschema-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_jsonschema-0.2.0.tar", max compression
+gzip compressed data, was "jinja2_jsonschema-0.2.1.tar", max compression
```

## Comparing `jinja2_jsonschema-0.2.0.tar` & `jinja2_jsonschema-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/LICENSE
--rw-r--r--   0        0        0     7095 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/README.md
--rw-r--r--   0        0        0     2313 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/__init__.py
--rw-r--r--   0        0        0      657 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/errors.py
--rw-r--r--   0        0        0     4617 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/extension.py
--rw-r--r--   0        0        0        0 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/py.typed
--rw-r--r--   0        0        0     8222 1970-01-01 00:00:00.000000 jinja2_jsonschema-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7351 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/README.md
+-rw-r--r--   0        0        0     2313 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/__init__.py
+-rw-r--r--   0        0        0      657 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/errors.py
+-rw-r--r--   0        0        0     4617 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/extension.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:49:44.488361 jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/py.typed
+-rw-r--r--   0        0        0     8546 1970-01-01 00:00:00.000000 jinja2_jsonschema-0.2.1/PKG-INFO
```

### Comparing `jinja2_jsonschema-0.2.0/LICENSE` & `jinja2_jsonschema-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_jsonschema-0.2.0/README.md` & `jinja2_jsonschema-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # JSON Schema Validation within Jinja2 Templates
 
-[![CI](https://github.com/copier-org/jinja2-jsonschema/workflows/tests/badge.svg)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
-![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?logo=python&logoColor=%23959DA5)
-[![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/jinja2-jsonschema)
-[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64)](https://github.com/charliermarsh/ruff)
-[![Type-checker: mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
+[![Tests](https://img.shields.io/github/actions/workflow/status/copier-org/jinja2-jsonschema/tests.yml?branch=main&label=Tests&labelColor=333&logo=github&style=flat-square)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
+[![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?label=Python&logo=python&logoColor=%23959DA5&style=flat-square)](https://pypi.org/project/jinja2-jsonschema)
+[![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?label=PyPI&logo=pypi&logoColor=%23959DA5&style=flat-square)](https://pypi.org/project/jinja2-jsonschema)
+[![Code style: Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg?style=flat-square)](https://github.com/psf/black)
+[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64&style=flat-square)](https://github.com/charliermarsh/ruff)
+[![Type-checker: mypy](https://img.shields.io/badge/mypy-strict-2A6DB2.svg?style=flat-square)](http://mypy-lang.org)
 
 A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] and a [Jinja2 test][jinja-test] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
 
 ## Installation
 
 * With [`pip`](https://pip.pypa.io):
```

### Comparing `jinja2_jsonschema-0.2.0/pyproject.toml` & `jinja2_jsonschema-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinja2-jsonschema"
-version = "0.2.0"
+version = "0.2.1"
 description = "JSON/YAML schema validation within Jinja2 templates"
 license = "MIT"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -24,14 +24,15 @@
 repository = "https://github.com/copier-org/jinja2-jsonschema"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2"
 jinja2 = ">=3.0.0"
 jsonschema = ">=4.0.0"
 pyyaml = { version = ">=6.0.0", optional = true }
+typing-extensions = { version = ">=3.7.4", python = "<3.8" }
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
 isort = ">=5.11.3"
@@ -44,15 +45,14 @@
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.3.1"
 pytest-cov = ">=4.0.0"
 
 [tool.poetry.group.typing.dependencies]
 types-jsonschema = ">=4.0.0"
 types-pyyaml = ">=6.0.12.10"
-typing-extensions = { version = ">=3.7.4", python = "<3.8" }
 
 [tool.black]
 target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
 force_single_line = true
```

### Comparing `jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/errors.py` & `jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/errors.py`

 * *Files identical despite different names*

### Comparing `jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/extension.py` & `jinja2_jsonschema-0.2.1/src/jinja2_jsonschema/extension.py`

 * *Files identical despite different names*

### Comparing `jinja2_jsonschema-0.2.0/PKG-INFO` & `jinja2_jsonschema-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-jsonschema
-Version: 0.2.0
+Version: 0.2.1
 Summary: JSON/YAML schema validation within Jinja2 templates
 Home-page: https://github.com/copier-org/jinja2-jsonschema
 License: MIT
 Keywords: jinja,jinja2,extension,jsonschema,json,yaml
 Author: Sigurd Spieckermann
 Author-email: sigurd.spieckermann@gmail.com
 Requires-Python: >=3.7.2
@@ -19,25 +19,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: yaml
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: jsonschema (>=4.0.0)
 Requires-Dist: pyyaml (>=6.0.0) ; extra == "yaml"
+Requires-Dist: typing-extensions (>=3.7.4) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/copier-org/jinja2-jsonschema
 Description-Content-Type: text/markdown
 
 # JSON Schema Validation within Jinja2 Templates
 
-[![CI](https://github.com/copier-org/jinja2-jsonschema/workflows/tests/badge.svg)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
-![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?logo=python&logoColor=%23959DA5)
-[![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/jinja2-jsonschema)
-[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64)](https://github.com/charliermarsh/ruff)
-[![Type-checker: mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
+[![Tests](https://img.shields.io/github/actions/workflow/status/copier-org/jinja2-jsonschema/tests.yml?branch=main&label=Tests&labelColor=333&logo=github&style=flat-square)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
+[![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?label=Python&logo=python&logoColor=%23959DA5&style=flat-square)](https://pypi.org/project/jinja2-jsonschema)
+[![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?label=PyPI&logo=pypi&logoColor=%23959DA5&style=flat-square)](https://pypi.org/project/jinja2-jsonschema)
+[![Code style: Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg?style=flat-square)](https://github.com/psf/black)
+[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64&style=flat-square)](https://github.com/charliermarsh/ruff)
+[![Type-checker: mypy](https://img.shields.io/badge/mypy-strict-2A6DB2.svg?style=flat-square)](http://mypy-lang.org)
 
 A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] and a [Jinja2 test][jinja-test] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
 
 ## Installation
 
 * With [`pip`](https://pip.pypa.io):
```

