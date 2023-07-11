# Comparing `tmp/pwnic-0.3.0.tar.gz` & `tmp/pwnic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwnic-0.3.0.tar", max compression
+gzip compressed data, was "pwnic-0.4.0.tar", max compression
```

## Comparing `pwnic-0.3.0.tar` & `pwnic-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0    32471 2023-07-09 18:22:17.480086 pwnic-0.3.0/LICENSE
--rw-r--r--   0        0        0    12475 2023-07-09 18:22:17.481086 pwnic-0.3.0/README.md
--rw-r--r--   0        0        0      346 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/Attacker.py
--rw-r--r--   0        0        0      239 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/Submitter.py
--rw-r--r--   0        0        0      394 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/__init__.py
--rw-r--r--   0        0        0      961 2023-07-11 15:11:07.449917 pwnic-0.3.0/pwnic/api.py
--rw-r--r--   0        0        0      468 2023-07-09 18:31:09.133305 pwnic-0.3.0/pwnic/config.py
--rw-r--r--   0        0        0      110 2023-07-09 18:22:17.485086 pwnic-0.3.0/pwnic/db.py
--rw-r--r--   0        0        0     3508 2023-07-11 15:13:42.678207 pwnic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    13454 1970-01-01 00:00:00.000000 pwnic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-07-09 18:22:17.480086 pwnic-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11979 2023-07-11 15:37:58.352880 pwnic-0.4.0/README.md
+-rw-r--r--   0        0        0      346 2023-07-09 18:22:17.484086 pwnic-0.4.0/pwnic/Attacker.py
+-rw-r--r--   0        0        0      239 2023-07-09 18:22:17.484086 pwnic-0.4.0/pwnic/Submitter.py
+-rw-r--r--   0        0        0      576 2023-07-11 20:56:51.048536 pwnic-0.4.0/pwnic/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-11 20:06:54.967256 pwnic-0.4.0/pwnic/__main__.py
+-rw-r--r--   0        0        0     1735 2023-07-11 20:59:23.281843 pwnic-0.4.0/pwnic/api.py
+-rw-r--r--   0        0        0      468 2023-07-09 18:31:09.133305 pwnic-0.4.0/pwnic/config.py
+-rw-r--r--   0        0        0      110 2023-07-09 18:22:17.485086 pwnic-0.4.0/pwnic/db.py
+-rw-r--r--   0        0        0     2425 2023-07-11 20:59:06.676810 pwnic-0.4.0/pwnic/exploits.py
+-rw-r--r--   0        0        0      612 2023-07-11 20:58:46.112768 pwnic-0.4.0/pwnic/utils.py
+-rw-r--r--   0        0        0     3623 2023-07-11 20:59:58.341914 pwnic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12958 1970-01-01 00:00:00.000000 pwnic-0.4.0/PKG-INFO
```

### Comparing `pwnic-0.3.0/LICENSE` & `pwnic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwnic-0.3.0/README.md` & `pwnic-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # pwnic
 
 <div align="center">
 
-[![Build status](https://github.com/pwnic/pwnic/workflows/build/badge.svg?branch=master&event=push)](https://github.com/pwnic/pwnic/actions?query=workflow%3Abuild)
+[![Build status](https://github.com/parmigggiana/pwnic/workflows/build/badge.svg?branch=master&event=push)](https://github.com/parmigggiana/pwnic/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/pwnic.svg)](https://pypi.org/project/pwnic/)
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/pwnic/pwnic/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pwnic/pwnic/blob/master/.pre-commit-config.yaml)
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/pwnic/pwnic/releases)
-[![License](https://img.shields.io/github/license/pwnic/pwnic)](https://github.com/pwnic/pwnic/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/parmigggiana/pwnic)](https://github.com/parmigggiana/pwnic/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
 
 </div>
 
 ## Very first steps
```

### Comparing `pwnic-0.3.0/pyproject.toml` & `pwnic-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pwnic"
-version = "0.3.0"
+version = "0.4.0"
 description = "Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template"
 readme = "README.md"
 authors = ["pwnic <francesco.basile12@studenti.unina.it>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/pwnic/pwnic"
 homepage = "https://github.com/pwnic/pwnic"
 
@@ -49,14 +49,15 @@
 safety = "^2.3.5"
 coverage = "^7.2.7"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.1.0"
 black = {version = "^23.7.0", allow-prereleases = true}
 httpx = "^0.24.1"
+icecream = "^2.1.3"
 
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py311"]
 line-length = 79
 color = true
@@ -112,14 +113,18 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
+exclude = [
+    'tests/exploits',
+    'exploits'
+]
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
 norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__", "tests/exploits"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 
@@ -139,7 +144,10 @@
 
 [coverage.run]
 branch = true
 
 [coverage.report]
 fail_under = 50
 show_missing = true
+
+[project.scripts]
+pwnic = "pwnic:__main__"
```

### Comparing `pwnic-0.3.0/PKG-INFO` & `pwnic-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwnic
-Version: 0.3.0
+Version: 0.4.0
 Summary: Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
 Home-page: https://github.com/pwnic/pwnic
 License: GNU GPL v3.0
 Author: pwnic
 Author-email: francesco.basile12@studenti.unina.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,23 +21,19 @@
 Project-URL: Repository, https://github.com/pwnic/pwnic
 Description-Content-Type: text/markdown
 
 # pwnic
 
 <div align="center">
 
-[![Build status](https://github.com/pwnic/pwnic/workflows/build/badge.svg?branch=master&event=push)](https://github.com/pwnic/pwnic/actions?query=workflow%3Abuild)
+[![Build status](https://github.com/parmigggiana/pwnic/workflows/build/badge.svg?branch=master&event=push)](https://github.com/parmigggiana/pwnic/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/pwnic.svg)](https://pypi.org/project/pwnic/)
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/pwnic/pwnic/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pwnic/pwnic/blob/master/.pre-commit-config.yaml)
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/pwnic/pwnic/releases)
-[![License](https://img.shields.io/github/license/pwnic/pwnic)](https://github.com/pwnic/pwnic/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/parmigggiana/pwnic)](https://github.com/parmigggiana/pwnic/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
 
 </div>
 
 ## Very first steps
```

