# Comparing `tmp/mleko-0.6.1.tar.gz` & `tmp/mleko-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.6.1.tar", max compression
+gzip compressed data, was "mleko-0.7.0.tar", max compression
```

## Comparing `mleko-0.6.1.tar` & `mleko-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1073 2023-06-30 10:51:03.036693 mleko-0.6.1/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-30 10:51:03.036693 mleko-0.6.1/README.md
--rw-r--r--   0        0        0     1323 2023-06-30 10:51:33.460752 mleko-0.6.1/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/__init__.py
--rw-r--r--   0        0        0    13234 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1938 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     6957 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1530 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    12019 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5979 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5332 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5134 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5387 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7212 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5717 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18020 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9768 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1489 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3931 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6038 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1611 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     4556 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4521 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0     4153 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3809 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4185 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      644 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3711 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      697 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2482 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2302 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2148 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2372 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     2211 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0        0 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1413 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-30 10:51:03.040693 mleko-0.6.1/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2501 2023-06-30 10:51:33.516752 mleko-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 mleko-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-11 17:49:21.416446 mleko-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-07-11 17:49:21.416446 mleko-0.7.0/README.md
+-rw-r--r--   0        0        0     1323 2023-07-11 17:49:52.608954 mleko-0.7.0/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    14251 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     2076 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     8242 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1537 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11968 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     8033 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     6228 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     4789 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5061 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     6921 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5380 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2261 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18017 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9970 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1580 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4059 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6543 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1611 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     5158 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     5477 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4195 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0     3829 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3464 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     3870 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      644 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3711 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      697 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2549 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2495 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2148 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2439 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     2399 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-07-11 17:49:21.416446 mleko-0.7.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-07-11 17:49:21.420446 mleko-0.7.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1413 2023-07-11 17:49:21.420446 mleko-0.7.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-07-11 17:49:21.420446 mleko-0.7.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2537 2023-07-11 17:49:52.660955 mleko-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3620 1970-01-01 00:00:00.000000 mleko-0.7.0/PKG-INFO
```

### Comparing `mleko-0.6.1/LICENSE` & `mleko-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/README.md` & `mleko-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/__init__.py` & `mleko-0.7.0/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `mleko-0.6.1/mleko/cache/__init__.py` & `mleko-0.7.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/cache/cache_mixin.py` & `mleko-0.7.0/mleko/cache/cache_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,32 @@
     module_name = caller_obj.__name__ if caller_obj is not None else "__main__"
     if "self" in frame.frame.f_locals:
         class_name = frame.frame.f_locals["self"].__class__.__name__
         return f"{module_name}.{class_name}.{caller_function}"
     return f"{module_name}.{caller_function}"
 
 
+def get_class_method_name(frame_depth: int) -> str:
+    """Gets the fully qualified name of the calling function or method.
+
+    The fully qualified name is in the format "module.class.method" for class methods or "module.function" for
+    functions.
+
+    Args:
+        frame_depth: The depth of the frame to inspect. The default value is 2, which is the frame of the calling
+            function or method. For each nested function or method, the frame depth should be increased by 1.
+
+    Returns:
+        A string representing the fully qualified name of the calling function or method.
+    """
+    frame_qualname = get_frame_qualname(inspect.stack()[frame_depth])
+    class_method_name = ".".join(frame_qualname.split(".")[-2:])
+    return class_method_name
+
+
 class CacheMixin:
     """A mixin class for caching the results of method calls based on user-defined cache keys and fingerprints.
 
     The basic functionality of this class is to cache the results of method calls based on user-defined cache keys and
     fingerprints. The cache keys can be a mix of hashable values and tuples containing a value and a BaseFingerprinter
     instance for generating fingerprints. The `CacheMixin` class will save cache files in the specified cache directory
     using the cache key as the filename and the cache file suffix as the file extension. The cache files will be saved
@@ -59,23 +77,24 @@
         This class maintains an ever-growing cache, which means that the cache size may increase indefinitely
         with new method calls, possibly consuming a large amount of disk space. It does not implement any
         cache eviction strategy. It is recommended to either clear the cache manually when needed or
         use the LRUCacheMixin class, which extends this class to provide an LRU cache mechanism with
         eviction of least recently used cache entries based on a specified maximum number of cache entries.
     """
 
-    def __init__(self, cache_directory: str | Path, cache_file_suffix: str) -> None:
+    def __init__(self, cache_directory: str | Path, cache_file_suffix: str, disable_cache: bool) -> None:
         """Initializes the `CacheMixin` with the provided cache directory.
 
         Note:
             The cache directory will be created if it does not exist.
 
         Args:
             cache_directory: The directory where cache files will be stored.
             cache_file_suffix: The suffix/file ending of the cache files.
+            disable_cache: Whether to disable the cache.
 
         Examples:
             >>> from mleko.cache.cache_mixin import CacheMixin
             >>> class MyClass(CacheMixin):
             ...     def __init__(self):
             ...         super().__init__(".cache", "pkl")
             ...
@@ -90,22 +109,23 @@
             >>> my_class.my_method(3)
             9 # This will be recomputed and cached
         """
         self._cache_directory = Path(cache_directory)
         self._cache_directory.mkdir(parents=True, exist_ok=True)
         self._cache_file_suffix = cache_file_suffix
         self._cache_type_name = self._find_cache_type_name(self.__class__)
+        self._disable_cache = disable_cache
 
     def _cached_execute(
         self,
         lambda_func: Callable[[], Any],
         cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]],
         cache_group: str | None = None,
         force_recompute: bool = False,
-    ) -> Any:
+    ) -> tuple[bool, Any]:
         """Executes the given function, caching the results based on the provided cache keys and fingerprints.
 
         Warning:
             The cache group is used to group related cache keys together to prevent collisions between cache keys
             originating from the same method. For example, if a method is called during the training and testing
             phases of a machine learning pipeline, the cache keys for the training and testing phases should be
             using different cache groups to prevent collisions between the cache keys for the two phases. Otherwise,
@@ -117,55 +137,58 @@
                 BaseFingerprinter instance for generating fingerprints.
             cache_group: A string representing the cache group, used to group related cache keys together when methods
                 are called independently.
             force_recompute: A boolean indicating whether to force recompute the result and update the cache, even if a
                 cached result is available.
 
         Returns:
-            The result of executing the given function. If a cached result is available and `force_recompute` is False,
-            the cached result will be returned instead of recomputing the result.
+            A tuple containing a boolean indicating whether the cached result was used, and the result of executing the
+            given function. If a cached result is available and `force_recompute` is False, the cached result will be
+            returned instead of recomputing the result.
         """
-        frame_qualname = get_frame_qualname(inspect.stack()[1])
-        class_method_name = ".".join(frame_qualname.split(".")[-2:])
-        cache_key = self._compute_cache_key(cache_keys, class_method_name, cache_group)
+        if self._disable_cache:
+            return False, lambda_func()
+
+        class_method_name = get_class_method_name(2)
+        cache_key = self._compute_cache_key(cache_keys, cache_group)
 
         if not force_recompute:
             output = self._load_from_cache(cache_key)
             if output is not None:
                 logger.info(
                     f"\033[32mCache Hit\033[0m ({self._cache_type_name}) {class_method_name}: Using cached output."
                 )
-                return output
+                return True, output
             else:
                 logger.info(
                     f"\033[31mCache Miss\033[0m ({self._cache_type_name}) {class_method_name}: Executing method."
                 )
         else:
             logger.info(
                 f"\033[33mForce Cache Refresh\033[0m ({self._cache_type_name}) {class_method_name}: Executing method."
             )
 
         output = lambda_func()
         self._save_to_cache(cache_key, output)
-        return self._load_from_cache(cache_key)
+        return False, self._load_from_cache(cache_key)
 
     def _compute_cache_key(
         self,
         cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]],
-        class_method_name: str,
         cache_group: str | None = None,
+        frame_depth: int = 3,
     ) -> str:
         """Computes the cache key based on the provided cache keys and the calling function's fully qualified name.
 
         Args:
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
                 BaseFingerprinter instance for generating fingerprints.
-            class_method_name: A string of format "class.method" for class methods or "module.function" for
-                functions, representing the fully qualified name of the calling function or method.
             cache_group: A string representing the cache group.
+            frame_depth: The depth of the frame to inspect. The default value is 2, which is the frame of the calling
+                function or method. For each nested function or method, the frame depth should be increased by 1.
 
         Raises:
             ValueError: If the computed cache key is too long.
 
         Returns:
             A string representing the computed cache key, which is the MD5 hash of the fully qualified name of the
             calling function or method, along with the fingerprints of the provided cache keys.
@@ -176,15 +199,15 @@
             if isinstance(key, tuple) and len(key) == 2 and isinstance(key[1], BaseFingerprinter):
                 value, fingerprinter = key
                 values_to_hash.append(fingerprinter.fingerprint(value))
             else:
                 values_to_hash.append(key)
 
         data = pickle.dumps(values_to_hash)
-        cache_key_prefix = class_method_name
+        cache_key_prefix = get_class_method_name(frame_depth)
         if cache_group is not None:
             cache_key_prefix = f"{cache_key_prefix}.{cache_group}"
 
         cache_key = f"{cache_key_prefix}.{hashlib.md5(data).hexdigest()}"
         if len(cache_key) + 1 + len(self._cache_file_suffix) > 255:
             raise ValueError(
                 f"The computed cache key is too long ({len(cache_key) + len(self._cache_file_suffix)} chars)."
```

### Comparing `mleko-0.6.1/mleko/cache/fingerprinters/__init__.py` & `mleko-0.7.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.7.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.7.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.7.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.7.0/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-"""The module containing the mixin class for `vaex` DataFrames to provide Arrow format caching capabilities."""
+"""The module containing the mixin class for `vaex` DataFrames to provide HDF5 format caching capabilities."""
 from __future__ import annotations
 
+import warnings
 from pathlib import Path
 
 import vaex
 from tqdm.auto import tqdm
 
 from mleko.utils.tqdm_helpers import set_tqdm_percent_wrapper
 
 
 class VaexCacheFormatMixin:
-    """A mixin class for `vaex` DataFrames to provide Arrow format caching capabilities.
+    """A mixin class for `vaex` DataFrames to provide HDF5 format caching capabilities.
 
-    This mixin class adds methods for reading and writing arrow cache files for `vaex` DataFrames.
+    This mixin class adds methods for reading and writing HDF5 cache files for `vaex` DataFrames.
     This mixin class is intended to be used with the `Cache` class. It is not intended to be used directly.
 
     Warning:
         The mixin should be before the cache format class in the inheritance list.
 
     Examples:
         >>> class MyCacheFormat(VaexCacheFormatMixin, CacheFormat):
         >>>     pass
     """
 
-    _cache_file_suffix = "arrow"
+    _cache_file_suffix = "hdf5"
     """The file extension to use for cache files."""
 
     def _read_cache_file(self, cache_file_path: Path) -> vaex.DataFrame:
         """Reads a cache file containing a `vaex` DataFrame.
 
         Args:
             cache_file_path: The path of the cache file to be read.
 
         Returns:
             The contents of the cache file as a DataFrame.
         """
         return vaex.open(cache_file_path)
 
     def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
-        """Writes the results of the DataFrame conversion to Arrow format in a cache file with `.arrow` suffix.
+        """Writes the results of the DataFrame conversion to HDF5 format in a cache file with `.hdf5` suffix.
 
         Args:
             cache_file_path: The path of the cache file to be written.
             output: The Vaex DataFrame to be saved in the cache file.
         """
-        with tqdm(total=100, desc=f"Writing DataFrame to .{self._cache_file_suffix} file") as pbar:
-            output.export(
-                cache_file_path,
-                progress=set_tqdm_percent_wrapper(pbar),
-                parallel=True,
-                chunk_size=100_000,
-            )
-        output.close()
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", "invalid value encountered in cast")
+            with tqdm(total=100, desc=f"Writing DataFrame to .{self._cache_file_suffix} file") as pbar:
+                output.export(
+                    cache_file_path,
+                    progress=set_tqdm_percent_wrapper(pbar),
+                    parallel=True,
+                    chunk_size=100_000,
+                )
```

### Comparing `mleko-0.6.1/mleko/cache/lru_cache_mixin.py` & `mleko-0.7.0/mleko/cache/lru_cache_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,53 +28,57 @@
 
     This mixin class extends the CacheMixin to provide a Least Recently Used (LRU) cache mechanism.
     It evicts the least recently used cache entries when the maximum number of cache entries is exceeded.
     The LRU cache mechanism ensures that the most frequently accessed cache entries are retained,
     while entries that are rarely accessed and have not been accessed recently are evicted first as the cache fills up.
     """
 
-    def __init__(self, cache_directory: str | Path, cache_file_suffix: str, cache_size: int) -> None:
+    def __init__(
+        self, cache_directory: str | Path, cache_file_suffix: str, cache_size: int, disable_cache: bool
+    ) -> None:
         """Initializes the `LRUCacheMixin` with the provided cache directory and maximum number of cache entries.
 
         Note:
             The cache directory is created if it does not exist. When cold starting the cache, the cache will be loaded
             from the cache directory. The files are sorted by their modification time, and the cache is trimmed if
             needed.
 
         Args:
-            cache_directory: The directory where cache files will be stored.
+            cache_directory: The directory where cache files will be stored. If None, the cache will be disabled.
             cache_file_suffix: The file extension to use for cache files.
             cache_size: The maximum number of cache entries allowed before eviction.
+            disable_cache: Whether to disable the cache.
 
         Examples:
             >>> from mleko.cache import LRUCacheMixin
             >>> class MyClass(LRUCacheMixin):
             ...     def __init__(self):
             ...         super().__init__("cache", "pkl", 2)
             ...
             ...     def my_method(self, x):
-            ...         return self._cached_execute(lambda: x ** 2, [x])
+            ...         return self._cached_execute(lambda: x ** 2, [x])[1]
             >>> my_class = MyClass()
             >>> my_class.my_method(2)
             4 # This is not cached
             >>> my_class.my_method(2)
             4 # This is cached
             >>> my_class.my_method(3)
             9 # This is not cached
             >>> my_class.my_method(2)
             4 # This is cached
             >>> my_class.my_method(3)
             9 # This is cached
             >>> my_class.my_method(4)
             16 # This is not cached, and the cache is full so the least recently used entry is evicted (x = 2)
         """
-        super().__init__(cache_directory, cache_file_suffix)
-        self._cache_size = cache_size
-        self._cache: dict[str, OrderedDict[str, bool]] = defaultdict(OrderedDict)
-        self._load_cache_from_disk()
+        super().__init__(cache_directory, cache_file_suffix, disable_cache)
+        if not self._disable_cache:
+            self._cache_size = cache_size
+            self._cache: dict[str, OrderedDict[str, bool]] = defaultdict(OrderedDict)
+            self._load_cache_from_disk()
 
     def _load_cache_from_disk(self) -> None:
         """Loads the cache entries from the cache directory and initializes the LRU cache.
 
         Cache entries are ordered by their modification time, and the cache is trimmed if needed.
         """
         frame_qualname = get_frame_qualname(inspect.stack()[2])
@@ -88,26 +92,31 @@
         ]
         ordered_cache_files = sorted(cache_files, key=lambda x: x.stat().st_mtime)
 
         for cache_file in ordered_cache_files:
             cache_key_match = re.search(file_name_pattern, cache_file.stem)
             if cache_key_match:
                 method_name, cache_group = cache_key_match.groups()
-                group_identifier = method_name + cache_group if cache_group else method_name
+                group_identifier = (
+                    f"{class_name}.{method_name}{cache_group}" if cache_group else f"{class_name}.{method_name}"
+                )
                 cache_key = cache_key_match.group(0)
 
                 if cache_key not in self._cache[group_identifier]:
                     if len(self._cache[group_identifier]) >= self._cache_size:
                         oldest_key = next(iter(self._cache[group_identifier]))
                         del self._cache[group_identifier][oldest_key]
                         for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                            logger.debug(f"Max cache size reached ({self._cache_size}), deleting file {file}")
                             file.unlink()
 
                     self._cache[group_identifier][cache_key] = True
 
+        self._delete_non_cache_files()
+
     def _load_from_cache(self, cache_key: str) -> Any | None:
         """Loads data from the cache based on the provided cache key and updates the LRU cache.
 
         Args:
             cache_key: A string representing the cache key.
 
         Returns:
@@ -124,26 +133,43 @@
 
         If the cache reaches its maximum size, the least recently used entry will be evicted.
 
         Args:
             cache_key: A string representing the cache key.
             output: The data to be saved to the cache.
         """
+        frame_qualname = get_frame_qualname(inspect.stack()[2])
+        class_name = frame_qualname.split(".")[-2]
         cache_key_match = re.match(
             r"[a-zA-Z_][a-zA-Z0-9_]*\.([a-zA-Z_][a-zA-Z0-9_]*)(\.[a-zA-Z_][a-zA-Z0-9_]*)?\.[a-fA-F\d]{32}", cache_key
         )
+
         if cache_key_match:
             method_name, cache_group = cache_key_match.groups()
-            group_identifier = method_name + cache_group if cache_group else method_name
+            group_identifier = (
+                f"{class_name}.{method_name}{cache_group}" if cache_group else f"{class_name}.{method_name}"
+            )
 
             if cache_key not in self._cache[group_identifier]:
                 if len(self._cache[group_identifier]) >= self._cache_size:
                     oldest_key = next(iter(self._cache[group_identifier]))
                     del self._cache[group_identifier][oldest_key]
                     for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                        logger.debug(f"Max cache size reached ({self._cache_size}), deleting file {file}")
                         file.unlink()
 
                 self._cache[group_identifier][cache_key] = True
             else:
                 self._cache[group_identifier].move_to_end(cache_key)
 
             super()._save_to_cache(cache_key, output)
+
+        self._delete_non_cache_files()
+
+    def _delete_non_cache_files(self) -> None:
+        """Deletes all non-cached files which are not connected to any in-memory cache entry."""
+        for group_identifier in self._cache.keys():
+            for file in self._cache_directory.glob(f"{group_identifier}*"):
+                cache_key = re.sub(r"_\d+$", "", file.stem)
+                if cache_key not in self._cache[group_identifier]:
+                    logger.debug(f"No matching cache entry found, deleting non-cached file {file}")
+                    file.unlink()
```

### Comparing `mleko-0.6.1/mleko/dataset/__init__.py` & `mleko-0.7.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/convert/base_converter.py` & `mleko-0.7.0/mleko/dataset/convert/base_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         The `cache_size` is the maximum number of cache entries, and the cache will be cleared if the number of
         entries exceeds this value.
 
         Args:
             cache_directory: The directory to store the cache in.
             cache_size: The maximum number of cache entries.
         """
-        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
+        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size, False)
 
     @abstractmethod
     def convert(
         self, file_paths: list[Path] | list[str], cache_group: str | None = None, force_recompute: bool = False
     ) -> vaex.DataFrame:
         """Abstract method to convert the input file paths to the desired output format.
```

### Comparing `mleko-0.6.1/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.7.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             file_paths: A list of file paths to be converted.
             cache_group: The cache group to use.
             force_recompute: If set to True, forces recomputation and ignores the cache.
 
         Returns:
             The resulting dataframe with the combined converted data.
         """
-        return self._cached_execute(
+        _, df = self._cached_execute(
             lambda_func=lambda: self._convert(file_paths),
             cache_keys=[
                 self._forced_numerical_columns,
                 self._forced_categorical_columns,
                 self._forced_boolean_columns,
                 self._drop_columns,
                 self._na_values,
@@ -153,20 +153,20 @@
                 self._false_values,
                 self._downcast_float,
                 (file_paths, CSVFingerprinter(n_rows=100_000 // len(file_paths))),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
         )
+        return df
 
     @staticmethod
     def _convert_csv_file_to_arrow(
         file_path: Path | str,
         output_directory: Path,
-        dataframe_suffix: str,
         forced_numerical_columns: tuple[str, ...],
         forced_categorical_columns: tuple[str, ...],
         forced_boolean_columns: tuple[str, ...],
         drop_columns: tuple[str, ...],
         na_values: tuple[str, ...],
         true_values: tuple[str, ...],
         false_values: tuple[str, ...],
@@ -176,15 +176,14 @@
 
         This operation is done in chunks to optimize parallel processing. The resulting dataframe is saved in the
         output directory with the given suffix.
 
         Args:
             file_path: The path of the CSV file to be converted.
             output_directory: The directory where the converted file should be saved.
-            dataframe_suffix: The suffix for the converted dataframe files.
             forced_numerical_columns: A sequence of column names to be forced to numerical type.
             forced_categorical_columns: A sequence of column names to be forced to categorical type.
             forced_boolean_columns: A sequence of column names to be forced to boolean type.
             drop_columns: A sequence of column names to be dropped from the dataframe.
             na_values: A sequence of values to be considered as NaN.
             true_values: A sequence of values to be considered as True.
             false_values: A sequence of values to be considered as False.
@@ -224,15 +223,15 @@
             ),
         ).drop(drop_columns)
 
         for column_name in df_chunk.get_column_names():
             if get_column(df_chunk, column_name).dtype in (pa.date32(), pa.date64()):
                 df_chunk[column_name] = get_column(df_chunk, column_name).astype("datetime64[s]")
 
-        output_path = output_directory / f"df_chunk_{file_path.stem}.{dataframe_suffix}"
+        output_path = output_directory / f"df_chunk_{file_path.stem}.arrow"
         df_chunk.export(output_path, chunk_size=100_000, parallel=False)
         df_chunk.close()
 
     def _convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format using parallel processing.
 
         Chunks of files are processed in parallel and saved in the output directory.
@@ -245,30 +244,33 @@
         """
         with tqdm(total=len(file_paths), desc="Converting CSV files") as pbar:
             with futures.ProcessPoolExecutor(max_workers=min(self._num_workers, len(file_paths))) as executor:
                 for _ in executor.map(
                     CSVToVaexConverter._convert_csv_file_to_arrow,
                     file_paths,
                     repeat(self._cache_directory),
-                    repeat(self._cache_file_suffix),
                     repeat(self._forced_numerical_columns),
                     repeat(self._forced_categorical_columns),
                     repeat(self._forced_boolean_columns),
                     repeat(self._drop_columns),
                     repeat(self._na_values),
                     repeat(self._true_values),
                     repeat(self._false_values),
                     repeat(self._downcast_float),
                 ):
                     pbar.update(1)
 
-        return vaex.open(self._cache_directory / f"df_chunk_*.{self._cache_file_suffix}")
+        df = vaex.open(self._cache_directory / "df_chunk_*.arrow")
+        for column_name in df.get_column_names(dtype=pa.null()):
+            df[column_name] = df[column_name].astype("string")
+
+        return df
 
     def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
         """Writes the results of the DataFrame conversion to Arrow format in a cache file with arrow suffix.
 
         Args:
             cache_file_path: The path of the cache file to be written.
             output: The Vaex DataFrame to be saved in the cache file.
         """
         super()._write_cache_file(cache_file_path, output)
-        clear_directory(cache_file_path.parent, pattern=f"df_chunk_*.{self._cache_file_suffix}")
+        clear_directory(cache_file_path.parent, pattern="df_chunk_*.arrow")
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/__init__.py` & `mleko-0.7.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Module for the base feature selector class."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Hashable
+from typing import Any, Hashable
 
+import joblib
 import vaex
 
+from mleko.cache.fingerprinters.base_fingerprinter import BaseFingerprinter
+from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.cache.format.vaex_cache_format_mixin import VaexCacheFormatMixin
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.utils.custom_logger import CustomLogger
 
 
 logger = CustomLogger()
 """The logger for the module."""
@@ -31,74 +34,85 @@
 
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...] | None,
         ignore_features: list[str] | tuple[str, ...] | None,
         cache_size: int,
+        disable_cache: bool,
     ) -> None:
         """Initializes the feature selector and ensures the destination directory exists.
 
         Note:
             The `features` and `ignore_features` arguments are mutually exclusive. If both are specified, a
             `ValueError` is raised.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the feature selector. If None, the default is all features
                 applicable to the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector. If None, the default is to
                 ignore no features.
             cache_size: The maximum number of cache entries.
+            disable_cache: Whether to disable the cache.
 
         Raises:
             ValueError: If both `features` and `ignore_features` are specified.
         """
-        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
+        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size, disable_cache)
         if features is not None and ignore_features is not None:
             error_msg = (
                 "Both `features` and `ignore_features` have been specified. The arguments are mutually exclusive."
             )
             logger.error(error_msg)
             raise ValueError(error_msg)
 
         self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
         self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
+        self._feature_selector = None
 
-    @abstractmethod
     def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+        self, dataframe: vaex.DataFrame, fit: bool, cache_group: str | None = None, force_recompute: bool = False
     ) -> vaex.DataFrame:
-        """Selects features from the given DataFrame.
+        """Selects features from the given DataFrame, using the cached result if available.
 
         Args:
             dataframe: DataFrame from which to select features.
+            fit: Whether to fit the feature selector on the input data.
             cache_group: The cache group to use.
             force_recompute: Whether to force the feature selector to recompute its output, even if it already exists.
 
-        Raises:
-            NotImplementedError: Must be implemented in the child class that inherits from `BaseFeatureSelector`.
-
         Returns:
             A DataFrame with the selected features.
         """
-        raise NotImplementedError
+        cache_keys = [self._fingerprint(), (dataframe, VaexFingerprinter())]
+        cached, df = self._cached_execute(
+            lambda_func=lambda: self._select_features(dataframe, fit),
+            cache_keys=cache_keys,
+            cache_group=cache_group,
+            force_recompute=force_recompute,
+        )
+        if fit and not self._disable_cache:
+            self._save_or_load_feature_selector(cached, cache_group, cache_keys)
+
+        return df
 
     @abstractmethod
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects features from the given DataFrame.
 
         Args:
             dataframe: DataFrame from which to select features.
+            fit: Whether to fit the feature selector on the input data.
 
         Raises:
             NotImplementedError: Must be implemented in the child class that inherits from `BaseFeatureSelector`.
 
         Returns:
-            DataFrame with the selected features.
+            A DataFrame with the selected features.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features to be used by the feature selector.
 
@@ -140,7 +154,31 @@
             Sorted list of feature names to be used by the feature selector.
         """
         return sorted(
             set(self._default_features(dataframe)) - set(self._ignore_features)
             if self._features is None
             else self._features
         )
+
+    def _save_or_load_feature_selector(
+        self, load: bool, cache_group: str | None, cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]]
+    ) -> None:
+        """Saves or loads the feature selector to/from the cache.
+
+        Will save the feature selector to the cache if `load` is False, otherwise will load the feature selector
+        from the cache. The cache key is computed using the specified cache keys and will be used to save the
+        feature selector to the cache using joblib.
+
+        Args:
+            load: Whether to load the feature selector from the cache or save it to the cache.
+            cache_group: The cache group to use.
+            cache_keys: The cache keys to use for the feature selector.
+        """
+        cache_key = self._compute_cache_key(cache_keys, cache_group, frame_depth=3)
+        feature_selector_path = self._cache_directory / f"{cache_key}.feature_selector"
+
+        if load:
+            logger.info(f"Loading feature selector from {feature_selector_path}.")
+            self._feature_selector = joblib.load(feature_selector_path)
+        else:
+            logger.info(f"Saving feature selector to {feature_selector_path}.")
+            joblib.dump(self._feature_selector, feature_selector_path)
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A feature selector that combines multiple feature selectors."""
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Hashable
+from typing import Any, Hashable
 
 import vaex
 
 from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
@@ -26,24 +26,26 @@
 
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         feature_selectors: list[BaseFeatureSelector] | tuple[BaseFeatureSelector, ...],
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the composite feature selector.
 
         The composite feature selector will combine the feature selectors into a single feature selector. Each feature
         selector will be applied to the DataFrame in the order they are specified.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             feature_selectors: List of feature selectors to be combined.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import CompositeFeatureSelector, MissingRateFeatureSelector
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
             ...     b=[1, 2, 3, 4, None, None, None, None, None, None],
@@ -71,52 +73,69 @@
             4    5    5
             5    6    6
             6    7    None
             7    8    None
             8    9    None
             9   10    None
         """
-        super().__init__(cache_directory, None, None, cache_size)
+        super().__init__(cache_directory, None, None, cache_size, disable_cache)
         self._feature_selectors = tuple(feature_selectors)
+        self._feature_selector: list[Any] = []
+
+        for feature_selector in self._feature_selectors:
+            feature_selector._disable_cache = True
 
     def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+        self, dataframe: vaex.DataFrame, fit: bool, cache_group: str | None = None, force_recompute: bool = False
     ) -> vaex.DataFrame:
         """Selects the features from the DataFrame.
 
         Args:
             dataframe: DataFrame from which the features will be selected.
+            fit: Whether to fit the feature selectors on the input data.
             cache_group: The cache group to use for caching.
             force_recompute: If True, the features will be recomputed even if they are cached.
 
         Returns:
             DataFrame with the selected features.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._select_features(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+        cache_keys = [self._fingerprint(), (dataframe, VaexFingerprinter())]
+        cached, df = self._cached_execute(
+            lambda_func=lambda: self._select_features(dataframe, fit),
+            cache_keys=cache_keys,
             cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
+        if fit:
+            self._save_or_load_feature_selector(cached, cache_group, cache_keys)
+
+            if cached:
+                for feature_selector, feature_selector_pkl in zip(self._feature_selectors, self._feature_selector):
+                    feature_selector._feature_selector = feature_selector_pkl
+
+        return df
+
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects the features from the DataFrame.
 
         Args:
             dataframe: DataFrame from which the features will be selected.
+            fit: Whether to fit the feature selectors on the input data.
 
         Returns:
             DataFrame with the selected features.
         """
         for i, feature_selector in enumerate(self._feature_selectors):
             logger.info(
                 f"Executing composite feature selection step {i+1}/{len(self._feature_selectors)}: "
                 f"{feature_selector.__class__.__name__}."
             )
-            dataframe = feature_selector._select_features(dataframe).extract()
+            dataframe = feature_selector.select_features(dataframe, fit).extract()
+            self._feature_selector.append(feature_selector._feature_selector)
             logger.info(f"Finished composite feature selection step {i+1}/{len(self._feature_selectors)}.")
         return dataframe
 
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:  # pragma: no cover
         """Returns the default features of the DataFrame.
 
         Args:
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 from tqdm.auto import tqdm
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.dataset.feature_select.base_feature_selector import BaseFeatureSelector
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
 
 
 logger = CustomLogger()
@@ -24,14 +23,15 @@
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...] | None = None,
         ignore_features: list[str] | tuple[str, ...] | None = None,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the feature selector.
 
         The feature selector will filter out all invariant features. The default set of features
         are all categorical and boolean features in the DataFrame.
 
         Note:
@@ -42,14 +42,15 @@
             target feature or some identifier.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import InvarianceFeatureSelector
             >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
@@ -60,60 +61,50 @@
             >>> selector = InvarianceFeatureSelector(
             ...     cache_directory=".",
             ... )
             >>> df_selected = selector.select_features(df)
             >>> df_selected.get_column_names()
             ['a', 'c', 'd']
         """
-        super().__init__(cache_directory, features, ignore_features, cache_size)
+        super().__init__(cache_directory, features, ignore_features, cache_size, disable_cache)
+        self._feature_selector: set[str] = set()
 
-    def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects features based on invariance.
 
         Args:
             dataframe: The DataFrame to select features from.
-            cache_group: The cache group to use for caching.
-            force_recompute: Whether to force recompute the selected features.
+            fit: Whether to fit the feature selector on the input data.
 
         Returns:
             The DataFrame with the selected features.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._select_features(dataframe),
-            cache_keys=[
-                self._fingerprint(),
-                (dataframe, VaexFingerprinter()),
-            ],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
-        )
+        if fit:
+            self._fit(dataframe)
 
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Selects features based on invariance.
+        dropped_features = self._feature_selector
+        logger.info(f"Dropping ({len(dropped_features)}) invariant features: {dropped_features}.")
+        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
+        return get_columns(dataframe, selected_features)
 
-        Args:
-            dataframe: The DataFrame to select features from.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the feature selector on the input data.
 
-        Returns:
-            The DataFrame with the selected features.
+        Args:
+            dataframe: The DataFrame to fit the feature selector on.
         """
         features = self._feature_set(dataframe)
-        logger.info(f"Selecting features from the following set ({len(features)}): {features}.")
+        logger.info(f"Fitting invariance feature selector on {len(features)} features: {features}.")
 
         cardinality = {}
         for feature in tqdm(features, desc="Calculating invariance of features"):
             column = get_column(dataframe, feature)
             cardinality[feature] = column.nunique(limit=2, limit_raise=False)
 
-        dropped_features = {feature for feature in features if cardinality[feature] == 1}
-        logger.info(f"Dropping ({len(dropped_features)}) invariant features: {dropped_features}.")
-        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
-        return get_columns(dataframe, selected_features)
+        self._feature_selector = {feature for feature in features if cardinality[feature] == 1}
 
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 from tqdm.auto import tqdm
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
 
 from .base_feature_selector import BaseFeatureSelector
 
 
@@ -26,14 +25,15 @@
     def __init__(
         self,
         cache_directory: str | Path,
         missing_rate_threshold: float,
         features: list[str] | tuple[str, ...] | None = None,
         ignore_features: list[str] | tuple[str, ...] | None = None,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the feature selector.
 
         The feature selector will select all features with a missing rate below the specified threshold. The default
         set of features is all features in the DataFrame.
 
         Note:
@@ -45,14 +45,15 @@
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             missing_rate_threshold: The maximum missing rate allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import MissingRateFeatureSelector
             >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
@@ -62,64 +63,56 @@
             >>> MissingRateFeatureSelector(
             ...     cache_directory=".",
             ...     ignore_features=["c"],
             ...     missing_rate_threshold=0.3,
             ... ).select_features(df).get_column_names()
             ['a', 'b']
         """
-        super().__init__(cache_directory, features, ignore_features, cache_size)
+        super().__init__(cache_directory, features, ignore_features, cache_size, disable_cache)
         self._missing_rate_threshold = missing_rate_threshold
+        self._feature_selector: set[str] = set()
 
-    def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects features based on the missing rate.
 
-        Will cache the result of the feature selection.
-
         Args:
             dataframe: The DataFrame to select features from.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recompute the feature selection.
+            fit: Whether to fit the feature selector on the input data.
 
         Returns:
             The DataFrame with the selected features.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._select_features(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
+        if fit:
+            self._fit(dataframe)
+
+        dropped_features = self._feature_selector
+        logger.info(
+            f"Dropping ({len(dropped_features)}) features with missing rate >= {self._missing_rate_threshold}: "
+            f"{dropped_features}."
         )
+        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
+        return get_columns(dataframe, selected_features)
 
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Selects features based on the missing rate.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the feature selector on the input data.
 
         Args:
-            dataframe: The DataFrame to select features from.
-
-        Returns:
-            The DataFrame with the selected features.
+            dataframe: The DataFrame to fit the feature selector on.
         """
         features = self._feature_set(dataframe)
-        logger.info(f"Selecting features from the following set ({len(features)}): {features}.")
+        logger.info(f"Fitting missing rate feature selector on {len(features)} features: {features}.")
 
         missing_rate: dict[str, float] = {}
         for feature in tqdm(features, desc="Calculating missing rates for features"):
             column = get_column(dataframe, feature)
             missing_rate[feature] = column.countna() / dataframe.shape[0]
 
-        dropped_features = {feature for feature in features if missing_rate[feature] >= self._missing_rate_threshold}
-        logger.info(
-            f"Dropping ({len(dropped_features)}) features with missing rate >= {self._missing_rate_threshold}: "
-            f"{dropped_features}."
-        )
-
-        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
-        return get_columns(dataframe, selected_features)
+        self._feature_selector = {
+            feature for feature in features if missing_rate[feature] >= self._missing_rate_threshold
+        }
 
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import itertools
 from pathlib import Path
 from typing import Hashable
 
 import numpy as np
 import vaex
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_columns
 
 from .base_feature_selector import BaseFeatureSelector
 
 
@@ -27,14 +26,15 @@
     def __init__(
         self,
         cache_directory: str | Path,
         correlation_threshold: float,
         features: list[str] | tuple[str, ...] | None = None,
         ignore_features: list[str] | tuple[str, ...] | None = None,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the feature selector.
 
         Will drop one of two features that are highly correlated. The feature to be dropped is the one with the lowest
         average correlation with all other features. If both features have the same average correlation, the first
         feature will be dropped. The default set of features is all numeric features in the DataFrame.
 
@@ -47,14 +47,15 @@
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             correlation_threshold: The maximum correlation allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import PearsonCorrelationFeatureSelector
             >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
@@ -65,48 +66,47 @@
             ...     cache_directory=".",
             ...     correlation_threshold=0.75,
             ... )
             >>> selected_features = feature_selector.select_features(df)
             >>> selected_features.get_column_names()
             ['a', 'c']
         """
-        super().__init__(cache_directory, features, ignore_features, cache_size)
+        super().__init__(cache_directory, features, ignore_features, cache_size, disable_cache)
         self._correlation_threshold = correlation_threshold
+        self._feature_selector: set[str] = set()
 
-    def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects features based on the Pearson correlation.
 
         Args:
             dataframe: The DataFrame to select features from.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recompute the selected features.
+            fit: Whether to fit the feature selector on the input data.
 
         Returns:
             The DataFrame with the selected features.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._select_features(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
+        if fit:
+            self._fit(dataframe)
+
+        dropped_features = self._feature_selector
+        logger.info(
+            f"Dropping ({len(dropped_features)}) features with correlation >= {self._correlation_threshold}: "
+            f"{dropped_features}."
         )
+        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
+        return get_columns(dataframe, selected_features)
 
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Selects features based on the Pearson correlation.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the feature selector on the input data.
 
         Args:
-            dataframe: The DataFrame to select features from.
-
-        Returns:
-            The DataFrame with the selected features.
+            dataframe: The DataFrame to fit the feature selector on.
         """
         features = self._feature_set(dataframe)
-        logger.info(f"Selecting features from the following set ({len(features)}): {features}.")
+        logger.info(f"Fitting pearson correlation feature selector on {len(features)} features: {features}.")
 
         corr_matrix = abs(np.array(dataframe.correlation(features)))
         avg_corr = corr_matrix.mean(axis=1)
 
         # Generate all possible pairs of features
         feature_pairs = list(itertools.combinations(enumerate(features), 2))
 
@@ -143,22 +143,15 @@
             drop_f
             for f_a, f_b, drop_f in correlated_features
             if (f_a in possible_drop or f_b in possible_drop)
             and (f_a not in guaranteed_dropped and f_b not in guaranteed_dropped)
         }
 
         # Combine guaranteed_dropped and additional_dropped sets
-        dropped_features = guaranteed_dropped.union(additional_dropped)
-        logger.info(
-            f"Dropping ({len(dropped_features)}) features with correlation >= {self._correlation_threshold}: "
-            f"{dropped_features}."
-        )
-
-        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
-        return get_columns(dataframe, selected_features)
+        self._feature_selector = guaranteed_dropped.union(additional_dropped)
 
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
```

### Comparing `mleko-0.6.1/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.7.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 from tqdm.auto import tqdm
 from vaex.ml import MaxAbsScaler
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.dataset.feature_select.base_feature_selector import BaseFeatureSelector
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
 
 
 logger = CustomLogger()
@@ -26,14 +25,15 @@
     def __init__(
         self,
         cache_directory: str | Path,
         variance_threshold: float,
         features: list[str] | tuple[str, ...] | None = None,
         ignore_features: list[str] | tuple[str, ...] | None = None,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the feature selector.
 
         The feature selector will select all features with a variance above the specified threshold.
         The default set of features is all numeric features in the DataFrame.
 
         Note:
@@ -45,14 +45,15 @@
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             variance_threshold: The minimum variance allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import VarianceFeatureSelector
             >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
@@ -65,70 +66,60 @@
             ...     ignore_features=["c"],
             ...     variance_threshold=0.1,
             ... )
             >>> df_selected = selector.select_features(df)
             >>> df_selected.get_column_names()
             ['a', 'c', 'd']
         """
-        super().__init__(cache_directory, features, ignore_features, cache_size)
+        super().__init__(cache_directory, features, ignore_features, cache_size, disable_cache)
         self._variance_threshold = variance_threshold
+        self._feature_selector: set[str] = set()
 
-    def select_features(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _select_features(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Selects features based on the variance.
 
         Args:
             dataframe: The DataFrame to select features from.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recompute the selected features.
+            fit: Whether to fit the feature selector on the input data.
 
         Returns:
             The DataFrame with the selected features.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._select_features(dataframe),
-            cache_keys=[
-                self._fingerprint(),
-                (dataframe, VaexFingerprinter()),
-            ],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
+        if fit:
+            self._fit(dataframe)
+
+        dropped_features = self._feature_selector
+        logger.info(
+            f"Dropping ({len(dropped_features)}) features with normalized variance <= {self._variance_threshold}: "
+            f"{dropped_features}."
         )
+        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
+        return get_columns(dataframe, selected_features)
 
-    def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Selects features based on the variance.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the feature selector on the input data.
 
         Args:
-            dataframe: The DataFrame to select features from.
-
-        Returns:
-            The DataFrame with the selected features.
+            dataframe: The DataFrame to fit the feature selector on.
         """
         features = self._feature_set(dataframe)
-        logger.info(f"Selecting features from the following set ({len(features)}): {features}.")
+        logger.info(f"Fitting variance feature selector on {len(features)} features: {features}.")
 
         if self._variance_threshold > 0:
             scaler = MaxAbsScaler(features=list(features), prefix="")
             df = scaler.fit_transform(dataframe)
         else:
             df = dataframe
 
         variance: dict[str, float] = {}
         for feature in tqdm(features, desc="Calculating variance for features"):
             column = get_column(df, feature)
             variance[feature] = column.var()
 
-        dropped_features = {feature for feature in features if variance[feature] <= self._variance_threshold}
-        logger.info(
-            f"Dropping ({len(dropped_features)}) features with normalized variance <= {self._variance_threshold}: "
-            f"{dropped_features}."
-        )
-        selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
-        return get_columns(dataframe, selected_features)
+        self._feature_selector = {feature for feature in features if variance[feature] <= self._variance_threshold}
 
     def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
```

### Comparing `mleko-0.6.1/mleko/dataset/ingest/__init__.py` & `mleko-0.7.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/ingest/base_ingester.py` & `mleko-0.7.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.7.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 "Attempting to fetch Kaggle API credentials from environment variables "
                 f"{KaggleCredentialsManager._ENV_VARIABLE_USERNAME!r} and "
                 f"{KaggleCredentialsManager._ENV_VARIABLE_KEY!r}."
             )
             env_credentials = KaggleCredentialsManager._read_environment_config()
 
             if env_credentials is None:
-                logger.warning(
+                logger.info(
                     "Kaggle API credentials not found in environment variables, attempting to fetch from "
                     f"fallback path at {KaggleCredentialsManager._CONFIG_DEFAULT_PATH}."
                 )
                 credentials = KaggleCredentialsManager._read_config_file(
                     Path(KaggleCredentialsManager._CONFIG_DEFAULT_PATH)
                 )
             else:
```

### Comparing `mleko-0.6.1/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.7.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,17 @@
             ... )
             >>> s3_ingester.fetch_data()
             [PosixPath('data/indian_food.csv')]
         """
         super().__init__(destination_directory)
         self._s3_bucket_name = s3_bucket_name
         self._s3_key_prefix = s3_key_prefix
-        self._s3_client = self._get_s3_client(aws_profile_name, aws_region_name)
+        self._aws_profile_name = aws_profile_name
+        self._aws_region_name = aws_region_name
+        self._s3_client = self._get_s3_client(self._aws_profile_name, self._aws_region_name)
         self._num_workers = num_workers
         self._manifest_file_name = manifest_file_name
         self._check_s3_timestamps = check_s3_timestamps
 
     def fetch_data(self, force_recompute: bool = False) -> list[Path]:
         """Downloads the data from the S3 bucket and stores it in the 'destination_directory'.
 
@@ -96,22 +98,23 @@
         Raises:
             Exception: If files in the S3 bucket have different last modified dates, indicating potential corruption
                        or duplication.
 
         Returns:
             A list of Path objects pointing to the downloaded data files.
         """
+        self._s3_client = self._get_s3_client(self._aws_profile_name, self._aws_region_name)
         resp = self._s3_client.list_objects(
             Bucket=self._s3_bucket_name,
             Prefix=self._s3_key_prefix,
         )
 
         if self._check_s3_timestamps:
             modification_dates = {key["LastModified"].day for key in resp["Contents"] if "LastModified" in key}
-            if len(modification_dates) != 1:
+            if len(modification_dates) > 1:
                 raise Exception(
                     "Files in S3 are from muliples dates. This might mean the data is corrupted/duplicated."
                 )
         if self._manifest_file_name is not None:
             manifest_file_key = next(
                 entry["Key"]
                 for entry in resp["Contents"]
```

### Comparing `mleko-0.6.1/mleko/dataset/split/__init__.py` & `mleko-0.7.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/split/base_splitter.py` & `mleko-0.7.0/mleko/dataset/split/base_splitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 
 class BaseSplitter(VaexCacheFormatMixin, LRUCacheMixin, ABC):
     """Abstract base class for data splitter.
 
     Will cache the split dataframes in the output directory.
     """
 
-    def __init__(self, cache_directory: str | Path, cache_size: int):
+    def __init__(self, cache_directory: str | Path, cache_size: int, disable_cache: bool):
         """Initializes the `BaseSplitter` with an output directory.
 
         Args:
             cache_directory: The target directory where the split dataframes are to be saved.
             cache_size: The maximum number of cache entries.
+            disable_cache: Whether to disable caching.
         """
-        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
+        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size, disable_cache)
 
     @abstractmethod
     def split(
         self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
     ) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Abstract method to split the given dataframe into two parts.
```

### Comparing `mleko-0.6.1/mleko/dataset/split/expression_splitter.py` & `mleko-0.7.0/mleko/dataset/split/expression_splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         expression: str,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ):
         """Initializes the `ExpressionSplitter` with the given parameters.
 
         The expression should be a valid Vaex expression that evaluates to a boolean
         value. The rows for which the expression evaluates to True will be returned as the first dataframe,
         and the remaining rows will be returned as the second dataframe.
 
@@ -39,14 +40,15 @@
 
         Args:
             cache_directory: The target directory where the split dataframes are to be saved.
             expression: A valid Vaex expression that evaluates to a boolean value. The rows for which the expression
                 evaluates to True will be returned as the first dataframe, and the remaining rows will be returned
                 as the second dataframe.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Example:
             >>> import vaex
             >>> from mleko.data.split import ExpressionSplitter
             >>> df = vaex.from_arrays(x=[1, 2, 3], y=[4, 5, 6])
             >>> splitter = ExpressionSplitter(cache_directory="cache", expression="x > 1")
             >>> df_train, df_test = splitter.split(df)
@@ -54,15 +56,15 @@
                 #    x    y
                 0    2    5
                 1    3    6
             >>> df_test
                 #    x    y
                 0    1    4
         """
-        super().__init__(cache_directory, cache_size)
+        super().__init__(cache_directory, cache_size, disable_cache)
         self._expression = expression
 
     def split(
         self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
     ) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
@@ -70,23 +72,24 @@
             dataframe: The dataframe to be split.
             cache_group: The cache group to use.
             force_recompute: Forces recomputation if True, otherwise reads from the cache if available.
 
         Returns:
             A tuple containing the split dataframes.
         """
-        return self._cached_execute(
+        _, dfs = self._cached_execute(
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._expression,
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
         )
+        return dfs
 
     def _split(self, dataframe: vaex.DataFrame) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Args:
             dataframe: The dataframe to be split.
```

### Comparing `mleko-0.6.1/mleko/dataset/split/random_splitter.py` & `mleko-0.7.0/mleko/dataset/split/random_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,32 +34,39 @@
         self,
         cache_directory: str | Path,
         data_split: tuple[float, float] = (0.80, 0.20),
         shuffle: bool = True,
         stratify: str | None = None,
         random_state: int | None = None,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ):
         """Initializes the `RandomSplitter` with the given parameters.
 
         Note:
             The stratification is performed before the split, meaning that the split will be performed on the stratified
             data. For example, if the data is split into 80% train and 20% test, and the stratification column contains
             80% of the rows with value 0 and 20% of the rows with value 1, the resulting split will contain 80% of the
             rows with value 0 and 20% of the rows with value 1.
 
+        Warning:
+            If `stratify` is not None and the target column is a string/categorical, the target feature must not have
+            any missing values. Please make sure to handle missing values before using this splitter by either dropping
+            the rows with missing values, imputing the missing values, or transforming the target to numeric or boolean.
+
         Args:
             cache_directory: The target directory where the split dataframes are to be saved.
             data_split: A tuple containing the desired split percentages or weights for the train and test dataframes.
                 If the sum of the values is not equal to 1, the values will be normalized. Meaning, if the values are
                 (0.90, 0.20), the resulting split will be (0.818, 0.182).
             shuffle: Whether to shuffle the data before splitting.
             stratify: The name of the column to use for stratification. If None, stratification will not be performed.
             random_state: The seed to use for random number generation.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Example:
             >>> import vaex
             >>> from mleko.data.split import RandomSplitter
             >>> df = vaex.from_arrays(x=[1, 2, 3, 4], y=[0, 1, 1, 0])
             >>> splitter = RandomSplitter(cache_directory="cache", data_split=(0.50, 0.50), shuffle=True, stratify="y")
             >>> df_train, df_test = splitter.split(df)
@@ -68,15 +75,15 @@
                 0    1    0
                 1    3    1
             >>> df_test
                 #    x    y
                 0    2    1
                 1    4    0
         """
-        super().__init__(cache_directory, cache_size)
+        super().__init__(cache_directory, cache_size, disable_cache)
         self._idx2_size = [split / sum(data_split) for split in data_split][1]
         self._shuffle = shuffle
         self._stratify = stratify
         self._random_state = random_state
 
     def split(
         self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
@@ -91,26 +98,27 @@
             dataframe: The dataframe to be split.
             cache_group: The cache group to use.
             force_recompute: Whether to force recompute the split, even if the cache is available.
 
         Returns:
             A tuple containing the split dataframes.
         """
-        return self._cached_execute(
+        _, dfs = self._cached_execute(
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._idx2_size,
                 self._shuffle,
                 self._stratify,
                 self._random_state,
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
         )
+        return dfs
 
     def _split(self, dataframe: vaex.DataFrame) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Args:
             dataframe: The dataframe to be split.
```

### Comparing `mleko-0.6.1/mleko/dataset/transform/__init__.py` & `mleko-0.7.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/dataset/transform/base_transformer.py` & `mleko-0.7.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,97 @@
-"""Module for the base transformer class."""
+"""Module for the max-abs scaler transformer."""
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Hashable
 
 import vaex
+import vaex.ml
 
-from mleko.cache.format.vaex_cache_format_mixin import VaexCacheFormatMixin
-from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.utils.custom_logger import CustomLogger
+from mleko.utils.decorators import auto_repr
 
+from .base_transformer import BaseTransformer
 
-logger = CustomLogger()
-"""The logger for the module."""
 
+logger = CustomLogger()
+"""A module-level logger for the module."""
 
-class BaseTransformer(VaexCacheFormatMixin, LRUCacheMixin, ABC):
-    """Abstract class for feature transformation.
 
-    The feature transformation process is implemented in the `transform` method, which takes a DataFrame as input and
-    returns a transformed DataFrame.
-    """
+class MaxAbsScalerTransformer(BaseTransformer):
+    """Transforms features using maximum absolute scaling."""
 
+    @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...],
-        cache_size: int,
+        cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
-        """Initializes the transformer and ensures the destination directory exists.
+        """Initializes the max absolute scaler transformer.
+
+        The max absolute scaler transformer will scale each feature by its maximum absolute value. This transformer
+        will not shift/center the data, and thus will not destroy any sparsity.
+
+        Warning:
+            Should only be used with numerical features. There should be no missing values in the features
+            or an error will be raised.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the transformer.
-            cache_size: The maximum number of cache entries to keep in the cache.
+            cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
+
+        Examples:
+            >>> import vaex
+            >>> from mleko.dataset.transform import MaxAbsScalerTransformer
+            >>> df = vaex.from_arrays(
+            ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+            ...     b=[-1, -2, -3, -4, -5, 0, 1, 2, 3, 4]
+            ... )
+            >>> df = MaxAbsScalerTransformer(
+            ...     cache_directory=".",
+            ...     features=["a", "b"],
+            ... ).transform(df)
+            >>> df["a"].tolist()
+            [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
+            >>> df["b"].tolist()
+            [-0.2, -0.4, -0.6, -0.8, -1.0, 0.0, 0.2, 0.4, 0.6, 0.8]
         """
-        LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
-        self._features: tuple[str, ...] = tuple(features)
+        super().__init__(cache_directory, features, cache_size, disable_cache)
+        self._transformer = vaex.ml.MaxAbsScaler(features=self._features, prefix="")
 
-    @abstractmethod
-    def transform(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
-        """Transfigures the specified features in the DataFrame.
+    def _transform(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
+        """Transforms the features in the DataFrame using max-abs scaling.
 
         Args:
-            dataframe: DataFrame to be transformed.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force the transformation to be recomputed even if the result is cached.
-
-        Raises:
-            NotImplementedError: Must be implemented by subclasses.
+            dataframe: The DataFrame to transform.
+            fit: Whether to fit the transformer on the input data.
 
         Returns:
-            Transformed DataFrame.
+            The transformed DataFrame.
         """
-        raise NotImplementedError
+        if fit:
+            self._fit(dataframe)
 
-    @abstractmethod
-    def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Transforms the specified features in the DataFrame.
+        logger.info(f"Transforming features using max-abs scaling ({len(self._features)}): {self._features}.")
+        transformed_df = self._transformer.transform(dataframe)
+        return transformed_df
 
-        Args:
-            dataframe: DataFrame to be transformed.
-
-        Raises:
-            NotImplementedError: Must be implemented by subclasses.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the transformer on the given DataFrame.
 
-        Returns:
-            Transformed DataFrame.
+        Args:
+            dataframe: The DataFrame to fit the transformer on.
         """
-        raise NotImplementedError
+        logger.info(f"Fitting max-abs scaler transformer ({len(self._features)}): {self._features}.")
+        self._transformer.fit(dataframe)
 
-    @abstractmethod
     def _fingerprint(self) -> Hashable:
-        """Returns a hashable object that uniquely identifies the transformer.
-
-        The base implementation fingerprints the class name and the features used by the transformer.
-
-        Note:
-            Subclasses should call the parent method and include the result in the hashable object along with any
-            other parameters that uniquely identify the transformer. All attributes that are used in the
-            transformer that affect the result of the transformation should be included in the hashable object.
+        """Returns the fingerprint of the transformer.
 
         Returns:
-            Hashable object that uniquely identifies the transformer.
+            A hashable object that uniquely identifies the transformer.
         """
-        return self.__class__.__name__, self._features
+        return super()._fingerprint()
```

### Comparing `mleko-0.6.1/mleko/dataset/transform/composite_transformer.py` & `mleko-0.7.0/mleko/dataset/transform/composite_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for the composite transformer."""
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Hashable
+from typing import Any, Hashable
 
 import vaex
 
 from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
@@ -26,24 +26,27 @@
 
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         transformers: list[BaseTransformer] | tuple[BaseTransformer, ...],
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the composite transformer.
 
         The composite transformer will combine the transformers into a single transformer. Each transformer will be
-        applied to the DataFrame in the order they are specified.
+        applied to the DataFrame in the order they are specified. Caching of the intermediate DataFrames is disabled
+        and will only be performed on the final DataFrame.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             transformers: List of transformers to be combined.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.transform import (
             ...     CompositeTransformer,
             ...     LabelEncoderTransformer,
             ...     FrequencyEncoderTransformer
@@ -67,52 +70,69 @@
             ... )
             >>> df = transformer.transform(df)
             >>> df["a"].tolist()
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
             >>> df["b"].tolist()
             [0.4, 0.4, 0.4, 0.4, nan, nan, nan, nan, nan, nan]
         """
-        super().__init__(cache_directory, [], cache_size)
+        super().__init__(cache_directory, [], cache_size, disable_cache)
         self._transformers = tuple(transformers)
+        self._transformer: list[Any] = []
+
+        for transformer in self._transformers:
+            transformer._disable_cache = True
 
     def transform(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+        self, dataframe: vaex.DataFrame, fit: bool, cache_group: str | None = None, force_recompute: bool = False
     ) -> vaex.DataFrame:
         """Transforms the DataFrame using the transformers in the order they are specified.
 
         Args:
             dataframe: The DataFrame to transform.
+            fit: Whether to fit the transformers on the input data.
             cache_group: The cache group to use.
             force_recompute: Whether to force the recomputation of the transformation.
 
         Returns:
             The transformed DataFrame.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._transform(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+        cache_keys = [self._fingerprint(), (dataframe, VaexFingerprinter())]
+        cached, df = self._cached_execute(
+            lambda_func=lambda: self._transform(dataframe, fit),
+            cache_keys=cache_keys,
             cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
-    def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
+        if fit:
+            self._save_or_load_transformer(cached, cache_group, cache_keys)
+
+            if cached:
+                for transformer, transformer_pkl in zip(self._transformers, self._transformer):
+                    transformer._transformer = transformer_pkl
+
+        return df
+
+    def _transform(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Returns the transformed DataFrame.
 
         Args:
             dataframe: The DataFrame to transform.
+            fit: Whether to fit the transformers on the input data.
 
         Returns:
             The transformed DataFrame.
         """
         for i, transformer in enumerate(self._transformers):
             logger.info(
                 f"Executing composite feature transformation step {i+1}/{len(self._transformers)}: "
                 f"{transformer.__class__.__name__}."
             )
-            dataframe = transformer._transform(dataframe).extract()
+            dataframe = transformer.transform(dataframe, fit).extract()
+            self._transformer.append(transformer._transformer)
             logger.info(f"Finished composite transformation step {i+1}/{len(self._transformers)}.")
         return dataframe
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the transformer.
 
         Returns:
```

### Comparing `mleko-0.6.1/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-0.7.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pathlib import Path
 from typing import Hashable, Literal
 
 import vaex
 import vaex.ml
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
 from .base_transformer import BaseTransformer
 
 
 logger = CustomLogger()
@@ -24,14 +23,15 @@
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...],
         unseen_strategy: Literal["zero", "nan"] = "nan",
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the transformer.
 
         Uses the `vaex.ml.FrequencyEncoder` transformer, which encodes categorical features using the frequency of
         their respective samples. If a value is not seen during fitting, it will be encoded as zero or nan,
         depending on the `unseen_strategy` parameter. Missing values will be encoded as nan, but will still count
         towards the frequency of other values.
@@ -41,14 +41,15 @@
             result in very small frequencies.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the transformer.
             unseen_strategy: Strategy to use for unseen values once the transformer is fitted.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.transform import FrequencyEncoderTransformer
             >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=["a", "b", "c", "d", "e", "f", "g", "h", "i", "j"],
@@ -60,54 +61,45 @@
             ...     features=["a", "b"],
             ... ).transform(df)
             >>> df["a"].tolist()
             [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
             >>> df["b"].tolist()
             [0.4, 0.4, 0.4, 0.4, nan, nan, nan, nan, nan, nan]
         """
-        super().__init__(cache_directory, features, cache_size)
+        super().__init__(cache_directory, features, cache_size, disable_cache)
         self._unseen_strategy = unseen_strategy
+        self._transformer = vaex.ml.FrequencyEncoder(
+            features=self._features, unseen_strategy=self._unseen_strategy, prefix=""
+        )
 
-    def transform(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _transform(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using frequency encoding.
 
-        Will cache the resulting DataFrame in the cache directory.
-
         Args:
             dataframe: The DataFrame to transform.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recomputing the transformation.
+            fit: Whether to fit the transformer on the input data.
 
         Returns:
             The transformed DataFrame.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._transform(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
-        )
+        if fit:
+            self._fit(dataframe)
 
-    def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Transforms the features in the DataFrame using frequency encoding.
+        logger.info(f"Transforming features using frequency encoding ({len(self._features)}): {self._features}.")
+        transformed_df = self._transformer.transform(dataframe)
+        return transformed_df
 
-        Args:
-            dataframe: The DataFrame to transform.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the transformer on the input data.
 
-        Returns:
-            The transformed DataFrame.
+        Args:
+            dataframe: The DataFrame to fit the transformer on.
         """
-        frequency_encoder = vaex.ml.FrequencyEncoder(
-            features=self._features, unseen_strategy=self._unseen_strategy, prefix=""
-        )
-        logger.info(f"Transforming features using frequency encoding ({len(self._features)}): {self._features}.")
-        transformed_df = frequency_encoder.fit_transform(dataframe)
-        return transformed_df
+        logger.info(f"Fitting frequency encoder transformer ({len(self._features)}): {self._features}.")
+        self._transformer.fit(dataframe)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the transformer.
 
         Append the `unseen_strategy` to the fingerprint.
 
         Returns:
```

### Comparing `mleko-0.6.1/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-0.7.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 import vaex.ml
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
 from .base_transformer import BaseTransformer
 
 
 logger = CustomLogger()
@@ -24,14 +23,15 @@
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...],
         allow_unseen: bool = True,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
         """Initializes the transformer.
 
         Uses the `vaex.ml.LabelEncoder` transformer, which encodes categorical features with integer values between 0
         and n_classes-1. If a value is not seen during fitting, it will be encoded as -1, unless `allow_unseen` is
         set to False, in which case an error will be raised.
 
@@ -39,14 +39,15 @@
             Should only be used with categorical features.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the transformer.
             allow_unseen: Whether to allow unseen values once the transformer is fitted.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.transform import LabelEncoderTransformer
             >>> df = vaex.from_arrays(
             ...     a=["a", "b", "c", "d", "e", "f", "g", "h", "i", "j"],
             ...     b=["a", "a", "a", "a", None, None, None, None, None, None],
@@ -58,52 +59,43 @@
             ...     allow_unseen=True,
             ... ).transform(df)
             >>> df["a"].tolist()
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
             >>> df["b"].tolist()
             [1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         """
-        super().__init__(cache_directory, features, cache_size)
+        super().__init__(cache_directory, features, cache_size, disable_cache)
         self._allow_unseen = allow_unseen
+        self._transformer = vaex.ml.LabelEncoder(features=self._features, prefix="")
 
-    def transform(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
+    def _transform(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
         """Transforms the features of the given DataFrame using label encoding.
 
-        Will cache the resulting DataFrame in the cache directory.
-
         Args:
             dataframe: The DataFrame to transform.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recomputation of the transformation.
+            fit: Whether to fit the transformer on the input data.
 
         Returns:
             The transformed DataFrame.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._transform(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
-        )
+        if fit:
+            self._fit(dataframe)
 
-    def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Transforms the features of the given DataFrame using label encoding.
+        logger.info(f"Transforming features using label encoding ({len(self._features)}): {self._features}.")
+        transformed_df = self._transformer.transform(dataframe)
+        return transformed_df
 
-        Args:
-            dataframe: The DataFrame to transform.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the transformer on the given DataFrame.
 
-        Returns:
-            The transformed DataFrame.
+        Args:
+            dataframe: The DataFrame to fit the transformer on.
         """
-        label_encoder = vaex.ml.LabelEncoder(features=self._features, prefix="")
-        logger.info(f"Transforming features using label encoding ({len(self._features)}): {self._features}.")
-        transformed_df = label_encoder.fit_transform(dataframe)
-        return transformed_df
+        logger.info(f"Fitting label encoder transformer ({len(self._features)}): {self._features}.")
+        self._transformer.fit(dataframe)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the transformer.
 
         Appends the `allow_unseen` parameter to the fingerprint of the base class.
 
         Returns:
```

### Comparing `mleko-0.6.1/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-0.7.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,55 @@
-"""Module for the frequency encoder transformer."""
+"""Module for the min-max scaler transformer."""
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 import vaex.ml
 
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
 from .base_transformer import BaseTransformer
 
 
 logger = CustomLogger()
 """A module-level logger for the module."""
 
 
-class MaxAbsScalerTransformer(BaseTransformer):
-    """Transforms features using maximum absolute scaling."""
+class MinMaxScalerTransformer(BaseTransformer):
+    """Transforms features using min-max scaling."""
 
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
         features: list[str] | tuple[str, ...],
+        min_value: float = 0.0,
+        max_value: float = 1.0,
         cache_size: int = 1,
+        disable_cache: bool = False,
     ) -> None:
-        """Initializes the max absolute scaler transformer.
+        """Initializes the min-max scaler transformer.
 
-        The max absolute scaler transformer will scale each feature by its maximum absolute value. This transformer
-        will not shift/center the data, and thus will not destroy any sparsity.
+        The min-max scaler transformer will scale each feature to a given range. If the range is not specified,
+        the range will be [0, 1]. The min-max scaler will not change the data distribution.
 
         Warning:
             Should only be used with numerical features. There should be no missing values in the features
             or an error will be raised.
 
         Args:
             cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the transformer.
+            min_value: The minimum value of the range.
+            max_value: The maximum value of the range.
             cache_size: The maximum number of entries to keep in the cache.
+            disable_cache: Whether to disable caching.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.transform import MaxAbsScalerTransformer
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
             ...     b=[-1, -2, -3, -4, -5, 0, 1, 2, 3, 4]
@@ -54,52 +59,49 @@
             ...     features=["a", "b"],
             ... ).transform(df)
             >>> df["a"].tolist()
             [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
             >>> df["b"].tolist()
             [-0.2, -0.4, -0.6, -0.8, -1.0, 0.0, 0.2, 0.4, 0.6, 0.8]
         """
-        super().__init__(cache_directory, features, cache_size)
-
-    def transform(
-        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
-    ) -> vaex.DataFrame:
-        """Transforms the features in the DataFrame using maximum absolute scaling.
+        super().__init__(cache_directory, features, cache_size, disable_cache)
+        self._min_value = min_value
+        self._max_value = max_value
+        self._transformer = vaex.ml.MinMaxScaler(
+            features=self._features, prefix="", feature_range=(self._min_value, self._max_value)
+        )
 
-        Will cache the resulting DataFrame in the cache directory.
+    def _transform(self, dataframe: vaex.DataFrame, fit: bool) -> vaex.DataFrame:
+        """Transforms the features in the DataFrame using min-max scaling.
 
         Args:
             dataframe: The DataFrame to transform.
-            cache_group: The cache group to use.
-            force_recompute: Whether to force recomputing the transformation.
+            fit: Whether to fit the transformer on the input data.
 
         Returns:
             The transformed DataFrame.
         """
-        return self._cached_execute(
-            lambda_func=lambda: self._transform(dataframe),
-            cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
-            cache_group=cache_group,
-            force_recompute=force_recompute,
-        )
+        if fit:
+            self._fit(dataframe)
 
-    def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
-        """Transforms the features in the DataFrame using maximum absolute scaling.
+        logger.info(f"Transforming features using min-max scaling ({len(self._features)}): {self._features}.")
+        transformed_df = self._transformer.transform(dataframe)
+        return transformed_df
 
-        Args:
-            dataframe: The DataFrame to transform.
+    def _fit(self, dataframe: vaex.DataFrame) -> None:
+        """Fits the transformer on the given DataFrame.
 
-        Returns:
-            The transformed DataFrame.
+        Args:
+            dataframe: The DataFrame to fit the transformer on.
         """
-        max_abs_scaler = vaex.ml.MaxAbsScaler(features=self._features, prefix="")
-        logger.info(f"Transforming features using maximum absolute scaling ({len(self._features)}): {self._features}.")
-        transformed_df = max_abs_scaler.fit_transform(dataframe)
-        return transformed_df
+        logger.info(f"Fitting min-max scaler transformer ({len(self._features)}): {self._features}.")
+        self._transformer.fit(dataframe)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the transformer.
 
+        Appends the min and max values to the fingerprint.
+
         Returns:
             A hashable object that uniquely identifies the transformer.
         """
-        return super()._fingerprint()
+        return super()._fingerprint(), self._min_value, self._max_value
```

### Comparing `mleko-0.6.1/mleko/pipeline/__init__.py` & `mleko-0.7.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/data_container.py` & `mleko-0.7.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/pipeline.py` & `mleko-0.7.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/pipeline_step.py` & `mleko-0.7.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/steps/__init__.py` & `mleko-0.7.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/steps/convert_step.py` & `mleko-0.7.0/mleko/pipeline/steps/convert_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,12 +52,12 @@
             ValueError: If data container contains invalid data - not a list of Paths.
 
         Returns:
             A DataContainer containing the converted data as a vaex dataframe.
         """
         file_paths = data_container.data[self._inputs[0]]
         if not isinstance(file_paths, list) or not all(isinstance(e, Path) for e in file_paths):
-            raise ValueError
+            raise ValueError(f"Invalid data type: {type(file_paths)}. Expected list of Paths.")
 
         df = self._converter.convert(file_paths, self._cache_group, force_recompute)
         data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.6.1/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.7.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,28 +18,31 @@
     _num_outputs = 1
     """Number of outputs expected by the FeatureSelectStep."""
 
     @auto_repr
     def __init__(
         self,
         feature_selector: BaseFeatureSelector,
+        fit: bool,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
         cache_group: str | None = None,
     ) -> None:
         """Initialize the FeatureSelectStep with the specified feature selector.
 
         Args:
             feature_selector: The FeatureSelector responsible for handling feature selection.
+            fit: Whether to fit the feature selector on the input data.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._feature_selector = feature_selector
+        self._fit = fit
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform feature selection using the configured feature selector.
 
         Args:
             data_container: Contains the input DataFrame.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
@@ -48,12 +51,12 @@
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the selected features as a vaex DataFrame.
         """
         dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
-            raise ValueError
+            raise ValueError(f"Invalid data type: {type(dataframe)}. Expected vaex DataFrame.")
 
-        df = self._feature_selector.select_features(dataframe, self._cache_group, force_recompute)
+        df = self._feature_selector.select_features(dataframe, self._fit, self._cache_group, force_recompute)
         data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.6.1/mleko/pipeline/steps/ingest_step.py` & `mleko-0.7.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/pipeline/steps/split_step.py` & `mleko-0.7.0/mleko/pipeline/steps/split_step.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,13 +52,13 @@
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the split data as two vaex DataFrames.
         """
         dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
-            raise ValueError
+            raise ValueError(f"Invalid data type: {type(dataframe)}. Expected vaex DataFrame.")
 
         df1, df2 = self._splitter.split(dataframe, self._cache_group, force_recompute)
         data_container.data[self._outputs[0]] = df1
         data_container.data[self._outputs[1]] = df2
         return data_container
```

### Comparing `mleko-0.6.1/mleko/pipeline/steps/transform_step.py` & `mleko-0.7.0/mleko/pipeline/steps/transform_step.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,28 +18,31 @@
     _num_outputs = 1
     """Number of outputs expected by the TransformStep."""
 
     @auto_repr
     def __init__(
         self,
         transformer: BaseTransformer,
+        fit: bool,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
         cache_group: str | None = None,
     ) -> None:
         """Initialize the TransformStep with the specified transformer.
 
         Args:
             transformer: The Transformer responsible for handling feature transformation.
+            fit: Whether to fit the transformer on the input data.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._transformer = transformer
+        self._fit = fit
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform transformation using the configured transformer.
 
         Args:
             data_container: Contains the input DataFrame.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
@@ -48,12 +51,12 @@
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the selected features as a vaex DataFrame.
         """
         dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
-            raise ValueError
+            raise ValueError(f"Invalid data type: {type(dataframe)}. Expected vaex DataFrame.")
 
-        df = self._transformer.transform(dataframe, self._cache_group, force_recompute)
+        df = self._transformer.transform(dataframe, self._fit, self._cache_group, force_recompute)
         data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.6.1/mleko/utils/__init__.py` & `mleko-0.7.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/utils/custom_logger.py` & `mleko-0.7.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/utils/decorators.py` & `mleko-0.7.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/utils/file_helpers.py` & `mleko-0.7.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/utils/tqdm_helpers.py` & `mleko-0.7.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/mleko/utils/vaex_helpers.py` & `mleko-0.7.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.6.1/pyproject.toml` & `mleko-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.6.1"
+version = "0.7.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
@@ -18,14 +18,16 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11.dev0"
 boto3 = "^1.26.91"
 botocore = "^1.29.91"
 tqdm = "^4.65.0"
 vaex = "^4.16.0"
 scikit-learn = "^1.2.2"
+joblib = "^1.3.1"
+pandas = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 boto3-stubs = {extras = ["s3"], version = "^1.26.91"}
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `mleko-0.6.1/PKG-INFO` & `mleko-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.6.1
+Version: 0.7.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8,<3.11.dev0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
 Requires-Dist: botocore (>=1.29.91,<2.0.0)
+Requires-Dist: joblib (>=1.3.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: vaex (>=4.16.0,<5.0.0)
 Project-URL: Changelog, https://github.com/ErikBavenstrand/mleko/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://mleko.readthedocs.io
 Project-URL: Repository, https://github.com/ErikBavenstrand/mleko
 Description-Content-Type: text/markdown
```

