# Comparing `tmp/json-any-2023.1.tar.gz` & `tmp/json-any-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.1.tar", last modified: Tue Jul 11 10:52:33 2023, max compression
+gzip compressed data, was "json-any-2023.2.tar", last modified: Tue Jul 11 12:02:21 2023, max compression
```

## Comparing `json-any-2023.1.tar` & `json-any-2023.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.1/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 10:52:33.441800 json-any-2023.1/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.1/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.1/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.438467 json-any-2023.1/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.1/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1744 2023-07-10 12:40:50.000000 json-any-2023.1/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.1/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.1/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     2882 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     9304 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.1/json_any/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)    14277 2023-07-11 10:47:37.000000 json-any-2023.1/json_any/object_to_json.py
--rw-r--r--   0 eric      (1000) users      (984)     3666 2023-07-11 09:56:39.000000 json-any-2023.1/json_any/type.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-10 17:21:22.000000 json-any-2023.1/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 10:52:33.441800 json-any-2023.1/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      441 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-11 10:52:33.000000 json-any-2023.1/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.1/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-11 10:52:33.441800 json-any-2023.1/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5261 2023-07-11 10:51:15.000000 json-any-2023.1/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.2/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 12:02:21.904978 json-any-2023.2/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.2/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.2/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.901645 json-any-2023.2/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.2/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1754 2023-07-11 10:57:55.000000 json-any-2023.2/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.2/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.2/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     2895 2023-07-11 10:56:35.000000 json-any-2023.2/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.2/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     3666 2023-07-11 09:56:39.000000 json-any-2023.2/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     9324 2023-07-11 10:59:14.000000 json-any-2023.2/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    14297 2023-07-11 10:59:29.000000 json-any-2023.2/json_any/object_to_json.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-11 11:01:55.000000 json-any-2023.2/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-11 12:02:21.904978 json-any-2023.2/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-11 12:02:21.000000 json-any-2023.2/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-11 12:02:21.000000 json-any-2023.2/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-11 12:02:21.000000 json-any-2023.2/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-11 12:02:21.000000 json-any-2023.2/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.2/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-11 12:02:21.904978 json-any-2023.2/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.2/setup.py
```

### Comparing `json-any-2023.1/PKG-INFO` & `json-any-2023.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.1
+Version: 2023.2
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.1/README-LICENCE-utf8.txt` & `json-any-2023.2/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/README.rst` & `json-any-2023.2/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/documentation/wiki/description.asciidoc` & `json-any-2023.2/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/json_any/__init__.py` & `json-any-2023.2/json_any/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from json_any.extension.type import FullyQualifiedType
 from json_any.json_to_object import ObjectFromJsonString
 from json_any.object_to_json import JsonStringOf
-from json_any.type import FullyQualifiedType
 from json_any.version import __version__
```

### Comparing `json-any-2023.1/json_any/catalog/module.py` & `json-any-2023.2/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/json_any/catalog/type.py` & `json-any-2023.2/json_any/catalog/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/json_any/constant.py` & `json-any-2023.2/json_any/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 STANDARD_PREFIX = "STANDARD_"
 UNHANDLED_PREFIX = "UNHANDLED_"
 
 JSON_TYPE_PREFIX_NETWORKX = "networkx_"
 JSON_TYPE_PREFIX_PANDAS = "pandas_"
 JSON_TYPE_PREFIX_PATHLIB = "pathlib_"
 JSON_TYPE_PREFIX_SCIPY = "scipy_"
-# For data_frame_t and series_t, use "frame" and "series" since it is used for
-# pandas.read_json's "typ" parameter.
+# For data_frame_t and series_t, use "frame" and "series" as postfixes since it is used
+# for pandas.read_json's "typ" parameter.
 JSON_TYPE = {
     array_t: "numpy_ndarray",
     data_frame_t: f"{JSON_TYPE_PREFIX_PANDAS}frame",
     date_t: "datetime_date",
     date_time_t: "datetime_datetime",
     enum_t: "enum_Enum_",
     figure_t: "matplotlib_pyplot_Figure",
```

### Comparing `json-any-2023.1/json_any/json_to_object.py` & `json-any-2023.2/json_any/json_to_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     JSON_TYPE_PREFIX_PANDAS,
     JSON_TYPE_PREFIX_PATHLIB,
     JSON_TYPE_PREFIX_SCIPY,
     NEW_FROM_JSON_DESCRIPTION,
     STANDARD_PREFIX,
     UNHANDLED_PREFIX,
 )
-from json_any.numpy import AsNumpyArray
-from json_any.type import TypeFromJsonType, builders_h, description_h
+from json_any.extension.numpy import AsNumpyArray
+from json_any.extension.type import TypeFromJsonType, builders_h, description_h
 
 
 def ObjectFromJsonString(jsoned: str, /, *, builders: builders_h = None) -> Any:
     """"""
     return _ObjectFromUnJSONed(
         json.loads(jsoned), highest_level_call=True, builders=builders
     )
```

### Comparing `json-any-2023.1/json_any/numpy.py` & `json-any-2023.2/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/json_any/object_to_json.py` & `json-any-2023.2/json_any/object_to_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
     JSON_TYPE_PREFIX_NETWORKX,
     JSON_TYPE_PREFIX_PATHLIB,
     JSON_TYPE_PREFIX_SCIPY,
     JSONING_ERROR_MARKER,
     STANDARD_PREFIX,
     UNHANDLED_PREFIX,
 )
-from json_any.numpy import AsMostConciseRepresentation
-from json_any.type import (
+from json_any.extension.numpy import AsMostConciseRepresentation
+from json_any.extension.type import (
     FullyQualifiedType,
     IsFullyDataclassBased,
     IsNamedTuple,
     TypeOfInstance,
     description_h,
     descriptors_h,
 )
```

### Comparing `json-any-2023.1/json_any/type.py` & `json-any-2023.2/json_any/extension/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.1/json_any/version.py` & `json-any-2023.2/json_any/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.1"
+__version__ = "2023.2"
```

### Comparing `json-any-2023.1/json_any.egg-info/PKG-INFO` & `json-any-2023.2/json_any.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.1
+Version: 2023.2
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.1/setup.py` & `json-any-2023.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 PYPI_AUDIENCE = "Developers"
 PYPI_STATUS = "4 - Beta"
 
 IMPORT_NAME = "json_any"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
+    f"{IMPORT_NAME}.extension",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
 )
 ENTRY_POINTS = {
     "console_scripts": [],
 }
```

