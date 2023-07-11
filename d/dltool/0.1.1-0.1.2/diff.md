# Comparing `tmp/dltool-0.1.1.tar.gz` & `tmp/dltool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltool-0.1.1.tar", last modified: Fri Jun 30 14:10:58 2023, max compression
+gzip compressed data, was "dltool-0.1.2.tar", last modified: Tue Jul 11 16:21:49 2023, max compression
```

## Comparing `dltool-0.1.1.tar` & `dltool-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.244140 dltool-0.1.1/
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-06-09 12:38:00.000000 dltool-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-30 14:10:58.244140 dltool-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      134 2023-06-22 13:04:02.000000 dltool-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.240140 dltool-0.1.1/dltool/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-19 01:34:38.000000 dltool-0.1.1/dltool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1884 2023-02-15 14:06:49.000000 dltool-0.1.1/dltool/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.244140 dltool-0.1.1/dltool/data/
--rw-rw-r--   0 root         (0) root         (0)      174 2023-04-29 04:26:16.000000 dltool-0.1.1/dltool/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6460 2023-06-09 12:38:12.000000 dltool-0.1.1/dltool/data/file.py
--rw-rw-r--   0 root         (0) root         (0)     5828 2023-04-29 04:22:08.000000 dltool-0.1.1/dltool/data/time.py
--rw-rw-r--   0 root         (0) root         (0)      439 2023-04-23 19:43:58.000000 dltool-0.1.1/dltool/data/union.py
--rw-rw-r--   0 root         (0) root         (0)     1268 2023-04-23 19:45:21.000000 dltool-0.1.1/dltool/data/utils.py
--rw-rw-r--   0 root         (0) root         (0)      762 2023-06-30 11:33:17.000000 dltool-0.1.1/dltool/hooks.py
--rw-rw-r--   0 root         (0) root         (0)     9050 2023-06-30 11:46:48.000000 dltool-0.1.1/dltool/log.py
--rw-rw-r--   0 root         (0) root         (0)     4026 2023-06-30 13:41:53.000000 dltool-0.1.1/dltool/train.py
--rw-rw-r--   0 root         (0) root         (0)     1625 2023-06-09 12:38:12.000000 dltool-0.1.1/dltool/types.py
--rw-rw-r--   0 root         (0) root         (0)     4099 2023-04-24 18:33:46.000000 dltool-0.1.1/dltool/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3823 2023-04-23 19:47:14.000000 dltool-0.1.1/dltool/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.240140 dltool-0.1.1/dltool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      729 2023-06-30 10:27:23.000000 dltool-0.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       49 2023-06-28 05:55:31.000000 dltool-0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 14:10:58.244140 dltool-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:21:49.853078 dltool-0.1.2/
+-rw-rw-r--   0 root         (0) root         (0)     1497 2023-06-09 12:38:00.000000 dltool-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-11 16:21:49.849078 dltool-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      148 2023-07-11 16:08:19.000000 dltool-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:21:49.845078 dltool-0.1.2/dltool/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-19 01:34:38.000000 dltool-0.1.2/dltool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1884 2023-02-15 14:06:49.000000 dltool-0.1.2/dltool/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:21:49.845078 dltool-0.1.2/dltool/data/
+-rw-rw-r--   0 root         (0) root         (0)      174 2023-04-29 04:26:16.000000 dltool-0.1.2/dltool/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6460 2023-06-09 12:38:12.000000 dltool-0.1.2/dltool/data/file.py
+-rw-rw-r--   0 root         (0) root         (0)     5836 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/data/time.py
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-04-23 19:43:58.000000 dltool-0.1.2/dltool/data/union.py
+-rw-rw-r--   0 root         (0) root         (0)     1348 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/data/utils.py
+-rw-rw-r--   0 root         (0) root         (0)      775 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)    11871 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/log.py
+-rw-rw-r--   0 root         (0) root         (0)     4019 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/train.py
+-rw-rw-r--   0 root         (0) root         (0)     1629 2023-07-11 16:08:53.000000 dltool-0.1.2/dltool/types.py
+-rw-rw-r--   0 root         (0) root         (0)     5109 2023-07-11 16:08:19.000000 dltool-0.1.2/dltool/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3823 2023-04-23 19:47:14.000000 dltool-0.1.2/dltool/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:21:49.845078 dltool-0.1.2/dltool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-11 16:21:49.000000 dltool-0.1.2/dltool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-11 16:21:49.000000 dltool-0.1.2/dltool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:21:49.000000 dltool-0.1.2/dltool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-11 16:21:49.000000 dltool-0.1.2/dltool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 16:21:49.000000 dltool-0.1.2/dltool.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      729 2023-07-11 16:08:45.000000 dltool-0.1.2/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       49 2023-06-28 05:55:31.000000 dltool-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:21:49.853078 dltool-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:21:49.849078 dltool-0.1.2/tests/
+-rw-rw-r--   0 root         (0) root         (0)     6921 2023-07-11 16:08:19.000000 dltool-0.1.2/tests/test_log.py
+-rw-rw-r--   0 root         (0) root         (0)      590 2023-07-11 16:08:19.000000 dltool-0.1.2/tests/test_utils.py
```

### Comparing `dltool-0.1.1/LICENSE` & `dltool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dltool-0.1.1/PKG-INFO` & `dltool-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small library with handy methods for DL with Pytorch
 Author-email: Artem Mikhaylov <simplerick@yandex.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, simplerick
         
         Redistribution and use in source and binary forms, with or without
@@ -42,9 +42,9 @@
 License-File: LICENSE
 
 # Small library with handy methods for DL with Pytorch
 
 
 # Run unit tests:
 ```
-python -m unittest discover -s tests -p '*_test.py'
+python3 -m pytest -W ignore::Warning  --durations=5  --cov=dltool
 ```
```

### Comparing `dltool-0.1.1/dltool/algorithm.py` & `dltool-0.1.2/dltool/algorithm.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1.1/dltool/data/file.py` & `dltool-0.1.2/dltool/data/file.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1.1/dltool/data/time.py` & `dltool-0.1.2/dltool/data/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             raise IndexError("out of range")
         pos = [(self._t_start + index * self._t_stride + t_i + self._t_delta - 1) // self._t_delta
                for t_i in self._t_edges]
         return pos
 
     def __getitem__(self, index: int) -> list[Sequence] | Sequence:
         if isinstance(index, slice):
-            return NotImplemented
+            raise NotImplementedError
         pos = self._get_index_positions(index)
         seqs = [self.sequence[pos[i]:pos[i + 1]] for i in range(len(pos) - 1)]
         if self.reduce:
             seqs, _ = seqs
         return seqs
 
     def get_dates(self, index: int) -> list[pd.DatetimeIndex] | pd.DatetimeIndex:
@@ -104,15 +104,15 @@
             slices = [s[0] for s in slices]
         if self.reduce_i:
             slices = slices[0]
         return slices
 
     def __getitem__(self, index: int) -> list[Sequence] | Sequence:
         if isinstance(index, slice):
-            return NotImplemented
+            raise NotImplementedError
         slices = [s[index] for s in self.slice_seq]  # [sequences, intervals]
         # transpose
         seqs = [[s[i] for s in slices] for i in range(len(self.intervals))]  # [intervals, sequences]
         # reduce dimensions
         seqs = self._reduce_dimensions(seqs)
         return seqs
```

### Comparing `dltool-0.1.1/dltool/data/utils.py` & `dltool-0.1.2/dltool/data/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,38 +13,30 @@
         try:
             return next(self._iter)
         except (AttributeError, TypeError, StopIteration):
             self._iter = iter(self.dataloader)
             return next(self._iter)
 
 
-def transformable(cls: type):
+def transformable(cls: type) -> type:
     """
-    Modify the class to be able to transform the data. Warning: it modifies the class in place.
-
-    Args:
-        cls: initial class
-
-    Returns:
-        modified class
+    Modifies the given class in-place to enable data transformation.
+    The transformed class will have a `with_transforms` method that attaches a sequence of transforms to the instance.
+    The transforms will be applied to the data returned by the `__getitem__` method of the instance.
     """
-    if hasattr(cls, "_getitem"):
-        raise ValueError("The class already has `_getitem` method. Check if it is already transformable.")
-
     def _with_transforms(self, transforms: Sequence[Callable]):
         self.transforms = transforms
         return self
 
-    cls.with_transforms = _with_transforms
-    cls._getitem = cls.__getitem__
-
     def _getitem(self, *args, **kwargs):
-        x = cls._getitem(self, *args, **kwargs)
-        trfm = getattr(self, "transforms", [])
-        for t in trfm:
-            x = t(x)
+        x = __getitem__(self, *args, **kwargs)
+        if ts := getattr(self, "transforms", None):
+            for t in ts:
+                x = t(x)
         return x
 
-    cls.__getitem__ = _getitem
+    if hasattr(cls, "__getitem__") and not hasattr(cls, "with_transforms"):
+        __getitem__ = cls.__getitem__
+        cls.__getitem__ = _getitem
+        cls.with_transforms = _with_transforms
     return cls
 
-
```

### Comparing `dltool-0.1.1/dltool/hooks.py` & `dltool-0.1.2/dltool/hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import torch
 
 from dltool.utils import cpu_state_dict
 
 
 def watch_best_state_hook(metric: str, select_fn: Callable = min):
     def hook(trainer):
-        metric_values = trainer.logger.history[metric]
-        if len(metric_values) > 0 and select_fn(metric_values) == metric_values[-1]:
-            trainer.best_model_state = cpu_state_dict(trainer.algorithm)
+        if (history := trainer.logger.history) and (metric_values := history[metric]):
+            if select_fn(metric_values) == metric_values[-1]:
+                trainer.best_model_state = cpu_state_dict(trainer.algorithm)
     return hook
 
 
 def save_state_hook(path: str | Path, best: bool = True):
     path = Path(path)
     path.parent.mkdir(parents=True, exist_ok=True)
     def hook(trainer):
```

### Comparing `dltool-0.1.1/dltool/train.py` & `dltool-0.1.2/dltool/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 with evaluating(self.algorithm):
                     self.loop(len(val_dataloader), val_iterator, self.algorithm.val_step)
             # hooks
             try:
                 for fn in self.hooks:
                     fn(self)
             except StopSignal as e:  # allows to stop training from hook
-                self.logger.console_logger.info(f"{e.__class__.__name__}: {e}" if e.args else f"{e.__class__.__name__}")
+                self.logger.console.info(f"{e.__class__.__name__}: {e}" if e.args else f"{e.__class__.__name__}")
                 break
         # load best model if any is saved
         if self.best_model_state is not None:
             self.algorithm.load_state_dict(self.best_model_state)
 
     def test(self, test_dataloader):
         # data iterator
```

### Comparing `dltool-0.1.1/dltool/types.py` & `dltool-0.1.2/dltool/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,13 +35,13 @@
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
         if (not all(issubclass(t, TensorDict) for t in types)
                 or func not in [torch.cat, torch.stack]):
-            return NotImplemented
+            raise NotImplementedError
         td = next(iter(next(iter(args))))
         ttypes = [torch.Tensor] * len(args)
         new = {k: torch.Tensor.__torch_function__(func, ttypes, [[x[k] for x in a] for a in args], kwargs)
                for k in td.keys()}
         return TensorDict.convert(new)
```

### Comparing `dltool-0.1.1/dltool/utils.py` & `dltool-0.1.2/dltool/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections.abc import Callable
 import torch
 from contextlib import contextmanager
+import re
 
 
 class FuncModule(torch.nn.Module):
+    """Torch module from function"""
     def __init__(self, func: Callable):
         super().__init__()
         self.forward = func
 
     def __repr__(self):
         return f"FuncModule({self.forward.__name__})"
 
@@ -24,15 +26,15 @@
 
     Returns:
         Resulting object, note that it is not necessarily a copy of the original object
     """
     if hasattr(obj, func_str):
         obj = getattr(obj, func_str)(**args)
     else:
-        if isinstance(obj, list):
+        if isinstance(obj, (list, tuple)):
             obj[:] = [apply(x, func_str, **args) for x in obj]
         if isinstance(obj, dict):
             for k in obj:
                 obj[k] = apply(obj[k], func_str, **args)
     return obj
 
 
@@ -77,15 +79,15 @@
     """
     return to(model.state_dict(), device='cpu')
 
 
 def cartesian_prod(*tensors: torch.Tensor) -> torch.Tensor:
     """
     Cartesian product of tensors. The same as torch.cartesian_prod but works with 0D, 1D and 2D tensors and returns 2D tensor.
-    If tensor is 2D, its rows are considered as one-piece elements of product, i.e. concated to the rows of the result cartesian product.
+    If tensor is 2D, its rows are considered as one-piece elements of product, i.e. concatenated to the rows of the result cartesian product.
 
     Example:
         a = torch.tensor([[1, 2], [3, 4]])
         b = torch.tensor([[5, 6], [7, 8]])
         cartesian_prod(a, b) = torch.tensor([[1, 2, 5, 6], [1, 2, 7, 8], [3, 4, 5, 6], [3, 4, 7, 8]])
 
     Args:
@@ -109,15 +111,14 @@
         view_shape[i] = 1
         grids.append(grid)
     prod = torch.cat(grids, dim=-1)
     prod = prod.view(-1, prod.shape[-1])
     return prod
 
 
-# context manager for evaluating
 @contextmanager
 def evaluating(model: torch.nn.Module):
     """
     Context-manager that temporarily switches the model to evaluation mode. Restores the initial training state of each submodule on exit.
 
     Args:
         model: torch module
@@ -128,7 +129,38 @@
         try:
             model.eval()
             yield model
         finally:
             # restore initial training state
             for k, v in train_state.items():
                 k.training = v
+
+
+def flatten_dict(d: dict, sep: str = "."):
+    """
+    Flatten a nested dictionary to a dictionary with keys like "a.b.c".
+    """
+    flattened_d = {}
+    for k, v in d.items():
+        if isinstance(v, dict):
+            flattened_v = flatten_dict(v, sep)
+            for k2, v2 in flattened_v.items():
+                flattened_d[f"{k}{sep}{k2}"] = v2
+        else:
+            flattened_d[k] = v
+    return flattened_d
+
+
+def unflatten_dict(d: dict, sep: str = ".", regex: bool = False):
+    """
+    Unflatten a dictionary with keys like "a.b.c" to a nested dictionary. Supports regex separators.
+    """
+    unflattened_d = {}
+    for k, v in d.items():
+        k_lvls = re.split(sep, k) if regex else k.split(sep)
+        cur_d = unflattened_d
+        for l in k_lvls[:-1]:
+            if l not in cur_d:
+                cur_d[l] = {}
+            cur_d = cur_d[l]
+        cur_d[k_lvls[-1]] = unflatten_dict(v, sep, regex) if isinstance(v, dict) else v
+    return unflattened_d
```

### Comparing `dltool-0.1.1/dltool/visualize.py` & `dltool-0.1.2/dltool/visualize.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1.1/dltool.egg-info/PKG-INFO` & `dltool-0.1.2/dltool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small library with handy methods for DL with Pytorch
 Author-email: Artem Mikhaylov <simplerick@yandex.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, simplerick
         
         Redistribution and use in source and binary forms, with or without
@@ -42,9 +42,9 @@
 License-File: LICENSE
 
 # Small library with handy methods for DL with Pytorch
 
 
 # Run unit tests:
 ```
-python -m unittest discover -s tests -p '*_test.py'
+python3 -m pytest -W ignore::Warning  --durations=5  --cov=dltool
 ```
```

### Comparing `dltool-0.1.1/pyproject.toml` & `dltool-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dltool"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Artem Mikhaylov", email="simplerick@yandex.com" },
 ]
 description = "A small library with handy methods for DL with Pytorch"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

