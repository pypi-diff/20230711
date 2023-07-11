# Comparing `tmp/brussel-0.2.1.tar.gz` & `tmp/brussel-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brussel-0.2.1.tar", max compression
+gzip compressed data, was "brussel-0.2.2.tar", max compression
```

## Comparing `brussel-0.2.1.tar` & `brussel-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-31 12:32:48.409602 brussel-0.2.1/LICENSE
--rw-r--r--   0        0        0     8307 2023-03-31 12:32:48.409602 brussel-0.2.1/README.md
--rw-r--r--   0        0        0      347 2023-03-31 12:32:48.409602 brussel-0.2.1/brussel/__init__.py
--rw-r--r--   0        0        0     4957 2023-03-31 12:32:48.409602 brussel-0.2.1/brussel/brussel.py
--rw-r--r--   0        0        0      278 2023-03-31 12:32:48.409602 brussel-0.2.1/brussel/exceptions.py
--rw-r--r--   0        0        0     2229 2023-03-31 12:32:48.409602 brussel-0.2.1/brussel/models.py
--rw-r--r--   0        0        0        0 2023-03-31 12:32:48.409602 brussel-0.2.1/brussel/py.typed
--rw-r--r--   0        0        0     3852 2023-03-31 12:33:08.501571 brussel-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 brussel-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-11 21:54:51.874832 brussel-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8631 2023-07-11 21:54:51.874832 brussel-0.2.2/README.md
+-rw-r--r--   0        0        0     3761 2023-07-11 21:55:07.746907 brussel-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-07-11 21:54:51.878832 brussel-0.2.2/src/brussel/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-11 21:54:51.878832 brussel-0.2.2/src/brussel/brussel.py
+-rw-r--r--   0        0        0      278 2023-07-11 21:54:51.878832 brussel-0.2.2/src/brussel/exceptions.py
+-rw-r--r--   0        0        0     2229 2023-07-11 21:54:51.878832 brussel-0.2.2/src/brussel/models.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:54:51.878832 brussel-0.2.2/src/brussel/py.typed
+-rw-r--r--   0        0        0     9967 1970-01-01 00:00:00.000000 brussel-0.2.2/PKG-INFO
```

### Comparing `brussel-0.2.1/LICENSE` & `brussel-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brussel-0.2.1/README.md` & `brussel-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
 [![PyPi Downloads][downloads-shield]][downloads-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 [![Maintainability][maintainability-shield]][maintainability-url]
 [![Code Coverage][codecov-shield]][codecov-url]
@@ -112,16 +111,22 @@
 We've set up a separate document for our
 [contribution guidelines](CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up development environment
 
-This Python project is fully managed using the [Poetry][poetry] dependency
-manager.
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
 
 You need at least:
 
 - Python 3.9+
 - [Poetry][poetry-install]
 
 Install all packages, including all development requirements:
@@ -194,29 +199,27 @@
 [build-url]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-brussel.svg
 [commits-url]: https://github.com/klaasnicolaas/python-brussel/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-brussel/branch/main/graph/badge.svg?token=qf9A9Hlk4I
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-brussel
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-brussel
 [downloads-shield]: https://img.shields.io/pypi/dm/brussel
 [downloads-url]: https://pypistats.org/packages/brussel
-[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-brussel.svg
-[issues-url]: https://github.com/klaasnicolaas/python-brussel/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-brussel.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-brussel.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/b978435e9849ca199fc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-brussel/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/brussel/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/brussel
 [typing-shield]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/typing.yaml
 [releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-brussel.svg
 [releases]: https://github.com/klaasnicolaas/python-brussel/releases
-[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-brussel.svg
-[stars-url]: https://github.com/klaasnicolaas/python-brussel/stargazers
 
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com
```

### Comparing `brussel-0.2.1/brussel/brussel.py` & `brussel-0.2.2/src/brussel/brussel.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,44 +106,36 @@
         ----
             limit: Maximum number of disabled parkings to return.
 
         Returns:
         -------
             A list of DisabledParking objects.
         """
-        results: list[DisabledParking] = []
         locations = await self._request(
             "search/",
             params={"dataset": "parking-spaces-for-disabled", "rows": limit},
         )
-
-        for item in locations["records"]:
-            results.append(DisabledParking.from_dict(item))
-        return results
+        return [DisabledParking.from_dict(item) for item in locations["records"]]
 
     async def garages(self, limit: int = 10) -> list[Garage]:
         """Get list of parking garages.
 
         Args:
         ----
             limit: Maximum number of garages to return.
 
         Returns:
         -------
             A list of Garage objects.
         """
-        results: list[Garage] = []
         locations = await self._request(
             "search/",
             params={"dataset": "parkings", "rows": limit},
         )
-
-        for item in locations["records"]:
-            results.append(Garage.from_dict(item))
-        return results
+        return [Garage.from_dict(item) for item in locations["records"]]
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> ODPBrussel:
```

### Comparing `brussel-0.2.1/brussel/models.py` & `brussel-0.2.2/src/brussel/models.py`

 * *Files identical despite different names*

### Comparing `brussel-0.2.1/pyproject.toml` & `brussel-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,140 +1,134 @@
 [tool.poetry]
 name = "brussel"
-version = "0.2.1"
+version = "0.2.2"
 description = "Asynchronous Python client providing Open Data information of Brussel (Belgium)"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-brussel"
 repository = "https://github.com/klaasnicolaas/python-brussel"
 documentation = "https://github.com/klaasnicolaas/python-brussel"
 keywords = ["open", "data", "platform", "brussel", "parking", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "brussel" }
+  { include = "brussel", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-brussel/issues"
 Changelog = "https://github.com/klaasnicolaas/python-brussel/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.261"
-aresponses = "^2.1.6"
-black = ">=22.10,<24.0"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.4"
-coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.2"
-pre-commit = "^3.2.0"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.17.0"
-pytest = "^7.2.2"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.3.0"
-types-pytz = ">=2022.7.1.2,<2024.0.0.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["brussel"]
+ruff = "0.0.277"
+aresponses = "2.1.6"
+black = "23.7.0"
+blacken-docs = "1.15.0"
+codespell = "2.2.5"
+coverage = {version = "7.2.7", extras = ["toml"]}
+mypy = "1.4.1"
+pre-commit = "3.3.3"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.1.0"
+yamllint = "1.32.0"
+covdefaults = "2.3.0"
+types-pytz = "2023.3.0.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["brussel"]
 
+[tool.coverage.report]
+fail_under = 90
+show_missing = true
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "vw",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes=20
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 20
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -154,9 +148,9 @@
 [tool.ruff.isort]
 known-first-party = ["brussel"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `brussel-0.2.1/PKG-INFO` & `brussel-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brussel
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asynchronous Python client providing Open Data information of Brussel (Belgium)
 Home-page: https://github.com/klaasnicolaas/python-brussel
 License: MIT
 Keywords: open,data,platform,brussel,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -14,18 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-brussel/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-brussel/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-brussel
@@ -40,17 +36,16 @@
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
 [![PyPi Downloads][downloads-shield]][downloads-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 [![Maintainability][maintainability-shield]][maintainability-url]
 [![Code Coverage][codecov-shield]][codecov-url]
@@ -146,16 +141,22 @@
 We've set up a separate document for our
 [contribution guidelines](CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up development environment
 
-This Python project is fully managed using the [Poetry][poetry] dependency
-manager.
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
 
 You need at least:
 
 - Python 3.9+
 - [Poetry][poetry-install]
 
 Install all packages, including all development requirements:
@@ -228,30 +229,28 @@
 [build-url]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-brussel.svg
 [commits-url]: https://github.com/klaasnicolaas/python-brussel/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-brussel/branch/main/graph/badge.svg?token=qf9A9Hlk4I
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-brussel
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-brussel
 [downloads-shield]: https://img.shields.io/pypi/dm/brussel
 [downloads-url]: https://pypistats.org/packages/brussel
-[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-brussel.svg
-[issues-url]: https://github.com/klaasnicolaas/python-brussel/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-brussel.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-brussel.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/b978435e9849ca199fc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-brussel/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/brussel/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/brussel
 [typing-shield]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-brussel/actions/workflows/typing.yaml
 [releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-brussel.svg
 [releases]: https://github.com/klaasnicolaas/python-brussel/releases
-[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-brussel.svg
-[stars-url]: https://github.com/klaasnicolaas/python-brussel/stargazers
 
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com
```

