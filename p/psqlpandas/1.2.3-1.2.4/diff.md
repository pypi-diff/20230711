# Comparing `tmp/psqlpandas-1.2.3.tar.gz` & `tmp/psqlpandas-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.2.3.tar", max compression
+gzip compressed data, was "psqlpandas-1.2.4.tar", max compression
```

## Comparing `psqlpandas-1.2.3.tar` & `psqlpandas-1.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      900 2023-07-05 11:04:01.409203 psqlpandas-1.2.3/LICENSE
--rw-r--r--   0        0        0      199 2023-07-05 11:04:01.409203 psqlpandas-1.2.3/README.md
--rw-r--r--   0        0        0        0 2023-07-05 11:04:01.434203 psqlpandas-1.2.3/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/__version__.py
--rw-r--r--   0        0        0     7939 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     3091 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/tables.py
--rw-r--r--   0        0        0     1909 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.2.3/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-11 10:16:31.854836 psqlpandas-1.2.4/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-11 10:16:31.854836 psqlpandas-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 10:16:31.877836 psqlpandas-1.2.4/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     7939 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     3091 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/tables.py
+-rw-r--r--   0        0        0     1908 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 psqlpandas-1.2.4/setup.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 psqlpandas-1.2.4/PKG-INFO
```

### Comparing `psqlpandas-1.2.3/LICENSE` & `psqlpandas-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.3/psqlpandas/postgresql.py` & `psqlpandas-1.2.4/psqlpandas/postgresql.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.3/psqlpandas/tables.py` & `psqlpandas-1.2.4/psqlpandas/tables.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.3/pyproject.toml` & `psqlpandas-1.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.2.3"
+version = "1.2.4"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = "^2.0.3"
-numpy = "^1.24.2"
+numpy = "^1.0.0"
 psycopg2 = "^2.9.5"
 pandas = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 commitizen = "^2.35.0"
 python-semantic-release = "^7.32.1"
```

### Comparing `psqlpandas-1.2.3/setup.py` & `psqlpandas-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['psqlpandas', 'psqlpandas.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.2,<2.0.0',
+['numpy>=1.0.0,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-1.2.3/PKG-INFO` & `psqlpandas-1.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.2.3
+Version: 1.2.4
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # psqlpandas
 Utilities to communicate with postgresql database through pandas dataframes.
```

