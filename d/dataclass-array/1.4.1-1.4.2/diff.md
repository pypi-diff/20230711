# Comparing `tmp/dataclass_array-1.4.1.tar.gz` & `tmp/dataclass_array-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_array-1.4.1.tar", last modified: Mon Mar 20 16:07:41 2023, max compression
+gzip compressed data, was "dataclass_array-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dataclass_array-1.4.1.tar` & `dataclass_array-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/LICENSE
--rw-r--r--   0        0        0     5858 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/README.md
--rw-r--r--   0        0        0     1638 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/__init__.py
--rw-r--r--   0        0        0    38602 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/array_dataclass.py
--rw-r--r--   0        0        0      856 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/conftest.py
--rw-r--r--   0        0        0     2205 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/field_utils.py
--rw-r--r--   0        0        0     2381 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/ops.py
--rw-r--r--   0        0        0      336 2023-03-20 16:07:16.859105 dataclass_array-1.4.1/dataclass_array/shape_grammar.lark
--rw-r--r--   0        0        0     2906 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/shape_parsing.py
--rw-r--r--   0        0        0     2937 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/testing.py
--rw-r--r--   0        0        0     4467 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/type_parsing.py
--rw-r--r--   0        0        0     2146 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/typing.py
--rw-r--r--   0        0        0      804 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/utils/file_utils.py
--rw-r--r--   0        0        0     7295 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/utils/inspect_utils.py
--rw-r--r--   0        0        0     5724 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/utils/np_utils.py
--rw-r--r--   0        0        0      845 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/utils/py_utils.py
--rw-r--r--   0        0        0     2213 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/utils/tree_utils.py
--rw-r--r--   0        0        0    13852 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/dataclass_array/vectorization.py
--rw-r--r--   0        0        0     1702 2023-03-20 16:07:16.863105 dataclass_array-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7126 1970-01-01 00:00:00.000000 dataclass_array-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/LICENSE
+-rw-r--r--   0        0        0     6030 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/README.md
+-rw-r--r--   0        0        0     1696 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/__init__.py
+-rw-r--r--   0        0        0    38577 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/array_dataclass.py
+-rw-r--r--   0        0        0      856 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/conftest.py
+-rw-r--r--   0        0        0     2205 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/field_utils.py
+-rw-r--r--   0        0        0     3720 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/ops.py
+-rw-r--r--   0        0        0      336 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/shape_grammar.lark
+-rw-r--r--   0        0        0     2906 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/shape_parsing.py
+-rw-r--r--   0        0        0     2937 2023-07-11 10:05:55.131347 dataclass_array-1.4.2/dataclass_array/testing.py
+-rw-r--r--   0        0        0     4467 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/type_parsing.py
+-rw-r--r--   0        0        0     2157 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/typing.py
+-rw-r--r--   0        0        0      804 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/file_utils.py
+-rw-r--r--   0        0        0     7295 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/inspect_utils.py
+-rw-r--r--   0        0        0     5792 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/np_utils.py
+-rw-r--r--   0        0        0      845 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/py_utils.py
+-rw-r--r--   0        0        0     2387 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/utils/tree_utils.py
+-rw-r--r--   0        0        0    13852 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/dataclass_array/vectorization.py
+-rw-r--r--   0        0        0     1789 2023-07-11 10:05:55.135347 dataclass_array-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 dataclass_array-1.4.2/PKG-INFO
```

### Comparing `dataclass_array-1.4.1/LICENSE` & `dataclass_array-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_array-1.4.1/README.md` & `dataclass_array-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Dataclass Array
 
-[![Unittests](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml)
+[![Unittests](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/dataclass_array.svg)](https://badge.fury.io/py/dataclass_array)
+[![Documentation Status](https://readthedocs.org/projects/dataclass-array/badge/?version=latest)](https://dataclass-array.readthedocs.io/en/latest/?badge=latest)
+
 
 `DataclassArray` are dataclasses which behave like numpy-like arrays (can be
 batched, reshaped, sliced,...), compatible with Jax, TensorFlow, and numpy (with
 torch support planned).
 
 This reduce boilerplate and improve readability. See the
 [motivating examples](#motivating-examples) section bellow.
```

### Comparing `dataclass_array-1.4.1/dataclass_array/__init__.py` & `dataclass_array-1.4.2/dataclass_array/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,32 +17,33 @@
 Dataclass arrays are dataclasses which can be sliced, indexed, reshaped,... like
 numpy arrays.
 
 """
 
 import sys
 
-# pylint: disable=g-import-not-at-top,g-bad-import-order
+# pylint: disable=g-import-not-at-top,g-bad-import-order,g-importing-member
 
 pytest = sys.modules.get('pytest')
 if pytest:
   # Inside tests, rewrite `assert` statement in `dca.testing` for better
   # debug messages
   pytest.register_assert_rewrite('dataclass_array.testing')
 
 from dataclass_array import typing
 # TODO(epot): Rename array_field -> field internally
 from dataclass_array.array_dataclass import array_field as field
 from dataclass_array.array_dataclass import dataclass_array
 from dataclass_array.array_dataclass import DataclassArray
+from dataclass_array.ops import concat
 from dataclass_array.ops import stack
 from dataclass_array.vectorization import vectorize_method
 
 # `dca.testing` do not depend on pytest or other heavy deps, so is safe to
 # import
 from dataclass_array import testing
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 
 del sys, pytest
```

### Comparing `dataclass_array-1.4.1/dataclass_array/array_dataclass.py` & `dataclass_array-1.4.2/dataclass_array/array_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,28 +21,26 @@
 import typing
 from typing import Any, Callable, ClassVar, Generic, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
 
 from dataclass_array import field_utils
 from dataclass_array import shape_parsing
 from dataclass_array import type_parsing
 from dataclass_array.typing import Array
-from dataclass_array.typing import Axes, DcOrArray, DcOrArrayT, DTypeArg, DynamicShape, Shape  # pylint: disable=g-multiple-import
+from dataclass_array.typing import Axes, DTypeArg, DcOrArray, DcOrArrayT, DynamicShape, Shape  # pylint: disable=g-multiple-import,g-importing-member
 from dataclass_array.utils import np_utils
 from dataclass_array.utils import py_utils
 import einops
 from etils import array_types
 from etils import edc
 from etils import enp
 from etils import epy
 import numpy as np
 import typing_extensions
 from typing_extensions import Annotated, Literal, TypeAlias  # pylint: disable=g-multiple-import
 
-if typing.TYPE_CHECKING:
-  import torch  # pytype: disable=import-error
 
 lazy = enp.lazy
 
 # TODO(pytype): Should use `dca.typing.DcT` but bound does not work across
 # modules.
 _DcT = TypeVar('_DcT', bound='DataclassArray')
 
@@ -148,23 +146,24 @@
 
   # TODO(b/204422756): We cannot use `__class_getitem__` due to b/204422756
   def __getitem__(cls, spec):
     # Not clear how this would interact if cls is also a `Generic`
     return Annotated[cls, field_utils.ShapeAnnotation(spec)]
 
 
-@typing_extensions.dataclass_transform(  # pytype: disable=not-supported-yet
-    kw_only_default=True,
-    # TODO(b/272524683):Restore field specifier
-    # field_specifiers=(
-    #     dataclasses.Field,
-    #     dataclasses.field,
-    #     array_field,
-    # ),
-)
+# TODO(epot): Restore once pytype support this
+# @typing_extensions.dataclass_transform(
+#     kw_only_default=True,
+#     # TODO(b/272524683):Restore field specifier
+#     # field_specifiers=(
+#     #     dataclasses.Field,
+#     #     dataclasses.field,
+#     #     array_field,
+#     # ),
+# )
 class DataclassArray(metaclass=MetaDataclassArray):
   """Dataclass which behaves like an array.
 
   Usage:
 
   ```python
   class Square(DataclassArray):
```

### Comparing `dataclass_array-1.4.1/dataclass_array/conftest.py` & `dataclass_array-1.4.2/dataclass_array/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/field_utils.py` & `dataclass_array-1.4.2/dataclass_array/field_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/shape_parsing.py` & `dataclass_array-1.4.2/dataclass_array/shape_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/testing.py` & `dataclass_array-1.4.2/dataclass_array/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/type_parsing.py` & `dataclass_array-1.4.2/dataclass_array/type_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/typing.py` & `dataclass_array-1.4.2/dataclass_array/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,18 +16,17 @@
 
 from __future__ import annotations
 
 import typing
 from typing import Any, Optional, Tuple, Type, TypeVar, Union
 
 from etils import enp
-from etils.array_types import FloatArray
 
 if typing.TYPE_CHECKING:
-  from dataclass_array import array_dataclass
+  from dataclass_array import array_dataclass  # pylint: disable=g-bad-import-order,unused-import
 
 # ======== Array types (alias of `enp.typing`) ========
 
 ArrayAliasMeta = enp.typing.ArrayAliasMeta
 ArrayLike = enp.typing.ArrayLike
 
 Array = enp.typing.Array
```

### Comparing `dataclass_array-1.4.1/dataclass_array/utils/file_utils.py` & `dataclass_array-1.4.2/dataclass_array/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/utils/inspect_utils.py` & `dataclass_array-1.4.2/dataclass_array/utils/inspect_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/utils/np_utils.py` & `dataclass_array-1.4.2/dataclass_array/utils/np_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -167,15 +167,15 @@
     elif axis < 0:
       return ndim + axis
     else:
       return axis
   elif isinstance(axis, tuple):
     if not all(isinstance(dim, int) for dim in axis):
       raise ValueError(f'Invalid axis={axis}')
-    return tuple(to_absolute_axis(dim, ndim=ndim) for dim in axis)
+    return tuple(to_absolute_axis(dim, ndim=ndim) for dim in axis)  # pytype: disable=bad-return-type  # always-use-return-annotations
   else:
     raise TypeError(f'Unexpected axis type: {type(axis)} {axis}')
 
 
 def to_absolute_einops(shape_pattern: str, *, nlastdim: int) -> str:
   """Convert the einops to absolute."""
   # Nested dataclass might already have shape set.
```

### Comparing `dataclass_array-1.4.1/dataclass_array/utils/py_utils.py` & `dataclass_array-1.4.2/dataclass_array/utils/py_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/dataclass_array/utils/tree_utils.py` & `dataclass_array-1.4.2/dataclass_array/utils/tree_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,22 +18,27 @@
 we need another API which doesn't.
 
 """
 
 from __future__ import annotations
 
 import collections.abc
-from typing import Callable, TypeVar
+from typing import Any, Callable, TypeVar
 
 from etils import epy
-from etils.etree.typing import Tree
-from typing_extensions import Unpack, TypeVarTuple  # pytype: disable=not-supported-yet  # pylint: disable=g-multiple-import
+from etils.etree.typing import Tree  # pylint: disable=g-importing-member
+from typing_extensions import TypeVarTuple, Unpack  # pytype: disable=not-supported-yet  # pylint: disable=g-multiple-import
 
-_InsT = TypeVarTuple('_InsT')
-_OutT = TypeVar('_OutT')
+# TODO(epot): Remove once pytype support `Unpack`
+del TypeVar, TypeVarTuple, Unpack
+Unpack = Any
+TypeVarTuple = Any
+
+_InsT = Any  # TypeVarTuple('_InsT')
+_OutT = Any  # TypeVar('_OutT')
 
 
 def tree_map(  # pylint: disable=redefined-builtin
     fn: Callable[[Unpack[Tree[_InsT]]], _OutT],
     *trees: Unpack[Tree[_InsT]],
 ) -> Tree[_OutT]:
   """Apply a function recursively to each element of a nested data struct.
```

### Comparing `dataclass_array-1.4.1/dataclass_array/vectorization.py` & `dataclass_array-1.4.2/dataclass_array/vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The dataclass_array Authors.
+# Copyright 2023 The dataclass_array Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `dataclass_array-1.4.1/pyproject.toml` & `dataclass_array-1.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "dataclass_array"
 description = "Dataclasses that behave like numpy arrays (with indexing, slicing, vectorization)."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "dataclass_array team", email="dataclass_array@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
@@ -41,14 +41,18 @@
     "pyink",
     # Lazy deps
     "chex",
     "jax[cpu]",
     "tf-nightly",
     "torch",
 ]
+docs = [
+    "sphinx-apitree[ext]",
+    "dataclass_array[dev]",  # Install lazy deps
+]
 
 [tool.pyink]
 # Formatting configuration to follow Google style-guide
 line-length = 80
 preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
```

### Comparing `dataclass_array-1.4.1/PKG-INFO` & `dataclass_array-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dataclass_array
-Version: 1.4.1
+Version: 1.4.2
 Summary: Dataclasses that behave like numpy arrays (with indexing, slicing, vectorization).
 Keywords: dataclass,dataclasses,numpy,jax,tensorflow,array
 Author-email: dataclass_array team <dataclass_array@google.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: einops
@@ -20,22 +20,27 @@
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
 Requires-Dist: pyink ; extra == "dev"
 Requires-Dist: chex ; extra == "dev"
 Requires-Dist: jax[cpu] ; extra == "dev"
 Requires-Dist: tf-nightly ; extra == "dev"
 Requires-Dist: torch ; extra == "dev"
+Requires-Dist: sphinx-apitree[ext] ; extra == "docs"
+Requires-Dist: dataclass_array[dev] ; extra == "docs"
 Project-URL: homepage, https://github.com/google-research/dataclass_array
 Project-URL: repository, https://github.com/google-research/dataclass_array
 Provides-Extra: dev
+Provides-Extra: docs
 
 # Dataclass Array
 
-[![Unittests](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml)
+[![Unittests](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/dataclass_array/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/dataclass_array.svg)](https://badge.fury.io/py/dataclass_array)
+[![Documentation Status](https://readthedocs.org/projects/dataclass-array/badge/?version=latest)](https://dataclass-array.readthedocs.io/en/latest/?badge=latest)
+
 
 `DataclassArray` are dataclasses which behave like numpy-like arrays (can be
 batched, reshaped, sliced,...), compatible with Jax, TensorFlow, and numpy (with
 torch support planned).
 
 This reduce boilerplate and improve readability. See the
 [motivating examples](#motivating-examples) section bellow.
```

