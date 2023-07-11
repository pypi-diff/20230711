# Comparing `tmp/pwnic-0.1.0.tar.gz` & `tmp/pwnic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwnic-0.1.0.tar", max compression
+gzip compressed data, was "pwnic-0.3.0.tar", max compression
```

## Comparing `pwnic-0.1.0.tar` & `pwnic-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    32471 2023-07-05 12:46:07.759059 pwnic-0.1.0/LICENSE
--rw-r--r--   0        0        0    12475 2023-07-05 12:46:07.714059 pwnic-0.1.0/README.md
--rw-r--r--   0        0        0      346 2023-07-05 14:11:38.276666 pwnic-0.1.0/pwnic/Attacker.py
--rw-r--r--   0        0        0      239 2023-07-05 14:25:54.897615 pwnic-0.1.0/pwnic/Submitter.py
--rw-r--r--   0        0        0      394 2023-07-05 13:25:28.881792 pwnic-0.1.0/pwnic/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 13:58:47.739868 pwnic-0.1.0/pwnic/api.py
--rw-r--r--   0        0        0      461 2023-07-05 14:24:42.310527 pwnic-0.1.0/pwnic/config.py
--rw-r--r--   0        0        0      110 2023-07-05 14:25:36.182592 pwnic-0.1.0/pwnic/db.py
--rw-r--r--   0        0        0     3769 2023-07-05 14:26:54.130687 pwnic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    13361 1970-01-01 00:00:00.000000 pwnic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-07-09 18:22:17.480086 pwnic-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12475 2023-07-09 18:22:17.481086 pwnic-0.3.0/README.md
+-rw-r--r--   0        0        0      346 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/Attacker.py
+-rw-r--r--   0        0        0      239 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/Submitter.py
+-rw-r--r--   0        0        0      394 2023-07-09 18:22:17.484086 pwnic-0.3.0/pwnic/__init__.py
+-rw-r--r--   0        0        0      961 2023-07-11 15:11:07.449917 pwnic-0.3.0/pwnic/api.py
+-rw-r--r--   0        0        0      468 2023-07-09 18:31:09.133305 pwnic-0.3.0/pwnic/config.py
+-rw-r--r--   0        0        0      110 2023-07-09 18:22:17.485086 pwnic-0.3.0/pwnic/db.py
+-rw-r--r--   0        0        0     3508 2023-07-11 15:13:42.678207 pwnic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13454 1970-01-01 00:00:00.000000 pwnic-0.3.0/PKG-INFO
```

### Comparing `pwnic-0.1.0/LICENSE` & `pwnic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwnic-0.1.0/README.md` & `pwnic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pwnic-0.1.0/pyproject.toml` & `pwnic-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pwnic"
-version = "0.1.0"
+version = "0.3.0"
 description = "Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template"
 readme = "README.md"
 authors = ["pwnic <francesco.basile12@studenti.unina.it>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/pwnic/pwnic"
 homepage = "https://github.com/pwnic/pwnic"
 
@@ -28,49 +28,36 @@
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pymongo = "*"
+fastapi = "^0.100.0"
+python-multipart = "^0.0.6"
 
-[tool.poetry.dev-dependencies]
-bandit = "*"
-black = {version = "*", allow-prereleases = true}
-darglint = "*"
-isort = {extras = ["colors"], version = "*"}
-mypy = "*"
-mypy-extensions = "*"
-pre-commit = "*"
-pydocstyle = "*"
-pylint = "*"
-pytest = "*"
-pyupgrade = "*"
-safety = "*"
-coverage = "*"
-coverage-badge = "*"
-pytest-html = "*"
-pytest-cov = "*"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.4"
 pytest = "^7.4.0"
-pyupgrade = "^3.8.0"
+pyupgrade = "^3.9.0"
 safety = "^2.3.5"
 coverage = "^7.2.7"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.1.0"
-black = {version = "^23.3.0", allow-prereleases = true}
+black = {version = "^23.7.0", allow-prereleases = true}
+httpx = "^0.24.1"
+
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py311"]
 line-length = 79
 color = true
 
@@ -129,15 +116,15 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
-norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
+norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__", "tests/exploits"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 
 # Extra options:
 addopts = [
   "--strict-markers",
   "--tb=short",
   "--doctest-modules",
```

### Comparing `pwnic-0.1.0/PKG-INFO` & `pwnic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pwnic
-Version: 0.1.0
+Version: 0.3.0
 Summary: Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
 Home-page: https://github.com/pwnic/pwnic
 License: GNU GPL v3.0
 Author: pwnic
 Author-email: francesco.basile12@studenti.unina.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: pymongo
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Project-URL: Repository, https://github.com/pwnic/pwnic
 Description-Content-Type: text/markdown
 
 # pwnic
 
 <div align="center">
```

