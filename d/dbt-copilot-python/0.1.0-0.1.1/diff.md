# Comparing `tmp/dbt_copilot_python-0.1.0.tar.gz` & `tmp/dbt_copilot_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_python-0.1.0.tar", max compression
+gzip compressed data, was "dbt_copilot_python-0.1.1.tar", max compression
```

## Comparing `dbt_copilot_python-0.1.0.tar` & `dbt_copilot_python-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1090 2023-06-30 08:44:11.359787 dbt_copilot_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     1309 2023-07-05 10:55:56.015382 dbt_copilot_python-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 11:33:07.684277 dbt_copilot_python-0.1.0/dbt_copilot_python/__init__.py
--rw-r--r--   0        0        0      809 2023-07-03 11:33:07.684543 dbt_copilot_python-0.1.0/dbt_copilot_python/database.py
--rw-r--r--   0        0        0      692 2023-07-03 11:33:07.684778 dbt_copilot_python-0.1.0/dbt_copilot_python/network.py
--rw-r--r--   0        0        0      128 2023-07-03 11:33:07.684860 dbt_copilot_python-0.1.0/dbt_copilot_python/utility.py
--rw-r--r--   0        0        0      582 2023-07-05 11:06:00.791721 dbt_copilot_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 dbt_copilot_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-30 08:44:11.359787 dbt_copilot_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1309 2023-07-10 14:34:46.022458 dbt_copilot_python-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 11:33:07.684277 dbt_copilot_python-0.1.1/dbt_copilot_python/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-11 11:36:47.245860 dbt_copilot_python-0.1.1/dbt_copilot_python/database.py
+-rw-r--r--   0        0        0      692 2023-07-03 11:33:07.684778 dbt_copilot_python-0.1.1/dbt_copilot_python/network.py
+-rw-r--r--   0        0        0      128 2023-07-03 11:33:07.684860 dbt_copilot_python-0.1.1/dbt_copilot_python/utility.py
+-rw-r--r--   0        0        0      582 2023-07-11 11:37:29.616935 dbt_copilot_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 dbt_copilot_python-0.1.1/PKG-INFO
```

### Comparing `dbt_copilot_python-0.1.0/LICENSE` & `dbt_copilot_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.0/README.md` & `dbt_copilot_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.0/dbt_copilot_python/network.py` & `dbt_copilot_python-0.1.1/dbt_copilot_python/network.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.0/pyproject.toml` & `dbt_copilot_python-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-copilot-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Helper functions to run Django and Flask applications in AWS Copilot/ECS."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 readme = "README.md"
 packages = [{ include = "dbt_copilot_python" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dbt_copilot_python-0.1.0/PKG-INFO` & `dbt_copilot_python-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helper functions to run Django and Flask applications in AWS Copilot/ECS.
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

