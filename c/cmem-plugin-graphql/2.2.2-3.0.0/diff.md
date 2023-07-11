# Comparing `tmp/cmem_plugin_graphql-2.2.2.tar.gz` & `tmp/cmem_plugin_graphql-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_graphql-2.2.2.tar", max compression
+gzip compressed data, was "cmem_plugin_graphql-3.0.0.tar", max compression
```

## Comparing `cmem_plugin_graphql-2.2.2.tar` & `cmem_plugin_graphql-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      545 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/CHANGELOG.md
--rw-r--r--   0        0        0    11334 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/LICENSE
--rw-r--r--   0        0        0      372 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/README-public.md
--rw-r--r--   0        0        0        0 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/workflow/__init__.py
--rw-r--r--   0        0        0     9021 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/workflow/graphql.py
--rw-r--r--   0        0        0     1974 2023-03-10 10:28:29.761159 cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/workflow/utils.py
--rw-r--r--   0        0        0     1942 2023-03-10 10:29:00.897756 cmem_plugin_graphql-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 cmem_plugin_graphql-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11334 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/LICENSE
+-rw-r--r--   0        0        0      372 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/workflow/__init__.py
+-rw-r--r--   0        0        0     9021 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/workflow/graphql.py
+-rw-r--r--   0        0        0     1974 2023-07-11 11:04:43.759638 cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/workflow/utils.py
+-rw-r--r--   0        0        0     1931 2023-07-11 11:05:11.041819 cmem_plugin_graphql-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 cmem_plugin_graphql-3.0.0/PKG-INFO
```

### Comparing `cmem_plugin_graphql-2.2.2/CHANGELOG.md` & `cmem_plugin_graphql-3.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](https://semver.org/)
 
-## [Unreleased]
+## [3.0.0] 2023-07-11
+
+### Changed
+
+- upgrade temlate to 5.0.1 (python 3.11, CMEM 23.2, cmem-plugin-base 5)
 
-TODO: add at least one Added, Changed, Deprecated, Removed, Fixed or Security section
 
 ## [2.0.1] 2022-08-26
 
 ### Changed
 
 - description
 
+
 ## [2.0.0] 2022-07-26
 
 ### Changed
 
 - adapt plugin execute method to ExecutionContext 
 
+
 ## [1.0.0] 2022-06-16
 
 ### Added
 
 - initial version to query GraphQL API's
```

### Comparing `cmem_plugin_graphql-2.2.2/LICENSE` & `cmem_plugin_graphql-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/workflow/graphql.py` & `cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/workflow/graphql.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_graphql-2.2.2/cmem_plugin_graphql/workflow/utils.py` & `cmem_plugin_graphql-3.0.0/cmem_plugin_graphql/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_graphql-2.2.2/pyproject.toml` & `cmem_plugin_graphql-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-graphql"
-version = "2.2.2"
+version = "3.0.0"
 license = "Apache-2.0"
 description = "Send queries to a GraphQL endpoint and save the results in a JSON dataset."
 homepage = "https://github.com/eccenca/cmem-plugin-graphql"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
@@ -15,38 +15,37 @@
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin", "GraphQL"
 ]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^3.0.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 validators = "^0.20.0"
 gql = {extras = ["all"], version ="^3.4.0" }
 Jinja2 = "^3.1.2"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^4.0.0"
-pytest-memray = "^1.3.0"
-black = "^23.1.0"
-bandit = "^1.7.2"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^1.0.0"
-coverage = "^7.1.0"
-defusedxml = "^0.7.1"
-wheel = "^0.38.3"
-
-[tool.poetry.group.dev.dependencies]
+typed-ast = "^1.5.4"
 types-requests = "^2.28.11.12"
+wheel = "^0.38.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `cmem_plugin_graphql-2.2.2/PKG-INFO` & `cmem_plugin_graphql-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-graphql
-Version: 2.2.2
+Version: 3.0.0
 Summary: Send queries to a GraphQL endpoint and save the results in a JSON dataset.
 Home-page: https://github.com/eccenca/cmem-plugin-graphql
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,GraphQL
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: cmem-plugin-base (>=3.0.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Requires-Dist: gql[all] (>=3.4.0,<4.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-graphql
 
 Send queries to a GraphQL endpoint and save the results in a JSON dataset.
```

