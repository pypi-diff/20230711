# Comparing `tmp/xarray-einstats-0.5.1.tar.gz` & `tmp/xarray_einstats-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-einstats-0.5.1.tar", last modified: Fri Jan 20 12:32:05 2023, max compression
+gzip compressed data, was "xarray_einstats-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xarray-einstats-0.5.1.tar` & `xarray_einstats-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11485 2023-01-20 12:31:58.140462 xarray-einstats-0.5.1/LICENSE
--rw-r--r--   0        0        0     3776 2023-01-20 12:31:58.140462 xarray-einstats-0.5.1/README.md
--rw-r--r--   0        0        0     2308 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5243 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/__init__.py
--rw-r--r--   0        0        0    16675 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/einops.py
--rw-r--r--   0        0        0    23614 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/linalg.py
--rw-r--r--   0        0        0     9637 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/numba.py
--rw-r--r--   0        0        0       27 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/py.typed
--rw-r--r--   0        0        0    22340 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/stats.py
--rw-r--r--   0        0        0     2297 2023-01-20 12:31:58.164462 xarray-einstats-0.5.1/src/xarray_einstats/tutorial.py
--rw-r--r--   0        0        0     5721 1970-01-01 00:00:00.000000 xarray-einstats-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11485 2023-07-10 23:05:54.163406 xarray_einstats-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3776 2023-07-10 23:05:54.163406 xarray_einstats-0.6.0/README.md
+-rw-r--r--   0        0        0     2313 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5341 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/__init__.py
+-rw-r--r--   0        0        0     5496 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/accessors.py
+-rw-r--r--   0        0        0    19748 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/einops.py
+-rw-r--r--   0        0        0    24481 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/linalg.py
+-rw-r--r--   0        0        0    10185 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/numba.py
+-rw-r--r--   0        0        0       27 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/py.typed
+-rw-r--r--   0        0        0    22364 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/stats.py
+-rw-r--r--   0        0        0     3505 2023-07-10 23:05:54.187406 xarray_einstats-0.6.0/src/xarray_einstats/tutorial.py
+-rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 xarray_einstats-0.6.0/PKG-INFO
```

### Comparing `xarray-einstats-0.5.1/LICENSE` & `xarray_einstats-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-einstats-0.5.1/README.md` & `xarray_einstats-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xarray-einstats-0.5.1/pyproject.toml` & `xarray_einstats-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "xarray-einstats"
 description = "Stats, linear algebra and einops for xarray"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "ArviZ team", email = "arviz.devs@gmail.com"}
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
-  "numpy>=1.20",
-  "scipy>=1.6",
+  "numpy>=1.21",
+  "scipy>=1.7",
   "xarray>=2022.09.0",
 ]
 
 [tool.flit.module]
 name = "xarray_einstats"
 
 [tool.setuptools.dynamic]
@@ -60,14 +59,15 @@
     "sphinx-copybutton",
     "numpydoc",
     "sphinx>=4",
     "jupyter-sphinx",
     "sphinx-design",
     "watermark",
     "matplotlib",
+    "sphinx-togglebutton",
 ]
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
@@ -85,14 +85,15 @@
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.run]
 source = ["xarray_einstats"]
+omit = ["tutorial.py"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
```

### Comparing `xarray-einstats-0.5.1/src/xarray_einstats/__init__.py` & `xarray_einstats-0.6.0/src/xarray_einstats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 """Stats, linear algebra and einops for xarray."""
 
 from __future__ import annotations
 
 import numpy as np
 import xarray as xr
 
-from .linalg import einsum, raw_einsum, einsum_path, matmul
+from .linalg import einsum, einsum_path, matmul
+from .accessors import LinAlgAccessor, EinopsAccessor
 
-__all__ = ["einsum", "raw_einsum", "einsum_path", "matmul", "zeros_ref", "ones_ref", "empty_ref"]
+__all__ = [
+    "einsum",
+    "einsum_path",
+    "matmul",
+    "zeros_ref",
+    "ones_ref",
+    "empty_ref",
+    "LinAlgAccessor",
+    "EinopsAccessor",
+]
 
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 
 def sort(da, dim, **kwargs):
     """Sort along dimension using DataArray values."""
-    sort_kwargs = dict(axis=-1)
+    sort_kwargs = {"axis": -1}
     if "kind" in kwargs:
         sort_kwargs["kind"] = kwargs.pop("kind")
     return xr.apply_ufunc(
         np.sort,
         da,
         input_core_dims=[[dim]],
         output_core_dims=[[dim]],
```

### Comparing `xarray-einstats-0.5.1/src/xarray_einstats/linalg.py` & `xarray_einstats-0.6.0/src/xarray_einstats/linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-"""Wrappers for :mod:`numpy.linalg`."""
+"""Wrappers for :mod:`numpy.linalg`.
+
+.. tip::
+
+    Most of the functions in this module are also available via the ``.linalg`` accessor
+    from :class:`DataArray` objects. See :ref:`linalg_tutorial` for
+    example usage.
+
+    The functions that are not available via the accessor are ``einsum``, ``einsum_path``,
+    ``matmul`` and ``get_default_dims``.
+
+"""
+import warnings
+
 import numpy as np
 import xarray as xr
 
 __all__ = [
     "matrix_power",
     "matrix_transpose",
     "cholesky",
@@ -200,32 +213,38 @@
         out_subscript = "->" + "".join(handler.dim_map[dim] for dim in out_dims)
     if out_subscript and "..." in in_subscript:
         out_subscript = "->..." + out_subscript[2:]
     subscripts = in_subscript + out_subscript
     return subscripts, updated_in_dims, out_dims
 
 
-def einsum_path(dims, *operands, keep_dims=frozenset(), optimize=None, **kwargs):
-    """Wrap :func:`numpy.einsum_path`.
+def _translate_pattern_string(subscripts):
+    """Translate a pattern given as string of dimension names to list of dimension names."""
+    if "->" in subscripts:
+        in_subscripts, out_subscript = subscripts.split("->")
+    else:
+        in_subscripts = subscripts
+        out_subscript = None
+    in_dims = [
+        [dim.strip(", ") for dim in in_subscript.split(" ")]
+        for in_subscript in in_subscripts.split(",")
+    ]
+    if out_subscript is None:
+        dims = in_dims
+    elif not out_subscript:
+        dims = [*in_dims, []]
+    else:
+        out_dims = [dim.strip(", ") for dim in out_subscript.split(" ")]
+        dims = [*in_dims, out_dims]
+    return dims
 
-    See :func:`xarray_einstats.einsum` for a detailed description of ``dims``
-    and ``operands``.
 
-    Parameters
-    ----------
-    dims : list of list of str
-    operands : DataArray
-    optimize : str, optional
-        ``optimize`` argument for :func:`numpy.einsum_path`. It defaults to None so that
-        we always default to numpy's default, without needing to keep the call signature
-        here up to date.
-    kwargs : dict, optional
-        Passed to :func:`xarray.apply_ufunc`
-    """
-    op_kwargs = {} if optimize is None else dict(optimize=optimize)
+def _einsum_path(dims, *operands, keep_dims=frozenset(), optimize=None, **kwargs):
+    """Wrap :func:`numpy.einsum_path` directly."""
+    op_kwargs = {} if optimize is None else {"optimize": optimize}
 
     subscripts, in_dims, _ = _einsum_parent(dims, *operands, keep_dims=keep_dims)
     updated_in_dims = []
     for sublist, da in zip(in_dims, operands):
         updated_in_dims.append([dim for dim in da.dims if dim not in sublist] + sublist)
 
     return xr.apply_ufunc(
@@ -235,52 +254,40 @@
         input_core_dims=[[], *updated_in_dims],
         output_core_dims=[[]],
         kwargs=op_kwargs,
         **kwargs,
     ).values.item()
 
 
-def einsum(dims, *operands, keep_dims=frozenset(), out_append="{i}", einsum_kwargs=None, **kwargs):
-    """Preprocess inputs to call :func:`numpy.einsum` or :func:`numpy.einsum_path`.
+def einsum_path(dims, *operands, keep_dims=frozenset(), optimize=None, **kwargs):
+    """Expose :func:`numpy.einsum_path` with an xarray-like API.
 
-    Usage examples of all arguments is available at the
-    :ref:`einsum section <linalg_tutorial/einsum>` of the linear algebra module tutorial.
+    See :func:`xarray_einstats.einsum` for a detailed description of ``dims``
+    and ``operands``.
 
     Parameters
     ----------
     dims : list of list of str
-        List of lists of dimension names. It must have the same length or be
-        only one item longer than ``operands``. If both have the same
-        length, the generated pattern passed to {func}`numpy.einsum`
-        won't have ``->`` nor right hand side. Otherwise, the last
-        item is assumed to be the dimension specification of the output
-        DataArray, and it can be an empty list to add ``->`` but no
-        subscripts.
     operands : DataArray
-        DataArrays for the operation. Multiple DataArrays are accepted.
-    keep_dims : set, optional
-        Dimensions to exclude from summation unless specifically specified in ``dims``
-    out_append : str, optional
-        Pattern to append to repeated dimension names in the output (if any). The pattern should
-        contain a substitution for variable ``i``, which indicates the number of the current
-        dimension among the repeated ones. Its default value is ``"{i}"``.
-        To keep repeated dimension names use ``""``.
-
-        The first occurrence will keep the original name and not use ``out_append``.
-        It will therefore inherit the coordinate values in case there were any.
-    einsum_kwargs : dict, optional
-        Passed to :func:`numpy.einsum`
+    optimize : str, optional
+        ``optimize`` argument for :func:`numpy.einsum_path`. It defaults to None so that
+        we always default to numpy's default, without needing to keep the call signature
+        here up to date.
     kwargs : dict, optional
         Passed to :func:`xarray.apply_ufunc`
+    """
+    if isinstance(dims, str):
+        dims = _translate_pattern_string(dims)
+    return _einsum_path(dims, *operands, keep_dims=keep_dims, optimize=optimize, **kwargs)
 
-    Notes
-    -----
-    Dimensions present in ``dims`` will be reduced, but unlike {func}`xarray.dot` it does so only
-    for that variable.
 
+def _einsum(dims, *operands, keep_dims=frozenset(), out_append="{i}", einsum_kwargs=None, **kwargs):
+    """Wrap :func:`numpy.einsum` directly.
+
+    The user facing version is :func:`xarray_einstats.einsum` which exposes two APIs.
     """
     if einsum_kwargs is None:
         einsum_kwargs = {}
 
     subscripts, updated_in_dims, out_dims = _einsum_parent(dims, *operands, keep_dims=keep_dims)
 
     updated_out_dims = []
@@ -297,55 +304,72 @@
         input_core_dims=[[], *updated_in_dims],
         output_core_dims=[updated_out_dims],
         kwargs=einsum_kwargs,
         **kwargs,
     )
 
 
-def raw_einsum(
-    subscripts, *operands, keep_dims=frozenset(), out_append="{i}", einsum_kwargs=None, **kwargs
-):
-    """Wrap :func:`numpy.einsum` crudely.
+def raw_einsum(*args, **kwargs):
+    """Wrap numpy.einsum.
+
+    DEPRECATED
+    """
+    warnings.warn(
+        "`raw_einsum` has been deprecated. Its functionality has been merged into `einsum`",
+        DeprecationWarning,
+    )
+    return einsum(*args, **kwargs)
+
+
+def einsum(dims, *operands, keep_dims=frozenset(), out_append="{i}", einsum_kwargs=None, **kwargs):
+    """Expose :func:`numpy.einsum` with an xarray-like API.
 
     Usage examples of all arguments is available at the
     :ref:`einsum section <linalg_tutorial/einsum>` of the linear algebra module tutorial.
 
-    The description of all the arguments except `subscripts` is available at
-    :func:`xarray_einstats.einsum`.
-
     Parameters
     ----------
-    subscripts : str
-        Specify the subscripts for the summation as dimension names. Spaces indicate
-        multiple dimensions in a DataArray and commas indicate multiple DataArray
-        operands. Only dimensions with no spaces, nor commas nor ``->`` characters
-        are valid.
+    dims : str or list of list of str
+        If `dims` is a string it is intepreted as the subscripts for the summation as dimension
+        names. Spaces indicate multiple dimensions in a DataArray and commas indicate
+        multiple DataArray operands.
+        Only dimensions with no spaces, nor commas nor ``->`` characters are valid.
+
+        If `dims` is a list it is interpreted as list of lists of dimension names.
+        It must have the same length or be only one item longer than `operands`.
+        If both have the same length, the generated pattern passed to {func}`numpy.einsum`
+        won't have ``->`` nor right hand side. Otherwise, the last
+        item is assumed to be the dimension specification of the output
+        DataArray. In this case it can be an empty list to add ``->`` but no
+        subscripts.
     operands : DataArray
+        DataArrays for the operation. Multiple DataArrays are accepted.
     keep_dims : set, optional
+        Dimensions to exclude from summation unless specifically specified in ``dims``
     out_append : str, optional
+        Pattern to append to repeated dimension names in the output (if any). The pattern should
+        contain a substitution for variable ``i``, which indicates the number of the current
+        dimension among the repeated ones. Its default value is ``"{i}"``.
+        To keep repeated dimension names use ``""``.
+
+        The first occurrence will keep the original name and not use ``out_append``.
+        It will therefore inherit the coordinate values in case there were any.
     einsum_kwargs : dict, optional
-    kwargs : optional
+        Passed to :func:`numpy.einsum`
+    kwargs : dict, optional
+        Passed to :func:`xarray.apply_ufunc`
+
+    Notes
+    -----
+    Dimensions present in ``dims`` will be reduced, but unlike {func}`xarray.dot` it does so only
+    for that variable.
     """
-    if "->" in subscripts:
-        in_subscripts, out_subscript = subscripts.split("->")
-    else:
-        in_subscripts = subscripts
-        out_subscript = None
-    in_dims = [
-        [dim.strip(", ") for dim in in_subscript.split(" ")]
-        for in_subscript in in_subscripts.split(",")
-    ]
-    if out_subscript is None:
-        dims = in_dims
-    elif not out_subscript:
-        dims = [*in_dims, []]
-    else:
-        out_dims = [dim.strip(", ") for dim in out_subscript.split(" ")]
-        dims = [*in_dims, out_dims]
-    return einsum(
+    if isinstance(dims, str):
+        dims = _translate_pattern_string(dims)
+    return _einsum(
         dims,
         *operands,
         keep_dims=keep_dims,
         out_append=out_append,
         einsum_kwargs=einsum_kwargs,
         **kwargs,
     )
@@ -480,15 +504,15 @@
         raise ValueError("mode not recognized")
 
     return xr.apply_ufunc(
         np.linalg.qr,
         da,
         input_core_dims=[dims],
         output_core_dims=out_dims,
-        kwargs=dict(mode=mode),
+        kwargs={"mode": mode},
         **kwargs,
     )
 
 
 def svd(
     da, dims=None, *, full_matrices=True, compute_uv=True, hermitian=False, out_append="2", **kwargs
 ):
@@ -517,15 +541,15 @@
     else:
         out_dims = [s_dims]
     return xr.apply_ufunc(
         np.linalg.svd,
         da,
         input_core_dims=[dims],
         output_core_dims=out_dims,
-        kwargs=dict(full_matrices=full_matrices, compute_uv=compute_uv, hermitian=hermitian),
+        kwargs={"full_matrices": full_matrices, "compute_uv": compute_uv, "hermitian": hermitian},
         **kwargs,
     )
 
 
 def eig(da, dims=None, **kwargs):
     """Wrap :func:`numpy.linalg.eig`.
 
@@ -546,15 +570,15 @@
     if dims is None:
         dims = _attempt_default_dims("eigh", da.dims)
     return xr.apply_ufunc(
         np.linalg.eigh,
         da,
         input_core_dims=[dims],
         output_core_dims=[dims[-1:], dims],
-        kwargs=dict(UPLO=UPLO),
+        kwargs={"UPLO": UPLO},
         **kwargs,
     )
 
 
 def eigvals(da, dims=None, **kwargs):
     """Wrap :func:`numpy.linalg.eigvals`.
 
@@ -575,15 +599,15 @@
     if dims is None:
         dims = _attempt_default_dims("eigvalsh", da.dims)
     return xr.apply_ufunc(
         np.linalg.eigvalsh,
         da,
         input_core_dims=[dims],
         output_core_dims=[dims[-1:]],
-        kwargs=dict(UPLO=UPLO),
+        kwargs={"UPLO": UPLO},
         **kwargs,
     )
 
 
 def norm(da, dims=None, *, ord=None, **kwargs):  # pylint: disable=redefined-builtin
     """Wrap :func:`numpy.linalg.norm`.
 
@@ -606,15 +630,15 @@
 def cond(da, dims=None, *, p=None, **kwargs):  # pylint: disable=invalid-name
     """Wrap :func:`numpy.linalg.cond`.
 
     Usage examples of all arguments is available at the :ref:`linalg_tutorial` page.
     """
     if dims is None:
         dims = _attempt_default_dims("cond", da.dims)
-    return xr.apply_ufunc(np.linalg.cond, da, input_core_dims=[dims], kwargs=dict(p=p), **kwargs)
+    return xr.apply_ufunc(np.linalg.cond, da, input_core_dims=[dims], kwargs={"p": p}, **kwargs)
 
 
 def det(da, dims=None, **kwargs):
     """Wrap :func:`numpy.linalg.det`.
 
     Usage examples of all arguments is available at the :ref:`linalg_tutorial` page.
     """
@@ -630,15 +654,15 @@
     """
     if dims is None:
         dims = _attempt_default_dims("matrix_rank", da.dims)
     return xr.apply_ufunc(
         np.linalg.matrix_rank,
         da,
         input_core_dims=[dims],
-        kwargs=dict(tol=tol, hermitian=hermitian),
+        kwargs={"tol": tol, "hermitian": hermitian},
         **kwargs,
     )
 
 
 def slogdet(da, dims=None, **kwargs):
     """Wrap :func:`numpy.linalg.slogdet`.
 
@@ -654,26 +678,26 @@
 def trace(da, dims=None, *, offset=0, dtype=None, out=None, **kwargs):
     """Wrap :func:`numpy.trace`.
 
     Usage examples of all arguments is available at the :ref:`linalg_tutorial` page.
     """
     if dims is None:
         dims = _attempt_default_dims("trace", da.dims)
-    trace_kwargs = dict(offset=offset, dtype=dtype, out=out, axis1=-2, axis2=-1)
+    trace_kwargs = {"offset": offset, "dtype": dtype, "out": out, "axis1": -2, "axis2": -1}
     return xr.apply_ufunc(np.trace, da, input_core_dims=[dims], kwargs=trace_kwargs, **kwargs)
 
 
 def diagonal(da, dims=None, *, offset=0, **kwargs):
     """Wrap :func:`numpy.diagonal`.
 
     Usage examples of all arguments is available at the :ref:`linalg_tutorial` page.
     """
     if dims is None:
         dims = _attempt_default_dims("diagonal", da.dims)
-    diagonal_kwargs = dict(offset=offset, axis1=-2, axis2=-1)
+    diagonal_kwargs = {"offset": offset, "axis1": -2, "axis2": -1}
     out_dims = [dims[0] if offset == 0 else "diag_id"]
     return xr.apply_ufunc(
         np.diagonal,
         da,
         input_core_dims=[dims],
         output_core_dims=[out_dims],
         kwargs=diagonal_kwargs,
```

### Comparing `xarray-einstats-0.5.1/src/xarray_einstats/numba.py` & `xarray_einstats-0.6.0/src/xarray_einstats/numba.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,54 +218,63 @@
         block defined by `dims`.
     **kwargs : dict, optional
         Keyword arguments passed as-is to :func:`xarray.apply_ufunc` through
         :func:`~xarray_einstats.numba.searchsorted`.
 
     Returns
     -------
-    Dataset
-        Dataset with two data variables: ``x`` and ``y`` with the values to plot.
+    DataArray
+        DataArray with the computed values. It reduces the dimensions
+        provided as `dims` and adds the dimensions ``quantile`` and ``ecdf_axis``.
 
     Examples
     --------
     Compute and plot the ecdf over all the data:
 
     .. plot::
        :context: close-figs
 
         from xarray_einstats import tutorial, numba
         import matplotlib.pyplot as plt
 
         ds = tutorial.generate_mcmc_like_dataset(3)
         out = numba.ecdf(ds["mu"], dims=("chain", "draw", "team"))
-        plt.plot(out["x"], out["y"], drawstyle="steps-post");
+        plt.plot(out.sel(ecdf_axis="x"), out.sel(ecdf_axis="y"), drawstyle="steps-post");
 
     Compute vectorized ecdf values to plot multiple subplots and
     multiple lines in each with different hue:
 
     .. plot::
        :context: close-figs
 
         out = numba.ecdf(ds["mu"], dims="draw")
-        out["y"].assign_coords(x=out["x"]).plot.line(
+        out.sel(ecdf_axis="y").assign_coords(x=out.sel(ecdf_axis="x")).plot.line(
             x="x", hue="chain", col="team", col_wrap=3, drawstyle="steps-post"
         );
 
     Warnings
     --------
     New and experimental feature, its API might change.
 
+    Notes
+    -----
+    There are two main reasons for returning a DataArray even if operations
+    do not happen in any vectorized way on the ``ecdf_axis`` dimension.
+    One is that this is more coherent with xarray in aiming to be idempotent.
+    The input is a single DataArray, so the output should be too.
+    The second is that this allows using it with `Dataset.map`.
+
     """
     if dims is None:
         dims = da.dims
     elif isinstance(dims, str):
         dims = [dims]
     total_points = np.product([da.sizes[d] for d in dims])
     if npoints is None:
         npoints = min(total_points, 200)
     x = xr.DataArray(np.linspace(0, 1, npoints), dims=["quantile"])
     max_da = da.max(dims)
     min_da = da.min(dims)
     x = (max_da - min_da) * x + min_da
 
     y = searchsorted(da, x, dims=dims, **kwargs) / total_points
-    return xr.Dataset({"x": x, "y": y})
+    return xr.concat((x, y), dim="ecdf_axis").assign_coords(ecdf_axis=["x", "y"])
```

### Comparing `xarray-einstats-0.5.1/src/xarray_einstats/stats.py` & `xarray_einstats-0.6.0/src/xarray_einstats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,16 @@
             f"Method wrapping :meth:`scipy.stats.{wrapped_cls}.{method_name}` "
             "with :func:`xarray.apply_ufunc`\n\nUsage examples available at "
             f":ref:`stats_tutorial/dists`.\n\n{extra_doc}",
         )
         setattr(cls, method_name, method)
 
 
-doc_extras = dict(
-    rvs="""
+doc_extras = {
+    "rvs": """
 Parameters
 ----------
 args : scalar or array_like, optional
     Passed to the scipy distribution after broadcasting.
 size : int of sequence of ints, optional
     The number of samples to draw *per array element*. If the distribution
     parameters broadcast to a ``(4, 10, 6)`` shape and ``size=(5, 3)`` then
@@ -312,15 +312,15 @@
     Dimension names for the dimensions created due to ``size``. If present
     it must have the same length as ``size``.
 apply_kwargs : dict, optional
     Passed to :func:`xarray.apply_ufunc`
 kwargs : dict, optional
     Passed to the scipy distribution after broadcasting using the same key.
 """
-)
+}
 base_methods = ["cdf", "logcdf", "sf", "logsf", "ppf", "isf", "rvs"]
 _add_documented_method(XrRV, "rv_generic", base_methods, doc_extras)
 _add_documented_method(
     XrContinuousRV, "rv_continuous", base_methods + ["pdf", "logpdf"], doc_extras
 )
 _add_documented_method(XrDiscreteRV, "rv_discrete", base_methods + ["pmf", "logpmf"], doc_extras)
 
@@ -488,59 +488,59 @@
 
 
 def circmean(da, dims=None, *, high=2 * np.pi, low=0, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.circmean`.
 
     Usage examples available at :ref:`stats_tutorial`
     """
-    circmean_kwargs = dict(axis=-1, high=high, low=low)
+    circmean_kwargs = {"axis": -1, "high": high, "low": low}
     if nan_policy is not None:
         circmean_kwargs["nan_policy"] = nan_policy
     return _apply_reduce_func(stats.circmean, da, dims, kwargs, circmean_kwargs)
 
 
 def circvar(da, dims=None, *, high=2 * np.pi, low=0, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.circvar`.
 
     Usage examples available at :ref:`stats_tutorial`
     """
-    circvar_kwargs = dict(axis=-1, high=high, low=low)
+    circvar_kwargs = {"axis": -1, "high": high, "low": low}
     if nan_policy is not None:
         circvar_kwargs["nan_policy"] = nan_policy
     return _apply_reduce_func(stats.circvar, da, dims, kwargs, circvar_kwargs)
 
 
 def circstd(da, dims=None, *, high=2 * np.pi, low=0, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.circstd`.
 
     Usage examples available at :ref:`stats_tutorial`
     """
-    circstd_kwargs = dict(axis=-1, high=high, low=low)
+    circstd_kwargs = {"axis": -1, "high": high, "low": low}
     if nan_policy is not None:
         circstd_kwargs["nan_policy"] = nan_policy
     return _apply_reduce_func(stats.circstd, da, dims, kwargs, circstd_kwargs)
 
 
 def kurtosis(da, dims=None, *, fisher=True, bias=True, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.kurtosis`.
 
     Usage examples available at :ref:`stats_tutorial`
     """
-    kurtosis_kwargs = dict(axis=-1, fisher=fisher, bias=bias)
+    kurtosis_kwargs = {"axis": -1, "fisher": fisher, "bias": bias}
     if nan_policy is not None:
         kurtosis_kwargs["nan_policy"] = nan_policy
     return _apply_reduce_func(stats.kurtosis, da, dims, kwargs, kurtosis_kwargs)
 
 
 def skew(da, dims=None, *, bias=True, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.skew`.
 
     Usage examples available at :ref:`stats_tutorial`
     """
-    skew_kwargs = dict(axis=-1, bias=bias)
+    skew_kwargs = {"axis": -1, "bias": bias}
     if nan_policy is not None:
         skew_kwargs["nan_policy"] = nan_policy
     return _apply_reduce_func(stats.skew, da, dims, kwargs, skew_kwargs)
 
 
 def logsumexp(da, dims=None, *, b=True, return_sign=False, **kwargs):
     """Wrap and extend :func:`scipy.special.logsumexp`.
@@ -571,25 +571,25 @@
     try:
         return xr.apply_ufunc(
             lambda a, b, **kwargs: special.logsumexp(a, b=b, **kwargs),
             da,
             b,
             input_core_dims=[b_dims_to_keep + core_dims, b_dims_to_keep + b_dims],
             output_core_dims=out_dims,
-            kwargs=dict(return_sign=return_sign, axis=axis),
+            kwargs={"return_sign": return_sign, "axis": axis},
             **kwargs,
         )
     except ValueError:
         out_dims[0] = []
         return xr.apply_ufunc(
             lambda a, b, **kwargs: special.logsumexp(a, b=b, **kwargs),
             *xr.broadcast(da, b),
             input_core_dims=[core_dims, core_dims],
             output_core_dims=out_dims,
-            kwargs=dict(return_sign=return_sign, axis=axis),
+            kwargs={"return_sign": return_sign, "axis": axis},
             **kwargs,
         )
 
 
 def median_abs_deviation(da, dims=None, *, center=None, scale=1, nan_policy=None, **kwargs):
     """Wrap and extend :func:`scipy.stats.median_abs_deviation`.
 
@@ -619,15 +619,15 @@
     .. jupyter-execute::
         :raises: ValueError
 
         from scipy import stats
         stats.median_abs_deviation(ds["mu"], axis=1, scale=s_da)
 
     """
-    mad_kwargs = dict(axis=-1)
+    mad_kwargs = {"axis": -1}
     if center is not None:
         mad_kwargs["center"] = center
     if nan_policy is not None:
         mad_kwargs["nan_policy"] = nan_policy
 
     if dims is None:
         dims = get_default_dims(da.dims)
```

### Comparing `xarray-einstats-0.5.1/src/xarray_einstats/tutorial.py` & `xarray_einstats-0.6.0/src/xarray_einstats/tutorial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 """Tutorial module with data for docs and quick testing."""
 import numpy as np
 import xarray as xr
 
+try:
+    from IPython import get_ipython
+    from PIL.Image import fromarray
+
+    array_display = True  # pylint: disable=invalid-name
+except ModuleNotFoundError:
+    array_display = False  # pylint: disable=invalid-name
+
 
 def generate_mcmc_like_dataset(seed=None):
     """Generate a Dataset with multiple variables, some with dimensions from mcmc sampling.
 
     Parameters
     ----------
     seed : int or sequence of int, optional
@@ -66,7 +74,33 @@
 
     """
     xr.set_options(display_expand_data=False)
     rng = np.random.default_rng(seed)
     return xr.DataArray(
         rng.exponential(size=(10, 3, 4, 4)), dims=["batch", "experiment", "dim", "dim2"]
     )
+
+
+if array_display:
+
+    def display_np_arrays_as_images():
+        """Display numpy arrays as images by default in IPython and Jupyter.
+
+        Only needs to be imported for the behaviour to be configured.
+        """
+        # pylint: disable=protected-access
+
+        def np_to_png(a):
+            if 2 <= len(a.shape) <= 3:
+                return fromarray(np.array(np.clip(a, 0, 1) * 255, dtype="uint8"))._repr_png_()
+            return fromarray(np.zeros([1, 1], dtype="uint8"))._repr_png_()
+
+        def np_to_text(obj, p, cycle):  # pylint: disable=unused-argument, invalid-name
+            if len(obj.shape) < 2:
+                print(repr(obj))
+            if 2 <= len(obj.shape) <= 3:
+                pass
+            else:
+                print(f"<array of shape {obj.shape}>")
+
+        get_ipython().display_formatter.formatters["image/png"].for_type(np.ndarray, np_to_png)
+        get_ipython().display_formatter.formatters["text/plain"].for_type(np.ndarray, np_to_text)
```

### Comparing `xarray-einstats-0.5.1/PKG-INFO` & `xarray_einstats-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: xarray-einstats
-Version: 0.5.1
+Version: 0.6.0
 Summary: Stats, linear algebra and einops for xarray
 Author-email: ArviZ team <arviz.devs@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.6
+Requires-Dist: numpy>=1.21
+Requires-Dist: scipy>=1.7
 Requires-Dist: xarray>=2022.09.0
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: myst-parser[linkify] ; extra == "doc"
 Requires-Dist: myst-nb ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: sphinx>=4 ; extra == "doc"
 Requires-Dist: jupyter-sphinx ; extra == "doc"
 Requires-Dist: sphinx-design ; extra == "doc"
 Requires-Dist: watermark ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "doc"
+Requires-Dist: sphinx-togglebutton ; extra == "doc"
 Requires-Dist: einops ; extra == "einops"
 Requires-Dist: numba>=0.55 ; extra == "numba"
 Requires-Dist: hypothesis ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: packaging ; extra == "test"
 Project-URL: documentation, https://xarray-einstats.readthedocs.io
```

