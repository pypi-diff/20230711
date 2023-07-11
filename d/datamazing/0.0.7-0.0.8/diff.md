# Comparing `tmp/datamazing-0.0.7.tar.gz` & `tmp/datamazing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.7.tar", max compression
+gzip compressed data, was "datamazing-0.0.8.tar", max compression
```

## Comparing `datamazing-0.0.7.tar` & `datamazing-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0       21 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      113 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      826 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3752 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     2763 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/types.py
--rw-r--r--   0        0        0      690 2023-07-10 09:30:34.672805 datamazing-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      826 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3818 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     2763 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2070 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-11 13:08:32.740400 datamazing-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.8/PKG-INFO
```

### Comparing `datamazing-0.0.7/datamazing/pandas/testing/assertions.py` & `datamazing-0.0.8/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.7/datamazing/pandas/testing/data.py` & `datamazing-0.0.8/datamazing/pandas/testing/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,20 @@
         return values
     if not (values_isoformat == values).all():
         # if original values is not in ISO 8601 format, return original values
         return values
     return converted_values
 
 
-def make_df(data: list[str]):
-    pd.DataFrame.from_records(data)
+def make_df(data: list[dict]):
+    return pd.DataFrame.from_records(data)
+
+
+def make_series(data: dict):
+    return pd.Series(data)
 
 
 def read_df(
     filename: str,
     subfolder: str = "data",
 ) -> pd.DataFrame:
     """
```

### Comparing `datamazing-0.0.7/datamazing/pandas/transformations/basic.py` & `datamazing-0.0.8/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.7/datamazing/pandas/transformations/grouping.py` & `datamazing-0.0.8/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.7/datamazing/pandas/transformations/resampling.py` & `datamazing-0.0.8/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.7/datamazing/pandas/types.py` & `datamazing-0.0.8/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.7/pyproject.toml` & `datamazing-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.7"
+version = "0.0.8"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
@@ -12,14 +12,15 @@
 pandas = "^1.4.3"
 pyarrow = "^9.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.20.0"
+pyspark = "3.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `datamazing-0.0.7/PKG-INFO` & `datamazing-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

