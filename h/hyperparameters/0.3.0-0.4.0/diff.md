# Comparing `tmp/hyperparameters-0.3.0.tar.gz` & `tmp/hyperparameters-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameters-0.3.0.tar", max compression
+gzip compressed data, was "hyperparameters-0.4.0.tar", max compression
```

## Comparing `hyperparameters-0.3.0.tar` & `hyperparameters-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.3.0/LICENSE
--rw-r--r--   0        0        0     7498 2023-05-15 12:43:54.565884 hyperparameters-0.3.0/README.md
--rw-r--r--   0        0        0      768 2023-05-15 16:19:51.657110 hyperparameters-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.3.0/src/hyperparameters/__init__.py
--rw-r--r--   0        0        0    11539 2023-05-15 16:15:36.529767 hyperparameters-0.3.0/src/hyperparameters/hyperparams.py
--rw-r--r--   0        0        0     1135 2023-05-15 12:42:47.049637 hyperparameters-0.3.0/src/hyperparameters/ray_tune_hyperparams.py
--rw-r--r--   0        0        0     8242 1970-01-01 00:00:00.000000 hyperparameters-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7498 2023-05-15 12:43:54.565884 hyperparameters-0.4.0/README.md
+-rw-r--r--   0        0        0      768 2023-07-11 16:28:02.747480 hyperparameters-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.4.0/src/hyperparameters/__init__.py
+-rw-r--r--   0        0        0    11465 2023-07-11 16:22:52.749997 hyperparameters-0.4.0/src/hyperparameters/hyperparams.py
+-rw-r--r--   0        0        0     1135 2023-05-15 12:42:47.049637 hyperparameters-0.4.0/src/hyperparameters/ray_tune_hyperparams.py
+-rw-r--r--   0        0        0     8242 1970-01-01 00:00:00.000000 hyperparameters-0.4.0/PKG-INFO
```

### Comparing `hyperparameters-0.3.0/LICENSE` & `hyperparameters-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.3.0/README.md` & `hyperparameters-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.3.0/pyproject.toml` & `hyperparameters-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Hyperparameters"
-version = "0.3.0"
+version = "0.4.0"
 description = "Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!"
 authors = ["Oleh Lokshyn <olokshyn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/olokshyn/Hyperparameters"
```

### Comparing `hyperparameters-0.3.0/src/hyperparameters/hyperparams.py` & `hyperparameters-0.4.0/src/hyperparameters/hyperparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import os
 from functools import partial, wraps
-from typing import Any, Iterator, TypeVar, Protocol, _ProtocolMeta, Optional
+from typing import Any, Iterator, Optional, Protocol, TypeVar, _ProtocolMeta
 
 from pydantic.fields import Field, Undefined, Validator
 from pydantic.main import BaseModel, ModelField, ModelMetaclass
 
 
 class HyperparamInfo(BaseModel):
     class Config:
@@ -13,15 +13,15 @@
         arbitrary_types_allowed = True
 
     description: str
     default: Any = None
     tunable: bool = False
     search_space: Any = None
     choices: list[Any] | None = None
-    is_path: bool = False
+    adjust_relative_path: bool = False
 
     annotation: Any = None
     type_: Any = None
     required: bool = False
 
     def can_be_none(self) -> bool:
         if self.annotation is Any:
@@ -32,27 +32,27 @@
 def HP(
     description: str,
     *,
     default: Any = Undefined,
     tunable: bool | None = None,
     search_space: Any = None,
     choices: list[Any] | None = None,
-    is_path: bool = False,
+    adjust_relative_path: bool = False,
 ):
     field = Field(
         default=default,
         description=description,
     )
     field.extra["info"] = HyperparamInfo(
         description=description,
         default=default if default is not Undefined else None,
         tunable=tunable if tunable is not None else search_space is not None,
         search_space=search_space,
         choices=choices,
-        is_path=is_path,
+        adjust_relative_path=adjust_relative_path,
     )
     return field
 
 
 def _choices_validator(value: Any, *, field_name: str, choices: list[Any]) -> None:
     if value not in choices:
         raise ValueError(
@@ -76,17 +76,14 @@
             continue
         if hasattr(config, name):
             return getattr(config, name)
     return default
 
 
 def _get_relative_paths_root(cls: type) -> Optional[str]:
-    should_adjust = _get_config_value(cls, "adjust_relative_paths", False)
-    if not should_adjust:
-        return None
     return _get_config_value(cls, "relative_paths_root", None)
 
 
 class HyperparamsMeta(ModelMetaclass, _ProtocolMeta):
     def __new__(mcs, name, bases, namespace, **kwargs) -> type[BaseModel]:
         cls: type[BaseModel] = super().__new__(mcs, name, bases, namespace, **kwargs)
         relative_paths_root = _get_relative_paths_root(cls)
@@ -96,15 +93,15 @@
 
             info.type_ = field.type_
             info.annotation = field.annotation
             info.required = field.required is True
 
             if (
                 relative_paths_root
-                and info.is_path
+                and info.adjust_relative_path
                 and info.default is not None
                 and not os.path.isabs(info.default)
             ):
                 value = os.path.join(relative_paths_root, info.default)
                 info.default = value
                 field.default = value
 
@@ -191,33 +188,32 @@
 class Hyperparams(BaseModel, HyperparamsProtocol, metaclass=HyperparamsMeta):
     class Config:
         # BaseModel configs
         validate_assignment = True
         arbitrary_types_allowed = True
 
         # Hyperparams config
-        adjust_relative_paths: bool = False
         relative_paths_root: str = os.getcwd()
 
     def __init__(self, **data: Any) -> None:
         relative_paths_root = _get_relative_paths_root(self.__class__)
         if relative_paths_root:
             for name in data:
                 if name not in self.__fields__:
                     continue
                 info: HyperparamInfo = _load_info(name, self.__fields__[name])
-                if info.is_path and not os.path.isabs(data[name]):
+                if info.adjust_relative_path and not os.path.isabs(data[name]):
                     data[name] = os.path.join(relative_paths_root, data[name])
         super().__init__(**data)
 
     def __setattr__(self, name, value) -> None:
         relative_paths_root = _get_relative_paths_root(self.__class__)
         if relative_paths_root:
             info: HyperparamInfo = _load_info(name, self.__fields__[name])
-            if info.is_path and not os.path.isabs(value):
+            if info.adjust_relative_path and not os.path.isabs(value):
                 value = os.path.join(relative_paths_root, value)
         return super().__setattr__(name, value)
 
     @classmethod
     def parameters(cls: type[SelfHyperparams]) -> dict[str, HyperparamInfo]:
         return {
             field_name: _load_info(field_name, field)
```

### Comparing `hyperparameters-0.3.0/src/hyperparameters/ray_tune_hyperparams.py` & `hyperparameters-0.4.0/src/hyperparameters/ray_tune_hyperparams.py`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.3.0/PKG-INFO` & `hyperparameters-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameters
-Version: 0.3.0
+Version: 0.4.0
 Summary: Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!
 License: MIT
 Author: Oleh Lokshyn
 Author-email: olokshyn@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

