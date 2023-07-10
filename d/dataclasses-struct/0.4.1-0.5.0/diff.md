# Comparing `tmp/dataclasses_struct-0.4.1.tar.gz` & `tmp/dataclasses_struct-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_struct-0.4.1.tar", max compression
+gzip compressed data, was "dataclasses_struct-0.5.0.tar", max compression
```

## Comparing `dataclasses_struct-0.4.1.tar` & `dataclasses_struct-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-03-13 00:20:21.169674 dataclasses_struct-0.4.1/LICENSE
--rw-r--r--   0        0        0     4419 2023-03-21 03:17:52.994873 dataclasses_struct-0.4.1/README.md
--rw-r--r--   0        0        0      716 2023-03-21 02:56:47.891082 dataclasses_struct-0.4.1/dataclasses_struct/__init__.py
--rw-r--r--   0        0        0     4114 2023-03-21 03:16:23.075177 dataclasses_struct-0.4.1/dataclasses_struct/dataclass.py
--rw-r--r--   0        0        0        0 2023-03-12 19:12:36.067613 dataclasses_struct-0.4.1/dataclasses_struct/ext/__init__.py
--rw-r--r--   0        0        0     1733 2023-03-14 00:23:45.326282 dataclasses_struct-0.4.1/dataclasses_struct/ext/mypy_plugin.py
--rw-r--r--   0        0        0     4284 2023-03-12 20:54:23.493612 dataclasses_struct-0.4.1/dataclasses_struct/field.py
--rw-r--r--   0        0        0        0 2023-03-09 03:22:03.389011 dataclasses_struct-0.4.1/dataclasses_struct/py.typed
--rw-r--r--   0        0        0      353 2023-03-09 04:25:24.661695 dataclasses_struct-0.4.1/dataclasses_struct/sizes.py
--rw-r--r--   0        0        0     1398 2023-03-21 03:26:15.185174 dataclasses_struct-0.4.1/dataclasses_struct/types.py
--rw-r--r--   0        0        0     1046 2023-03-21 03:28:16.873654 dataclasses_struct-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 dataclasses_struct-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-03-13 00:20:21.169674 dataclasses_struct-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4442 2023-05-03 01:15:52.493070 dataclasses_struct-0.5.0/README.md
+-rw-r--r--   0        0        0      716 2023-03-21 02:56:47.891082 dataclasses_struct-0.5.0/dataclasses_struct/__init__.py
+-rw-r--r--   0        0        0     4114 2023-03-21 03:16:23.075177 dataclasses_struct-0.5.0/dataclasses_struct/dataclass.py
+-rw-r--r--   0        0        0        0 2023-03-12 19:12:36.067613 dataclasses_struct-0.5.0/dataclasses_struct/ext/__init__.py
+-rw-r--r--   0        0        0     1781 2023-07-10 23:01:04.751130 dataclasses_struct-0.5.0/dataclasses_struct/ext/mypy_plugin.py
+-rw-r--r--   0        0        0     4474 2023-07-10 22:57:28.383690 dataclasses_struct-0.5.0/dataclasses_struct/field.py
+-rw-r--r--   0        0        0        0 2023-03-09 03:22:03.389011 dataclasses_struct-0.5.0/dataclasses_struct/py.typed
+-rw-r--r--   0        0        0      353 2023-03-09 04:25:24.661695 dataclasses_struct-0.5.0/dataclasses_struct/sizes.py
+-rw-r--r--   0        0        0     1398 2023-03-21 03:26:15.185174 dataclasses_struct-0.5.0/dataclasses_struct/types.py
+-rw-r--r--   0        0        0     1046 2023-07-10 23:03:27.566742 dataclasses_struct-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 dataclasses_struct-0.5.0/PKG-INFO
```

### Comparing `dataclasses_struct-0.4.1/LICENSE` & `dataclasses_struct-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.4.1/README.md` & `dataclasses_struct-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class Test:
     x: int  # or dcs.UInt64
     y: dcs.Float32
     z: dcs.Uint8
     s: Annotated[bytes, 10]
 ```
 
-```
+```python
 >>> t = Test(100, -0.25, 0xff, b'12345')
 >>> t
 Test(x=100, y=-0.25, z=255, s=b'12345')
 >>> packed = t.pack()
 >>> packed
 b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbe\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
@@ -115,19 +115,19 @@
 
 An additional class attribute, `__dataclass_struct__`, of type
 [`struct.Struct`](https://docs.python.org/3/library/struct.html#struct.Struct)
 is added. The [`struct` format
 string](https://docs.python.org/3/library/struct.html#format-strings) and packed
 size can be accessed like so:
 
-```
+```python
 >>> Test.__dataclass_struct__.format
-'@cc??bBhHiIQqqNnPfdd100s'
+'@cc??bBhHiIQqqNnPfdd100s4xqq2x3xq2x'
 >>> Test.__dataclass_struct__.size
-196
+234
 ```
 
 Default attribute values will be validated against their expected type and
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
```

### Comparing `dataclasses_struct-0.4.1/dataclasses_struct/__init__.py` & `dataclasses_struct-0.5.0/dataclasses_struct/__init__.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.4.1/dataclasses_struct/dataclass.py` & `dataclasses_struct-0.5.0/dataclasses_struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.4.1/dataclasses_struct/ext/mypy_plugin.py` & `dataclasses_struct-0.5.0/dataclasses_struct/ext/mypy_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 def transform_dataclass_struct(ctx: ClassDefContext) -> bool:
     bytes_type = ctx.api.named_type('builtins.bytes')
     tvd = TypeVarType(
         'T',
         f'{ctx.cls.info.fullname}.T',
         -1,
         [],
-        ctx.api.named_type('builtins.object')
+        ctx.api.named_type('builtins.object'),
+        ctx.api.named_type('builtins.object'),
     )
     add_method_to_class(ctx.api, ctx.cls, 'pack', [], bytes_type)
     add_method_to_class(
         ctx.api,
         ctx.cls,
         'from_packed',
         [Argument(Var('data', bytes_type), bytes_type, None, ArgKind.ARG_POS)],
```

### Comparing `dataclasses_struct-0.4.1/dataclasses_struct/field.py` & `dataclasses_struct-0.5.0/dataclasses_struct/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 from ctypes import c_size_t, c_ssize_t, c_void_p, sizeof
 from typing import Generic, Literal, Type, TypeVar
 
+from . import sizes as intsizes
 
 T = TypeVar('T')
 
 
 class Field(abc.ABC, Generic[T]):
     native_only: bool = False
     type_: Type[T]
@@ -48,25 +49,25 @@
         1: 'b',
         2: 'h',
         4: 'i',
         8: 'q',
     }
 
     _signed_sizes = {
-        1: (-0x80, 0x7f),
-        2: (-0x8000, 0x7fff),
-        4: (-0x8000_0000, 0x7fff_ffff),
-        8: (-0x8000_0000_0000_0000, 0x7fff_ffff_ffff_ffff),
+        1: (intsizes.INT8_MIN, intsizes.INT8_MAX),
+        2: (intsizes.INT16_MIN, intsizes.INT16_MAX),
+        4: (intsizes.INT32_MIN, intsizes.INT32_MAX),
+        8: (intsizes.INT64_MIN, intsizes.INT64_MAX),
     }
 
     _unsigned_sizes = {
-        1: (0, 0xff),
-        2: (0, 0xffff),
-        4: (0, 0xffff_ffff),
-        8: (0, 0xffff_ffff_ffff_ffff),
+        1: (intsizes.UINT8_MIN, intsizes.UINT8_MAX),
+        2: (intsizes.UINT16_MIN, intsizes.UINT16_MAX),
+        4: (intsizes.UINT32_MIN, intsizes.UINT32_MAX),
+        8: (intsizes.UINT64_MIN, intsizes.UINT64_MAX),
     }
 
     def __init__(
         self,
         signed: bool,
         size: Literal[1, 2, 4, 8]
     ):
```

### Comparing `dataclasses_struct-0.4.1/dataclasses_struct/types.py` & `dataclasses_struct-0.5.0/dataclasses_struct/types.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.4.1/pyproject.toml` & `dataclasses_struct-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-struct"
-version = "0.4.1"
+version = "0.5.0"
 description = "Converting dataclasses to and from fixed-length binary data using struct"
 authors = ["Harry Mander <harrymander96@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/harrymander/dataclasses-struct"
 repository = "https://github.com/harrymander/dataclasses-struct"
 documentation = "https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage"
```

### Comparing `dataclasses_struct-0.4.1/PKG-INFO` & `dataclasses_struct-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-struct
-Version: 0.4.1
+Version: 0.5.0
 Summary: Converting dataclasses to and from fixed-length binary data using struct
 Home-page: https://github.com/harrymander/dataclasses-struct
 License: MIT
 Author: Harry Mander
 Author-email: harrymander96@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 class Test:
     x: int  # or dcs.UInt64
     y: dcs.Float32
     z: dcs.Uint8
     s: Annotated[bytes, 10]
 ```
 
-```
+```python
 >>> t = Test(100, -0.25, 0xff, b'12345')
 >>> t
 Test(x=100, y=-0.25, z=255, s=b'12345')
 >>> packed = t.pack()
 >>> packed
 b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbe\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
@@ -134,19 +134,19 @@
 
 An additional class attribute, `__dataclass_struct__`, of type
 [`struct.Struct`](https://docs.python.org/3/library/struct.html#struct.Struct)
 is added. The [`struct` format
 string](https://docs.python.org/3/library/struct.html#format-strings) and packed
 size can be accessed like so:
 
-```
+```python
 >>> Test.__dataclass_struct__.format
-'@cc??bBhHiIQqqNnPfdd100s'
+'@cc??bBhHiIQqqNnPfdd100s4xqq2x3xq2x'
 >>> Test.__dataclass_struct__.size
-196
+234
 ```
 
 Default attribute values will be validated against their expected type and
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
```

