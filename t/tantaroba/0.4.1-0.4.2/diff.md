# Comparing `tmp/tantaroba-0.4.1.tar.gz` & `tmp/tantaroba-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tantaroba-0.4.1.tar", max compression
+gzip compressed data, was "tantaroba-0.4.2.tar", max compression
```

## Comparing `tantaroba-0.4.1.tar` & `tantaroba-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      900 2023-04-28 10:08:47.277778 tantaroba-0.4.1/LICENSE
--rw-r--r--   0        0        0      199 2023-04-28 10:08:47.277778 tantaroba-0.4.1/README.md
--rw-r--r--   0        0        0     1985 2023-04-28 10:08:47.278778 tantaroba-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/__init__.py
--rw-r--r--   0        0        0       22 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/__version__.py
--rw-r--r--   0        0        0      499 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/dynamic_import.py
--rw-r--r--   0        0        0      641 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/iterator_helpers.py
--rw-r--r--   0        0        0      936 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/log.py
--rw-r--r--   0        0        0      683 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/profile.py
--rw-r--r--   0        0        0       88 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/scripts/script.py
--rw-r--r--   0        0        0      691 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/strings.py
--rw-r--r--   0        0        0      528 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/yaml.py
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 tantaroba-0.4.1/setup.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 tantaroba-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-11 10:06:22.024861 tantaroba-0.4.2/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-11 10:06:22.024861 tantaroba-0.4.2/README.md
+-rw-r--r--   0        0        0     1984 2023-07-11 10:06:22.024861 tantaroba-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 10:06:22.045944 tantaroba-0.4.2/tantaroba/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/__version__.py
+-rw-r--r--   0        0        0      499 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/dynamic_import.py
+-rw-r--r--   0        0        0      641 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/iterator_helpers.py
+-rw-r--r--   0        0        0      936 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/log.py
+-rw-r--r--   0        0        0      683 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/profile.py
+-rw-r--r--   0        0        0       88 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/scripts/script.py
+-rw-r--r--   0        0        0      691 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/strings.py
+-rw-r--r--   0        0        0      528 2023-07-11 10:06:22.025778 tantaroba-0.4.2/tantaroba/yaml.py
+-rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 tantaroba-0.4.2/setup.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 tantaroba-0.4.2/PKG-INFO
```

### Comparing `tantaroba-0.4.1/LICENSE` & `tantaroba-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/pyproject.toml` & `tantaroba-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tantaroba"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python package template"
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/tantardini/tantaroba"
 keywords = ["utils", "postgresql", "yaml"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
 pandas = ">=1.5.3"
-numpy = "^1.24.2"
+numpy = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 commitizen = "^2.35.0"
 python-semantic-release = "^7.32.1"
 pytest = "^7.1.3"
```

### Comparing `tantaroba-0.4.1/tantaroba/iterator_helpers.py` & `tantaroba-0.4.2/tantaroba/iterator_helpers.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/tantaroba/log.py` & `tantaroba-0.4.2/tantaroba/log.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/tantaroba/profile.py` & `tantaroba-0.4.2/tantaroba/profile.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/tantaroba/strings.py` & `tantaroba-0.4.2/tantaroba/strings.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/tantaroba/yaml.py` & `tantaroba-0.4.2/tantaroba/yaml.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.1/setup.py` & `tantaroba-0.4.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['tantaroba', 'tantaroba.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['loguru>=0.6.0,<0.7.0', 'numpy>=1.24.2,<2.0.0', 'pandas>=1.5.3']
+['loguru>=0.6.0,<0.7.0', 'numpy>=1.0.0,<2.0.0', 'pandas>=1.5.3']
 
 setup_kwargs = {
     'name': 'tantaroba',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Python package template',
     'long_description': '# tantaroba\n\nCollection of miscellanoeus utilities commonly used across different projects.\n\n## Installation\n```\npip install tantaroba\n```\n\n## Usage\nDescribe how to launch and use tantaroba project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tantardini/tantaroba',
```

### Comparing `tantaroba-0.4.1/PKG-INFO` & `tantaroba-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tantaroba
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package template
 Home-page: https://gitlab.com/tantardini/tantaroba
 Keywords: utils,postgresql,yaml
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Project-URL: Repository, https://gitlab.com/tantardini/tantaroba
 Description-Content-Type: text/markdown
 
 # tantaroba
 
 Collection of miscellanoeus utilities commonly used across different projects.
```

