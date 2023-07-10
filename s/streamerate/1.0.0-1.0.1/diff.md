# Comparing `tmp/streamerate-1.0.0-py3-none-any.whl.zip` & `tmp/streamerate-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18199 bytes, number of entries: 7
+Zip file size: 18246 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      161 b- defN 23-May-06 10:55 streamerate/__init__.py
--rw-rw-rw-  2.0 fat    58469 b- defN 23-May-06 11:21 streamerate/streams.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-May-06 11:51 streamerate-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14392 b- defN 23-May-06 11:51 streamerate-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 11:51 streamerate-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-06 11:51 streamerate-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      566 b- defN 23-May-06 11:51 streamerate-1.0.0.dist-info/RECORD
-7 files, 74781 bytes uncompressed, 17197 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat    59008 b- defN 23-Jul-10 22:07 streamerate/streams.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-10 22:18 streamerate-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14392 b- defN 23-Jul-10 22:18 streamerate-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 22:18 streamerate-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-10 22:18 streamerate-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      566 b- defN 23-Jul-10 22:18 streamerate-1.0.1.dist-info/RECORD
+7 files, 75320 bytes uncompressed, 17244 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: streamerate/__init__.py
 Comment: 
 
 Filename: streamerate/streams.py
 Comment: 
 
-Filename: streamerate-1.0.0.dist-info/LICENSE
+Filename: streamerate-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: streamerate-1.0.0.dist-info/METADATA
+Filename: streamerate-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: streamerate-1.0.0.dist-info/WHEEL
+Filename: streamerate-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: streamerate-1.0.0.dist-info/top_level.txt
+Filename: streamerate-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: streamerate-1.0.0.dist-info/RECORD
+Filename: streamerate-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamerate/streams.py

```diff
@@ -357,14 +357,19 @@
         else:
             for el in itr:
                 m_el = f(el)
                 if m_el not in st:
                     st.add(m_el)
                     yield el
 
+    def __add_observer_generator(self, observer: Callable[[_K], None]) -> Iterator[_K]:
+        for el in self:
+            observer(el)
+            yield el
+
     def map(self, f: Callable[[_K], _V]) -> 'stream[_V]':
         return stream(partial(map, f, self))
 
     def starmap(self, f: Callable[[_K], _V]) -> 'stream[_V]':
         return stream(partial(itertools.starmap, f, self))
 
     def mpmap(self, f: Callable[[_K], _V], poolSize: int = cpu_count(),
@@ -485,15 +490,14 @@
         It spawns at most poolSize threads and applies the f function.
         The elements in the result stream appears in the same order as at input.
         It's most usefull for I/O or CPU intensive consuming functions.
         :param poolSize: number of threads to spawn
         """
         return self.mtmap(lambda el: f(*el), poolSize, bufferSize)
 
-    # ToDo - add fastFlatMap to Python 2.x version
     def fastFlatMap(self, predicate: Callable[[_K], Iterable[_V]] = _IDENTITY_FUNC, poolSize: int = cpu_count(),
                     bufferSize: Optional[int] = None) -> 'stream[_V]':
         if not isinstance(poolSize, int) or poolSize <= 0 or poolSize > 2 ** 12:
             raise ValueError("poolSize should be an integer between 1 and 2^12. Received: %s" % str(poolSize))
         elif poolSize == 1:
             return self.flatMap(predicate)
         if bufferSize is None:
@@ -514,14 +518,25 @@
             By default predicate is an identity function
         :return: will return stream of objects of the same type of elements from the stream returned by predicate()
         """
         if id(predicate) == id(_IDENTITY_FUNC):
             return stream(ItrFromFunc(lambda: itertools.chain.from_iterable(self)))
         return stream(ItrFromFunc(lambda: itertools.chain.from_iterable(self.map(predicate))))
 
+    def for_each(self, f: Callable[[_K], None]) -> None:
+        for el in self:
+            f(el)
+
+    def add_observer(self, f: Callable[[_K], None]) -> 'stream[_K]':
+        """
+        :param f: f is observer that will receive elements of self collection and return None
+        :return: will return stream of objects of the same type of elements from the stream
+        """
+        return stream(ItrFromFunc(lambda: self.__add_observer_generator(f)))
+
     def filter(self, predicate: Optional[Callable[[_K], bool]] = None) -> 'stream[_K]':
         """
         :param predicate: If predicate is None, return the items that are true.
         """
         return stream(ItrFromFunc(lambda: filter(predicate, self)))
 
     def starfilter(self, predicate: Callable[[_K], bool]) -> 'stream[_K]':
@@ -769,15 +784,14 @@
                 batch = slist(itertools.islice(itr, 0, size))
                 if not batch:
                     break
                 yield batch
 
         return stream(lambda: stream(batch_gen(iter(self))))
 
-    # ToDo - add this fix to Python 2.7
     def take(self, n: int) -> 'stream[_K]':
         def gen(other_gen: GeneratorType, n):
             count = 0
             while count < n:
                 if count < n:
                     try:
                         el = next(other_gen)
```

## Comparing `streamerate-1.0.0.dist-info/LICENSE` & `streamerate-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `streamerate-1.0.0.dist-info/METADATA` & `streamerate-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamerate
-Version: 1.0.0
+Version: 1.0.1
 Summary: streamerate: a fluent and expressive Python library for chainable iterable processing, inspired by Java 8 streams.
 Home-page: https://github.com/asuiu/streamerate
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: MIT
 Keywords: stream itertools fluent functional chainable iterable processing
 Classifier: Development Status :: 5 - Production/Stable
```

