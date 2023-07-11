# Comparing `tmp/triad-0.9.0.tar.gz` & `tmp/triad-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.9.0.tar", last modified: Tue Jun  6 07:04:41 2023, max compression
+gzip compressed data, was "triad-0.9.1.tar", last modified: Tue Jul 11 07:01:00 2023, max compression
```

## Comparing `triad-0.9.0.tar` & `triad-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.876869 triad-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 07:04:05.000000 triad-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-06 07:04:41.876869 triad-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-06 07:04:05.000000 triad-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 07:04:41.876869 triad-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-06 07:04:05.000000 triad-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.864869 triad-0.9.0/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-06 07:04:05.000000 triad-0.9.0/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.868869 triad-0.9.0/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 07:04:05.000000 triad-0.9.0/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-06 07:04:05.000000 triad-0.9.0/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.872869 triad-0.9.0/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/batch_reslicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.868869 triad-0.9.0/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.872869 triad-0.9.0/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 07:04:05.000000 triad-0.9.0/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.769259 triad-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 07:00:09.000000 triad-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-11 07:01:00.769259 triad-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-11 07:00:09.000000 triad-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 07:01:00.769259 triad-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-11 07:00:09.000000 triad-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.761258 triad-0.9.1/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 07:00:09.000000 triad-0.9.1/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.765259 triad-0.9.1/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 07:00:09.000000 triad-0.9.1/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-11 07:00:09.000000 triad-0.9.1/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-11 07:00:09.000000 triad-0.9.1/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-11 07:00:09.000000 triad-0.9.1/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-07-11 07:00:09.000000 triad-0.9.1/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 07:00:09.000000 triad-0.9.1/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-11 07:00:09.000000 triad-0.9.1/triad/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 07:00:09.000000 triad-0.9.1/triad/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.769259 triad-0.9.1/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/batch_reslicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-11 07:00:09.000000 triad-0.9.1/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.765259 triad-0.9.1/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-11 07:01:00.000000 triad-0.9.1/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-11 07:01:00.000000 triad-0.9.1/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:01:00.000000 triad-0.9.1/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 07:01:00.000000 triad-0.9.1/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 07:01:00.000000 triad-0.9.1/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:01:00.769259 triad-0.9.1/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 07:00:09.000000 triad-0.9.1/triad_version/__init__.py
```

### Comparing `triad-0.9.0/LICENSE` & `triad-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/PKG-INFO` & `triad-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,20 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.9.1
+        
+        * Add `fsspec` as a core dependency, add io utils
+        * Add `py.typed`
+        * Improve `Schema` class comments
+        
         ### 0.9.0
         
         * Merge QPD pandas utils functions back to Triad
         
         ### 0.8.9
         
         * Add batch reslicers
```

### Comparing `triad-0.9.0/README.md` & `triad-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.9.1
+
+* Add `fsspec` as a core dependency, add io utils
+* Add `py.typed`
+* Improve `Schema` class comments
+
 ### 0.9.0
 
 * Merge QPD pandas utils functions back to Triad
 
 ### 0.8.9
 
 * Add batch reslicers
```

### Comparing `triad-0.9.0/setup.py` & `triad-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="triad",
     version=__version__,
     packages=find_packages(include=["triad*"]),
+    package_data={"triad": ["py.typed"]},
     description="A collection of python utils for Fugue projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="fugue util utils utility utilities",
     url="http://github.com/fugue-project/triad",
     install_requires=[
         "numpy",
         "pandas>=1.2.0",
         "six",
         "pyarrow",
-        "fs",
+        "fsspec",
+        "fs",  # TODO: remove this hard dependency
         "importlib-metadata; python_version < '3.8'",
     ],
     extras_require={"ciso8601": ["ciso8601"]},
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `triad-0.9.0/triad/collections/dict.py` & `triad-0.9.1/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/collections/fs.py` & `triad-0.9.1/triad/collections/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 
 class FileSystem(MountFS):
     """A unified filesystem based on PyFileSystem2. The special requirement
     for this class is that all paths must be absolute path with scheme.
     To customize different file systems, you should override `create_fs`
     to provide your own configured file systems.
 
+    :param auto_close: If `True` (the default), the child filesystems
+        will be closed when `MountFS` is closed.
+
     .. admonition:: Examples
 
         .. code-block:: python
 
             fs = FileSystem()
             fs.writetext("mem://from/a.txt", "hello")
             fs.copy("mem://from/a.txt", "mem://to/a.txt")
 
     .. note::
 
         If a path is not a local path, it must include the scheme and `netloc`
         (the first element after `://`)
-        :param auto_close: If `True` (the default), the child filesystems
-        will be closed when `MountFS` is closed.
     """
 
     def __init__(self, auto_close: bool = True):
         super().__init__(auto_close)
         self._fs_store: Dict[str, FSBase] = {}
         self._in_create = False
         self._fs_lock = RLock()
```

### Comparing `triad-0.9.0/triad/collections/function_wrapper.py` & `triad-0.9.1/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/collections/schema.py` & `triad-0.9.1/triad/collections/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -142,40 +142,80 @@
     def pd_dtype(self) -> Dict[str, np.dtype]:
         """convert as `dtype` dict for pandas dataframes.
         Currently, struct type is not supported
         """
         return self.pandas_dtype
 
     def assert_not_empty(self) -> "Schema":
+        """Raise exception if schema is empty"""
         if len(self) > 0:
             return self
         raise SchemaError("Schema can't be empty")
 
     def copy(self) -> "Schema":
         """Clone Schema object
 
         :return: cloned object
         """
         other = super().copy()
         assert isinstance(other, Schema)
         return other
 
     def __repr__(self) -> str:
+        """Convert to the string representation of the schema"""
         return schema_to_expression(self.pyarrow_schema)
 
     def __iadd__(self, obj: Any) -> "Schema":
+        """Append a schema like object to the current schema
+
+        :param obj: a schema like object
+
+        .. admonition:: Examples
+
+            .. code-block:: python
+
+                s = Schema("a:int,b:str")
+                s += "c:long"
+                s += ("d",int)
+        """
         return self.append(obj)
 
     def __isub__(self, obj: Any) -> "Schema":
+        """Remove columns from a schema is not allowed"""
         raise SchemaError("'-=' is not allowed for Schema")
 
     def __add__(self, obj: Any) -> "Schema":
+        """Add a schema like object to the current schema
+
+        :param obj: a schema like object
+
+        .. admonition:: Examples
+
+            .. code-block:: python
+
+                s = Schema("a:int,b:str")
+                s = s + "c:long" +  ("d",int)
+        """
         return self.copy().append(obj)
 
     def __sub__(self, obj: Any) -> "Schema":
+        """Remove columns or schema from the schema.
+
+        :param obj: one column name, a list/set of column names or
+            a schema like object
+        :return: a schema excluding the columns in ``obj``
+
+        .. note::
+
+            If ``obj`` violates any of the following conditions, ``SchemaError``
+            will be raised:
+
+            * all columns in ``obj`` must be found in the schema
+            * If ``obj`` is a schema like object, the types must also match
+        """
         return self.remove(
             obj,
             ignore_key_mismatch=False,
             require_type_match=True,
             ignore_type_mismatch=False,
         )
 
@@ -195,25 +235,36 @@
             value = pa.field(name, to_pa_datatype(value))
         assert_or_throw(
             is_supported(value.type), SchemaError(f"{value} is not supported")
         )
         super().__setitem__(name, value, *args, **kwds)  # type: ignore
 
     def __eq__(self, other: Any) -> bool:
+        """Check if the two schemas are equal
+
+        :param other: a schema like object
+        :return: True if the two schemas are equal
+        """
         if other is None:
             return False
         if other is self:
             return True
         if isinstance(other, Schema):
             return super().__eq__(other)
         if isinstance(other, str):
             return self.__repr__() == other
         return self == Schema(other)
 
     def __contains__(self, key: Any) -> bool:  # noqa: C901
+        """Check if the schema contains the key.
+
+        :param key: a column name, a list of column names, a data
+            type like object or a schema like object
+        :return: True if the schema contains the object
+        """
         if key is None:
             return False
         if isinstance(key, str):
             if ":" not in key:
                 return super().__contains__(key)
         elif isinstance(key, pa.Field):
             res = super().get(key.name, None)
@@ -269,14 +320,28 @@
     def remove(  # noqa: C901
         self,
         obj: Any,
         ignore_key_mismatch: bool = False,
         require_type_match: bool = True,
         ignore_type_mismatch: bool = False,
     ) -> "Schema":
+        """Remove columns or schema from the schema
+
+        :param obj: one column name, a list/set of column names or
+            a schema like object
+        :param ignore_key_mismatch: if True, ignore the non-existing keys,
+            default False
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :param ignore_type_mismatch: if False, when keys match but types don't
+            (if ``obj`` contains type), raise an exception ``SchemaError``,
+            default False
+        :return: a schema excluding the columns in ``obj``
+        """
         if obj is None:
             return self.copy()
         target = self
         if isinstance(obj, str):
             if ":" in obj:  # expression
                 ps = expression_to_schema(obj)
                 pairs: List[Tuple[str, pa.DataType]] = list(zip(ps.names, ps.types))
@@ -311,15 +376,17 @@
         for k, v in pairs:
             # k = k.strip()
             # if k == "":
             #    continue
             if k not in od:
                 if ignore_key_mismatch:
                     continue
-                raise SchemaError(f"Can't remove {quote_name(k)} from {target}")
+                raise SchemaError(
+                    f"Can't remove {quote_name(k)} from {target} (not found)"
+                )
             if v is None:
                 del od[k]
             else:
                 tp = od[k].type
                 if not require_type_match or tp == v:
                     del od[k]
                 elif not ignore_type_mismatch:
@@ -331,14 +398,28 @@
     def extract(  # noqa: C901
         self,
         obj: Any,
         ignore_key_mismatch: bool = False,
         require_type_match: bool = True,
         ignore_type_mismatch: bool = False,
     ) -> "Schema":
+        """Extract a sub schema from the schema based on the columns in ``obj``
+
+        :param obj: one column name, a list/set of column names or
+            a schema like object
+        :param ignore_key_mismatch: if True, ignore the non-existing keys,
+            default False
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :param ignore_type_mismatch: if False, when keys match but types don't
+            (if ``obj`` contains type), raise an exception ``SchemaError``,
+            default False
+        :return: a sub-schema containing the columns in ``obj``
+        """
         if obj is None:
             return Schema()
         if isinstance(obj, str):
             if ":" in obj:  # expression
                 ps = expression_to_schema(obj)
                 pairs: List[Tuple[str, pa.DataType]] = list(zip(ps.names, ps.types))
             else:
@@ -389,28 +470,58 @@
 
     def exclude(
         self,
         other: Any,
         require_type_match: bool = True,
         ignore_type_mismatch: bool = False,
     ) -> "Schema":
+        """Exclude columns from the current schema which are also in ``other``.
+        ``other`` can contain columns that are not in the current schema, they
+        will be ignored.
+
+        :param other: one column name, a list/set of column names or
+            a schema like object
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :param ignore_type_mismatch: if False, when keys match but types don't
+            (if ``obj`` contains type), raise an exception ``SchemaError``,
+            default False
+        :return: a schema excluding the columns in ``other``
+        """
         return self.remove(
             other,
             ignore_key_mismatch=True,
             require_type_match=require_type_match,
             ignore_type_mismatch=ignore_type_mismatch,
         )
 
     def intersect(
         self,
         other: Any,
         require_type_match: bool = True,
         ignore_type_mismatch: bool = True,
         use_other_order: bool = False,
     ) -> "Schema":
+        """Extract the sub-schema from the current schema which are also in
+        ``other``. ``other`` can contain columns that are not in the current schema,
+        they will be ignored.
+
+        :param other: one column name, a list/set of column names or
+            a schema like object
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :param ignore_type_mismatch: if False, when keys match but types don't
+            (if ``obj`` contains type), raise an exception ``SchemaError``,
+            default False
+        :param use_other_order: if True, the output schema will use the column order
+            of ``other``, default False
+        :return: the intersected schema
+        """
         if not use_other_order:
             diff = self.exclude(
                 other,
                 require_type_match=require_type_match,
                 ignore_type_mismatch=ignore_type_mismatch,
             )
             return self - diff
@@ -418,17 +529,33 @@
             return self.extract(
                 other,
                 require_type_match=require_type_match,
                 ignore_type_mismatch=ignore_type_mismatch,
             )
 
     def union(self, other: Any, require_type_match: bool = False) -> "Schema":
+        """Union the ``other`` schema
+
+        :param other: a schema like object
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :return: the new unioned schema
+        """
         return self.copy().union_with(other, require_type_match=require_type_match)
 
     def union_with(self, other: Any, require_type_match: bool = False) -> "Schema":
+        """Union the ``other`` schema into the current schema
+
+        :param other: a schema like object
+        :param require_type_match: if True, a match requires the same key
+            and same type (if ``obj`` contains type), otherwise, only the
+            key needs to match, default True
+        :return: the current schema
+        """
         if not isinstance(other, Schema):
             other = Schema(other)
         try:
             other = other.exclude(
                 self, require_type_match=require_type_match, ignore_type_mismatch=False
             )
             self += other
```

### Comparing `triad-0.9.0/triad/utils/assertion.py` & `triad-0.9.1/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/batch_reslicers.py` & `triad-0.9.1/triad/utils/batch_reslicers.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/class_extension.py` & `triad-0.9.1/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/convert.py` & `triad-0.9.1/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/dispatcher.py` & `triad-0.9.1/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/entry_points.py` & `triad-0.9.1/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/hash.py` & `triad-0.9.1/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/iter.py` & `triad-0.9.1/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/json.py` & `triad-0.9.1/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/pandas_like.py` & `triad-0.9.1/triad/utils/pandas_like.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/pyarrow.py` & `triad-0.9.1/triad/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/rename.py` & `triad-0.9.1/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/schema.py` & `triad-0.9.1/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad/utils/string.py` & `triad-0.9.1/triad/utils/string.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 def validate_triad_var_name(expr: str) -> bool:
-    """Check if `expr` is a valid Triad variable name based on Triad standard:
+    """Check if ``expr`` is a valid Triad variable name based on Triad standard:
     it has to be a valid python identifier and it can't be purely ``_``
 
     .. note::
 
-        Any valid triad var name can be used as column names without quote ````
+        Any valid triad var name can be used as column names without quote ` `
 
     :param expr: column name expression
     :return: whether it is valid
     """
     if not isinstance(expr, str) or not expr.isidentifier() or not expr.isascii():
         return False
     return expr.strip("_") != ""
 
 
 def assert_triad_var_name(expr: str) -> str:
-    """Check if `expr` is a valid Triad variable name based on Triad standard:
-    it has to be a valid python identifier and it can't be purely `_`
+    """Check if ``expr`` is a valid Triad variable name based on Triad standard:
+    it has to be a valid python identifier and it can't be purely ``_``
+
     :param expr: column name expression
     :raises AssertionError: if the expression is invalid
     :return: the expression string
     """
     if validate_triad_var_name(expr):
         return expr
     raise AssertionError(f"{expr} is not a valid Triad variable name")
```

### Comparing `triad-0.9.0/triad/utils/threading.py` & `triad-0.9.1/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.9.0/triad.egg-info/PKG-INFO` & `triad-0.9.1/triad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,20 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.9.1
+        
+        * Add `fsspec` as a core dependency, add io utils
+        * Add `py.typed`
+        * Improve `Schema` class comments
+        
         ### 0.9.0
         
         * Merge QPD pandas utils functions back to Triad
         
         ### 0.8.9
         
         * Add batch reslicers
```

### Comparing `triad-0.9.0/triad.egg-info/SOURCES.txt` & `triad-0.9.1/triad.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 triad/__init__.py
 triad/constants.py
 triad/exceptions.py
+triad/py.typed
 triad.egg-info/PKG-INFO
 triad.egg-info/SOURCES.txt
 triad.egg-info/dependency_links.txt
 triad.egg-info/requires.txt
 triad.egg-info/top_level.txt
 triad/collections/__init__.py
 triad/collections/dict.py
@@ -19,14 +20,15 @@
 triad/utils/assertion.py
 triad/utils/batch_reslicers.py
 triad/utils/class_extension.py
 triad/utils/convert.py
 triad/utils/dispatcher.py
 triad/utils/entry_points.py
 triad/utils/hash.py
+triad/utils/io.py
 triad/utils/iter.py
 triad/utils/json.py
 triad/utils/pandas_like.py
 triad/utils/pyarrow.py
 triad/utils/rename.py
 triad/utils/schema.py
 triad/utils/string.py
```

