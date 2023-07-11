# Comparing `tmp/fastbloom_rs-0.5.3-cp37-abi3-win_amd64.whl.zip` & `tmp/fastbloom_rs-0.5.4-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 176556 bytes, number of entries: 7
--rw-r--r--  4.6 unx    22045 b- defN 23-Feb-17 06:15 fastbloom_rs-0.5.3.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Feb-17 06:15 fastbloom_rs-0.5.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     4997 b- defN 23-Feb-17 06:15 fastbloom_rs/fastbloom_rs.pyi
--rw-r--r--  4.6 unx    23553 b- defN 23-Feb-17 06:15 fastbloom_rs/filter.py
--rw-r--r--  4.6 unx      315 b- defN 23-Feb-17 06:15 fastbloom_rs/__init__.py
--rwxr-xr-x  4.6 unx   425472 b- defN 23-Feb-17 06:15 fastbloom_rs/fastbloom_rs.pyd
--rw-r--r--  4.6 unx      556 b- defN 23-Feb-17 06:15 fastbloom_rs-0.5.3.dist-info/RECORD
-7 files, 477033 bytes uncompressed, 175582 bytes compressed:  63.2%
+Zip file size: 182683 bytes, number of entries: 7
+-rw-r--r--  4.6 unx    22045 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     5232 b- defN 23-Jul-11 14:58 fastbloom_rs/fastbloom_rs.pyi
+-rw-r--r--  4.6 unx    24510 b- defN 23-Jul-11 14:58 fastbloom_rs/filter.py
+-rw-r--r--  4.6 unx      315 b- defN 23-Jul-11 14:58 fastbloom_rs/__init__.py
+-rwxr-xr-x  4.6 unx   458240 b- defN 23-Jul-11 14:58 fastbloom_rs/fastbloom_rs.pyd
+-rw-r--r--  4.6 unx      556 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/RECORD
+7 files, 510993 bytes uncompressed, 181709 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: fastbloom_rs-0.5.3.dist-info/METADATA
+Filename: fastbloom_rs-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: fastbloom_rs-0.5.3.dist-info/WHEEL
+Filename: fastbloom_rs-0.5.4.dist-info/WHEEL
 Comment: 
 
 Filename: fastbloom_rs/fastbloom_rs.pyi
 Comment: 
 
 Filename: fastbloom_rs/filter.py
 Comment: 
 
 Filename: fastbloom_rs/__init__.py
 Comment: 
 
 Filename: fastbloom_rs/fastbloom_rs.pyd
 Comment: 
 
-Filename: fastbloom_rs-0.5.3.dist-info/RECORD
+Filename: fastbloom_rs-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastbloom_rs/fastbloom_rs.pyi

```diff
@@ -32,26 +32,35 @@
 class PyBloomFilter(object):
     def add(self, element: Union[str, int, bytes]):
         ...
 
     def add_int(self, element: int):
         ...
 
+    def add_int_if_not_contains(self, element: int) -> bool:
+        ...
+
     def add_int_batch(self, array: Sequence[int]):
         ...
 
     def add_str(self, element: str):
         ...
 
+    def add_str_if_not_contains(self, element: str) -> bool:
+        ...
+
     def add_str_batch(self, array: Sequence[str]):
         ...
 
     def add_bytes(self, element: bytes):
         ...
 
+    def add_bytes_if_not_contains(self, element: bytes) -> bool:
+        ...
+
     def add_bytes_batch(self, elements: Sequence[bytes]):
         ...
 
     def contains(self, element: Union[str, int, bytes]) -> bool:
         ...
 
     def contains_int(self, element: int) -> bool:
```

## fastbloom_rs/filter.py

```diff
@@ -112,14 +112,32 @@
         elif isinstance(element, str):
             self._py_bloom.add_str(element)
         elif isinstance(element, bytes):
             self._py_bloom.add_bytes(element)
         else:
             self._py_bloom.add_str(str(element))
 
+    def add_if_not_contains(self, element: Union[str, int, bytes]) -> bool:
+        """
+        Tests whether an element is present in the filter (subject to the specified false positive rate).
+        And if it is not in this filter, add it to the filter.
+
+        :param element: value to test
+        :return: “False” if this element did not exist in the Bloom filter before, and then this method will insert
+        this element into the current filter. “True” if the element is already in the Bloom filter.
+        """
+        if isinstance(element, int):
+            return self._py_bloom.add_int_if_not_contains(element)
+        elif isinstance(element, str):
+            return self._py_bloom.add_str_if_not_contains(element)
+        elif isinstance(element, bytes):
+            return self._py_bloom.add_bytes_if_not_contains(element)
+        else:
+            return self._py_bloom.add_str_if_not_contains(str(element))
+
     def add_int(self, element: int):
         """
         Add element to the filter.
 
         :param element: value to add
         :return:
         """
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `fastbloom_rs-0.5.3.dist-info/METADATA` & `fastbloom_rs-0.5.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastbloom_rs
-Version: 0.5.3
+Version: 0.5.4
 Classifier: Programming Language :: Python
 Requires-Dist: pytest <= 7.1.1; extra == 'test'
 Requires-Dist: pybloom_live; extra == 'test'
 Provides-Extra: test
 Summary: Some fast bloom filter implemented by Rust for Python and Rust! 10x faster than pybloom!
 Keywords: bloom-filter,bloom,filter,bloomfilter,probabilistic data structure,counting-bloom-filter
 Home-Page: https://github.com/yankun1992/fastbloom
```

