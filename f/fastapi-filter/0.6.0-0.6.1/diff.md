# Comparing `tmp/fastapi_filter-0.6.0.tar.gz` & `tmp/fastapi_filter-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_filter-0.6.0.tar", max compression
+gzip compressed data, was "fastapi_filter-0.6.1.tar", max compression
```

## Comparing `fastapi_filter-0.6.0.tar` & `fastapi_filter-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/LICENSE
--rw-r--r--   0        0        0     1945 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/README.md
--rw-r--r--   0        0        0      107 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/base/__init__.py
--rw-r--r--   0        0        0     7764 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/base/filter.py
--rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/__init__.py
--rw-r--r--   0        0        0       50 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/__init__.py
--rw-r--r--   0        0        0     2511 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/filter.py
--rw-r--r--   0        0        0       50 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/filter.py
--rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/py.typed
--rw-r--r--   0        0        0     2309 2023-04-16 13:44:15.346773 fastapi_filter-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 fastapi_filter-0.6.0/setup.py
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 fastapi_filter-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-11 11:08:54.121215 fastapi_filter-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1945 2023-07-11 11:08:54.121215 fastapi_filter-0.6.1/README.md
+-rw-r--r--   0        0        0      107 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/base/__init__.py
+-rw-r--r--   0        0        0     7772 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/base/filter.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/contrib/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/contrib/mongoengine/__init__.py
+-rw-r--r--   0        0        0     2511 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/contrib/mongoengine/filter.py
+-rw-r--r--   0        0        0       50 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4529 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/contrib/sqlalchemy/filter.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:08:54.125215 fastapi_filter-0.6.1/fastapi_filter/py.typed
+-rw-r--r--   0        0        0     3115 2023-07-11 11:08:54.129216 fastapi_filter-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 fastapi_filter-0.6.1/setup.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 fastapi_filter-0.6.1/PKG-INFO
```

### Comparing `fastapi_filter-0.6.0/LICENSE` & `fastapi_filter-0.6.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Yurii Karabas
+Copyright (c) 2022 Arthur Rio
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fastapi_filter-0.6.0/README.md` & `fastapi_filter-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.6.0/fastapi_filter/base/filter.py` & `fastapi_filter-0.6.1/fastapi_filter/base/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,19 @@
         ...
 
     @property
     def ordering_values(self):
         """Check that the ordering field is present on the class definition."""
         try:
             return getattr(self, self.Constants.ordering_field_name)
-        except AttributeError:
+        except AttributeError as e:
             raise AttributeError(
                 f"Ordering field {self.Constants.ordering_field_name} is not defined. "
                 "Make sure to add it to your filter class."
-            )
+            ) from e
 
     @validator("*", pre=True)
     def split_str(cls, value, field):  # pragma: no cover
         ...
 
     @validator("*", pre=True, allow_reuse=True, check_fields=False)
     def strip_order_by_values(cls, value, values, field):
@@ -194,15 +194,15 @@
             field_type = Filter.__annotations__.get(f.name, f.outer_type_)
             ret[f.name] = (field_type if f.required else Optional[field_type], field_info)
 
     return ret
 
 
 def FilterDepends(Filter: Type[BaseFilterModel], *, by_alias: bool = False, use_cache: bool = True) -> Any:
-    """This is a hack to support lists in filters.
+    """Use a hack to support lists in filters.
 
     FastAPI doesn't support it yet: https://github.com/tiangolo/fastapi/issues/50
 
     What we do is loop through the fields of a filter and change any `list` field to a `str` one so that it won't be
     excluded from the possible query parameters.
 
     When we apply the filter, we build the original filter to properly validate the data (i.e. can the string be parsed
```

### Comparing `fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/filter.py` & `fastapi_filter-0.6.1/fastapi_filter/contrib/mongoengine/filter.py`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/filter.py` & `fastapi_filter-0.6.1/fastapi_filter/contrib/sqlalchemy/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from sqlalchemy import or_
 from sqlalchemy.orm import Query
 from sqlalchemy.sql.selectable import Select
 
 from ...base.filter import BaseFilterModel
 
 
-def _backward_compatible_value_for_like_and_ilike(value):
-    """Adds % if not in value to be backward compatible.
+def _backward_compatible_value_for_like_and_ilike(value: str):
+    """Add % if not in value to be backward compatible.
 
     Args:
-        value: The value to filter.
+        value (str): The value to filter.
 
     Returns:
         Either the unmodified value if a percent sign is present, the value wrapped in % otherwise to preserve
         current behavior.
     """
     if "%" not in value:
         warn(
             "You must pass the % character explicitly to use the like and ilike operators.",
             DeprecationWarning,
+            stacklevel=2,
         )
         value = f"%{value}%"
     return value
 
 
 _orm_operator_transformer = {
     "neq": lambda value: ("__ne__", value),
@@ -105,19 +106,19 @@
                 if "__" in field_name:
                     field_name, operator = field_name.split("__")
                     operator, value = _orm_operator_transformer[operator](value)
                 else:
                     operator = "__eq__"
 
                 if field_name == self.Constants.search_field_name and hasattr(self.Constants, "search_model_fields"):
-
-                    def search_filter(field):
-                        return getattr(self.Constants.model, field).ilike("%" + value + "%")
-
-                    query = query.filter(or_(*list(map(search_filter, self.Constants.search_model_fields))))
+                    search_filters = [
+                        getattr(self.Constants.model, field).ilike(f"%{value}%")
+                        for field in self.Constants.search_model_fields
+                    ]
+                    query = query.filter(or_(*search_filters))
                 else:
                     model_field = getattr(self.Constants.model, field_name)
                     query = query.filter(getattr(model_field, operator)(value))
 
         return query
 
     def sort(self, query: Union[Query, Select]):
```

### Comparing `fastapi_filter-0.6.0/pyproject.toml` & `fastapi_filter-0.6.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length=120
 skip_gitignore = true
 
+[tool.flynt]
+line-length = 120
+
 [tool.mypy]
 mypy_path = [
   "fastapi_filter",
 ]
 show_error_codes = true
 check_untyped_defs = true
 plugins = [
@@ -20,17 +23,57 @@
 module = [
   "bson.objectid",
   "mongoengine.*",
   "uvicorn.*",
 ]
 ignore_missing_imports = true
 
+[tool.ruff]
+select = [
+  "A",
+  "B",
+  "C",
+  "D",
+  "E",
+  "F"
+]
+ignore = [
+  "A003",  # Argument name should be lowercase.
+  "B008",  # Do not perform function calls in argument defaults.
+  "D1",  # Missing docstring https://www.pydocstyle.org/en/2.1.1/error_codes.html.
+  "D203",  # 1 blank line required before class docstring.
+  "D213",  # Multi-line docstring summary should start at the second line.
+]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F"]
+unfixable = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".ruff_cache",
+]
+
+line-length = 120
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.11.
+target-version = "py311"
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.poetry]
 name = "fastapi-filter"
-version = "0.6.0"
+version = "0.6.1"
 description = "FastAPI filter"
 authors = ["Arthur Rio <arthur.rio44@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/arthurio/fastapi-filter"
 classifiers = [
     "Natural Language :: English",
@@ -46,28 +89,23 @@
 ]
 
 [tool.poetry.dependencies]
 SQLAlchemy = {version = ">=1.4.36,<2.1.0", optional = true}
 fastapi = ">=0.78,<1.0"
 mongoengine = {version = ">=0.24.1,<0.28.0", optional = true}
 pydantic = ">=1.10.0,<2.0.0"
-python = ">=3.8,<3.12"
+python = ">=3.8,<4.0"
 
 [tool.poetry.dev-dependencies]
 Faker = "^18.0.0"
 SQLAlchemy-Utils = "^0.41.0"
-aiosqlite = "^0.18.0"
+aiosqlite = "^0.19.0"
 bandit = "^1.7.5"
 black = "^23.1.0"
-flake8 = "^5.0.4"
-flake8-breakpoint = "^1.1.0"
-flake8-builtins = "^2.1.0"
-flake8-docstrings = "^1.7.0"
-flake8-simplify = "^0.20.0"
-flynt = "^0.77"
+flynt = "^1.0.0"
 greenlet = "^2.0.2"
 httpx = "^0.24.0"
 ipython = "^8.11.0"
 isort = "^5.12.0"
 mkdocs-material = "^9.1.2"
 mypy = "^1.1"
 mypy-extensions = "^1.0.0"
@@ -80,20 +118,21 @@
 pytest-pudb = "^0.7.0"
 python-lsp-server = "^1.7.1"
 requests = "^2.28.2"
 tomli = "^2.0.1"
 types-click = "^7.1.8"
 types-setuptools = "^67.6.0"
 typing-extensions = "^4.5.0"
-uvicorn = "^0.21.0"
+uvicorn = "^0.22.0"
 
 [tool.poetry.extras]
 mongoengine = ["mongoengine"]
 sqlalchemy = ["SQLAlchemy"]
 all = ["mongoengine", "SQLAlchemy"]
 
 [tool.poetry.group.dev.dependencies]
-nox = "^2022.11.21"
+nox = "^2023.0.0"
+ruff = "^0.0.277"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `fastapi_filter-0.6.0/setup.py` & `fastapi_filter-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 extras_require = \
 {'all': ['SQLAlchemy>=1.4.36,<2.1.0', 'mongoengine>=0.24.1,<0.28.0'],
  'mongoengine': ['mongoengine>=0.24.1,<0.28.0'],
  'sqlalchemy': ['SQLAlchemy>=1.4.36,<2.1.0']}
 
 setup_kwargs = {
     'name': 'fastapi-filter',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'FastAPI filter',
     'long_description': '[![pypi downloads](https://img.shields.io/pypi/dm/fastapi-filter?color=%232E73B2&logo=python&logoColor=%23F9D25F)](https://pypi.org/project/fastapi-filter)\n[![codecov](https://codecov.io/gh/arthurio/fastapi-filter/branch/main/graph/badge.svg?token=I1DVBL1682)](https://codecov.io/gh/arthurio/fastapi-filter)\n[![Netlify Status](https://api.netlify.com/api/v1/badges/83451c4f-76dd-4154-9b2d-61f654eb0704/deploy-status)](https://fastapi-filter.netlify.app/)\n[![CodeQL](https://github.com/arthurio/fastapi-filter/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/arthurio/fastapi-filter/actions/workflows/codeql-analysis.yml)\n\n# FastAPI filter\n\n## Compatibility\n\n**Required:**\n  * Python: >=3.8, <3.12\n  * Fastapi: >=0.78, <1.0\n  * Pydantic: >=1.10.0, <2.0.0\n\n\n**Optional**\n  * MongoEngine: >=0.24.1, <0.28.0\n  * SQLAlchemy: >=1.4.36, <2.1.0\n\n## Installation\n\n```bash\n# Basic version\npip install fastapi-filter\n\n# With backends\npip install fastapi-filter[all]\n\n# More selective\npip install fastapi-filter[sqlalchemy]\npip install fastapi-filter[mongoengine]\n```\n\n## Documentation\n\nPlease visit: [https://fastapi-filter.netlify.app/](https://fastapi-filter.netlify.app/)\n\n## Examples\n\n![Swagger UI](https://raw.githubusercontent.com/arthurio/fastapi-filter/main/docs/swagger-ui.png)\n\nYou can play with examples:\n\n```bash\npip install poetry\npoetry install\npython examples/fastapi_filter_sqlalchemy.py\n```\n\n### Filter\n\nhttps://user-images.githubusercontent.com/950449/176737541-0e36b72f-38e2-4368-abfa-8bbc0c82e8ae.mp4\n\n### Order by\n\nhttps://user-images.githubusercontent.com/950449/176747056-ea82d6b9-cb3b-43eb-aec7-96ba0bc79e8b.mp4\n\n## Contribution\n\nYou can run tests with `pytest`.\n\n```bash\npip install poetry\npoetry install --extras all\npytest\n```\n\n<img width="884" alt="arthur_Arthurs-MacBook-Pro-2___code_fastapi-filter" src="https://user-images.githubusercontent.com/950449/176737623-a77f15d6-4e60-4c06-bdb7-b3d77f346a54.png">\n',
     'author': 'Arthur Rio',
     'author_email': 'arthur.rio44@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/arthurio/fastapi-filter',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fastapi_filter-0.6.0/PKG-INFO` & `fastapi_filter-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-filter
-Version: 0.6.0
+Version: 0.6.1
 Summary: FastAPI filter
 Home-page: https://github.com/arthurio/fastapi-filter
 License: MIT
 Author: Arthur Rio
 Author-email: arthur.rio44@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

