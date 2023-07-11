# Comparing `tmp/model_transformer-0.1.1.tar.gz` & `tmp/model_transformer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_transformer-0.1.1.tar", max compression
+gzip compressed data, was "model_transformer-0.1.2.tar", max compression
```

## Comparing `model_transformer-0.1.1.tar` & `model_transformer-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      989 2023-06-20 13:55:39.433417 model_transformer-0.1.1/README.md
--rw-r--r--   0        0        0     2030 2023-06-20 13:12:52.933951 model_transformer-0.1.1/model_transformer/__init__.py
--rw-r--r--   0        0        0      384 2023-06-20 13:55:35.223418 model_transformer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 model_transformer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      989 2023-06-20 13:55:39.433417 model_transformer-0.1.2/README.md
+-rw-r--r--   0        0        0     2210 2023-07-11 00:44:21.237851 model_transformer-0.1.2/model_transformer/__init__.py
+-rw-r--r--   0        0        0      384 2023-07-11 00:45:55.727835 model_transformer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 model_transformer-0.1.2/PKG-INFO
```

### Comparing `model_transformer-0.1.1/README.md` & `model_transformer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `model_transformer-0.1.1/model_transformer/__init__.py` & `model_transformer-0.1.2/model_transformer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Any
+from functools import partial
+from typing import Any, Generic, List, TypeVar
 
-from functools import wraps, partial
+_InputDict = TypeVar("_InputDict", bound=dict)
+_OutputDict = TypeVar("_OutputDict", bound=dict)
 
 
 class BaseField:
     def __call__(self, row: dict) -> Any:
         raise NotImplementedError("BaseField is an abstract class")
 
 
@@ -19,15 +21,15 @@
 
         if self.filter:
             data = self.filter(data)
 
         return data
 
 
-class Transformer:
+class Transformer(Generic[_InputDict, _OutputDict]):
     """Schema is a base class for all schemas defined.
 
     It provides a way to define a schema for a given data source.
     """
 
     @property
     def fields(self):
@@ -45,18 +47,18 @@
 
         return {**defined_fields, **dynamic_fields}
 
     @property
     def field_names(self):
         return self.fields.keys()
 
-    def transform_row(self, row: dict) -> dict:
+    def transform_row(self, row: _InputDict) -> _OutputDict:
         return {k: field(row) for k, field in self.fields.items()}
 
-    def transform(self, rows: list[dict]) -> Any:
+    def transform(self, rows: list[_InputDict]) -> List[_OutputDict]:
         return [self.transform_row(row) for row in rows]
 
 
 class CombineTransformers:
     def __init__(self, **transformers) -> None:
         assert all(isinstance(t, Transformer) for t in transformers.values())
```

### Comparing `model_transformer-0.1.1/PKG-INFO` & `model_transformer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-transformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Giancarlo Rocha
 Author-email: giancarloiff@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

