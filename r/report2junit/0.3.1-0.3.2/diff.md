# Comparing `tmp/report2junit-0.3.1.tar.gz` & `tmp/report2junit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report2junit-0.3.1.tar", max compression
+gzip compressed data, was "report2junit-0.3.2.tar", max compression
```

## Comparing `report2junit-0.3.1.tar` & `report2junit-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1052 2023-06-26 06:53:12.165052 report2junit-0.3.1/LICENSE.md
--rw-r--r--   0        0        0      902 2023-06-26 06:53:13.145058 report2junit-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1457 2023-06-26 06:53:13.145058 report2junit-0.3.1/report2junit/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/junit.py
--rw-r--r--   0        0        0      886 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/cfn_guard.py
--rw-r--r--   0        0        0     1402 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/cfn_nag.py
--rw-r--r--   0        0        0     1705 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/junit.py
--rw-r--r--   0        0        0      328 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/noreport.py
--rw-r--r--   0        0        0     1347 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/report_factory.py
--rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 report2junit-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-11 07:03:57.383296 report2junit-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0      901 2023-07-11 07:03:58.067293 report2junit-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1433 2023-07-11 07:03:58.067293 report2junit-0.3.2/report2junit/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/junit.py
+-rw-r--r--   0        0        0      886 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/cfn_guard.py
+-rw-r--r--   0        0        0     1402 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/cfn_nag.py
+-rw-r--r--   0        0        0     1705 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/junit.py
+-rw-r--r--   0        0        0      328 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/noreport.py
+-rw-r--r--   0        0        0     1347 2023-07-11 07:03:57.383296 report2junit-0.3.2/report2junit/reports/report_factory.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 report2junit-0.3.2/PKG-INFO
```

### Comparing `report2junit-0.3.1/LICENSE.md` & `report2junit-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/pyproject.toml` & `report2junit-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "report2junit"
-version = "0.3.1"
+version = "0.3.2"
 description = "`report2junit` is a tool that converts various reports into the JUnit format."
 authors = ["Joris Conijn <joris@conijnonline.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 junit-xml = "^1.9"
 click = "^8.0.3"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-mypy = "^0.910"
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-pytest-mypy = "^0.8.1"
+black = "^23.7.0"
+mypy = "^1.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pytest-mypy = "^0.10.3"
 toml = "^0.10.2"
-types-toml = "^0.10.1"
-twine = "^3.4.2"
+types-toml = "^0.10.8"
+twine = "^4.0.2"
 radon = "^5.1.0"
-xenon = "^0.8.0"
+xenon = "^0.9.0"
 
 [tool.poetry.scripts]
 report2junit = 'report2junit:main'
 
 [tool.semantic_release]
 version_variable = [
     "report2junit/__init__.py:__version__",
```

### Comparing `report2junit-0.3.1/report2junit/__init__.py` & `report2junit-0.3.2/report2junit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os.path
 import click
 
 from report2junit.junit import JUnitOutput
 from report2junit.reports import AVAILABLE_REPORTS
 
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.argument("source-files", nargs=-1)
 @click.option("--destination-file", required=False)
 @click.option("--fail-on-failures/--ignore-failures", default=True)
 def main(
     source_files: List[str], destination_file: Optional[str], fail_on_failures: bool
 ) -> None:
     """
@@ -42,11 +42,7 @@
 def initialize_report(
     destination_file: Optional[str], source_files: List[str]
 ) -> JUnitOutput:
     if not destination_file:
         destination_file = os.path.join(os.path.dirname(source_files[0]), "junit.xml")
 
     return JUnitOutput(destination_file)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `report2junit-0.3.1/report2junit/junit.py` & `report2junit-0.3.2/report2junit/junit.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/report2junit/reports/__init__.py` & `report2junit-0.3.2/report2junit/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/report2junit/reports/cfn_guard.py` & `report2junit-0.3.2/report2junit/reports/cfn_guard.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/report2junit/reports/cfn_nag.py` & `report2junit-0.3.2/report2junit/reports/cfn_nag.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/report2junit/reports/junit.py` & `report2junit-0.3.2/report2junit/reports/junit.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/report2junit/reports/report_factory.py` & `report2junit-0.3.2/report2junit/reports/report_factory.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.1/PKG-INFO` & `report2junit-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report2junit
-Version: 0.3.1
+Version: 0.3.2
 Summary: `report2junit` is a tool that converts various reports into the JUnit format.
 License: MIT
 Author: Joris Conijn
 Author-email: joris@conijnonline.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

