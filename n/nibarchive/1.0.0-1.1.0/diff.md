# Comparing `tmp/nibarchive-1.0.0.tar.gz` & `tmp/nibarchive-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibarchive-1.0.0.tar", last modified: Mon Jul 10 19:26:08 2023, max compression
+gzip compressed data, was "nibarchive-1.1.0.tar", last modified: Tue Jul 11 14:31:28 2023, max compression
```

## Comparing `nibarchive-1.0.0.tar` & `nibarchive-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 19:26:08.396077 nibarchive-1.0.0/
--rw-rw-rw-   0        0        0    35803 2023-07-10 19:21:37.000000 nibarchive-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4012 2023-07-10 19:26:08.397074 nibarchive-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3291 2023-07-10 19:21:37.000000 nibarchive-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 19:26:08.292071 nibarchive-1.0.0/nibarchive/
--rw-rw-rw-   0        0        0       44 2023-07-10 19:21:37.000000 nibarchive-1.0.0/nibarchive/__init__.py
--rw-rw-rw-   0        0        0     8423 2023-07-10 19:21:37.000000 nibarchive-1.0.0/nibarchive/model.py
--rw-rw-rw-   0        0        0    10073 2023-07-10 19:21:37.000000 nibarchive-1.0.0/nibarchive/parse.py
-drwxrwxrwx   0        0        0        0 2023-07-10 19:26:08.379070 nibarchive-1.0.0/nibarchive.egg-info/
--rw-rw-rw-   0        0        0     4012 2023-07-10 19:26:07.000000 nibarchive-1.0.0/nibarchive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-10 19:26:08.000000 nibarchive-1.0.0/nibarchive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 19:26:07.000000 nibarchive-1.0.0/nibarchive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 19:26:07.000000 nibarchive-1.0.0/nibarchive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      850 2023-07-10 19:21:37.000000 nibarchive-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 19:26:08.405094 nibarchive-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 14:31:28.061594 nibarchive-1.1.0/
+-rw-rw-rw-   0        0        0    35803 2023-07-10 19:21:37.000000 nibarchive-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4013 2023-07-11 14:31:28.062594 nibarchive-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3292 2023-07-11 14:19:18.000000 nibarchive-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 14:31:27.974101 nibarchive-1.1.0/nibarchive/
+-rw-rw-rw-   0        0        0       44 2023-07-10 19:21:37.000000 nibarchive-1.1.0/nibarchive/__init__.py
+-rw-rw-rw-   0        0        0    10724 2023-07-11 14:21:54.000000 nibarchive-1.1.0/nibarchive/__main__.py
+-rw-rw-rw-   0        0        0     8182 2023-07-11 06:21:14.000000 nibarchive-1.1.0/nibarchive/model.py
+-rw-rw-rw-   0        0        0    10030 2023-07-11 14:16:00.000000 nibarchive-1.1.0/nibarchive/parse.py
+-rw-rw-rw-   0        0        0     4772 2023-07-11 06:17:47.000000 nibarchive-1.1.0/nibarchive/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:31:28.045715 nibarchive-1.1.0/nibarchive.egg-info/
+-rw-rw-rw-   0        0        0     4013 2023-07-11 14:31:27.000000 nibarchive-1.1.0/nibarchive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-11 14:31:27.000000 nibarchive-1.1.0/nibarchive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:31:27.000000 nibarchive-1.1.0/nibarchive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 14:31:27.000000 nibarchive-1.1.0/nibarchive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      850 2023-07-11 14:31:07.000000 nibarchive-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:31:28.068594 nibarchive-1.1.0/setup.cfg
```

### Comparing `nibarchive-1.0.0/LICENSE` & `nibarchive-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nibarchive-1.0.0/PKG-INFO` & `nibarchive-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibarchive
-Version: 1.0.0
+Version: 1.1.0
 Summary: Parser implementation of NeXTSTEP Interface Builder (NIB) files
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/nibarchive
 Project-URL: API-Docs, https://matrixeditor.github.io/nibarchive/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 License-File: LICENSE
 
 # NIBArchive-Parser
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.0&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.0&color=lightblue)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml)
 
 
 Parser implementation of NeXTSTEP Interface Builder (NIB) files in Python3.
 
 ## NIBArchive
 
@@ -61,15 +61,15 @@
 parser = NIBArchiveParser(verify=True)
 
 # Parse an input file from scratch
 with open("path/to/file.nib", "rb") as fp:
     archive: NIBArchive = parser.parse(fp)
 ```
 
-Or with `ByteIO`:
+Or with `BytesIO`:
 
 ```python
 from io import BytesIO
 
 # assue the file content is stored here
 buffer = bytes(...)
 parser = NIBArchiveParser()
```

### Comparing `nibarchive-1.0.0/README.md` & `nibarchive-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # NIBArchive-Parser
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.0&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.0&color=lightblue)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml)
 
 
 Parser implementation of NeXTSTEP Interface Builder (NIB) files in Python3.
 
 ## NIBArchive
 
@@ -45,15 +45,15 @@
 parser = NIBArchiveParser(verify=True)
 
 # Parse an input file from scratch
 with open("path/to/file.nib", "rb") as fp:
     archive: NIBArchive = parser.parse(fp)
 ```
 
-Or with `ByteIO`:
+Or with `BytesIO`:
 
 ```python
 from io import BytesIO
 
 # assue the file content is stored here
 buffer = bytes(...)
 parser = NIBArchiveParser()
```

### Comparing `nibarchive-1.0.0/nibarchive/model.py` & `nibarchive-1.1.0/nibarchive/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,261 +1,262 @@
-# Copyright (C) 2023 MatrixEditor
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from __future__ import annotations
-
-import enum
-
-from typing import Any
-from dataclasses import dataclass, field
-
-__all__ = [
-    "NIBArchiveHeader",
-    "ClassName",
-    "NIBKey",
-    "NIBValueType",
-    "NIBValue",
-    "NIBObject",
-    "NIBArchive",
-]
-
-
-@dataclass
-class NIBArchiveHeader:
-    """Represents the header of a NIB archive.
-
-    The header contains information about the archive, such as the number of objects,
-    keys, values, and class names present in the archive.
-
-    :param unknown_1: Unknown value 1.
-    :type unknown_1: int
-    :param unknown_2: Unknown value 2.
-    :type unknown_2: int
-    :param object_count: Number of objects in the archive.
-    :type object_count: int
-    :param offset_objects: Offset to the objects in the archive.
-    :type offset_objects: int
-    :param key_count: Number of keys in the archive.
-    :type key_count: int
-    :param offset_keys: Offset to the keys in the archive.
-    :type offset_keys: int
-    :param value_count: Number of values in the archive.
-    :type value_count: int
-    :param offset_values: Offset to the values in the archive.
-    :type offset_values: int
-    :param class_name_count: Number of class names in the archive.
-    :type class_name_count: int
-    :param offset_class_names: Offset to the class names in the archive.
-    :type offset_class_names: int
-    """
-    unknown_1: int
-    unknown_2: int
-    object_count: int
-    offset_objects: int
-    key_count: int
-    offset_keys: int
-    value_count: int
-    offset_values: int
-    class_name_count: int
-    offset_class_names: int
-
-
-@dataclass
-class ClassName:
-    """Represents a class name in a NIB archive.
-
-    Class names are used to identify the class type of objects in the archive.
-
-    :param length: Length of the class name (varint).
-    :type length: int
-    :param extras_count: Number of extra integers following the name (varint).
-    :type extras_count: int
-    :param name: Name of the class.
-    :type name: str
-    :param extras: Extra integers associated with the class (default: empty list).
-    :type extras: list[int]
-    """
-    length: int  # varint
-    extras_count: int  # varint
-    name: str  # name definition comes after extra integers
-    extras: list[int] = field(default_factory=list)
-
-
-@dataclass
-class NIBKey:
-    """Represents a key in a NIB archive.
-
-    Keys are used to identify the values associated with objects.
-
-    :param length: Length of the key (varint).
-    :type length: int
-    :param name: Name of the key.
-    :type name: str
-    """
-    length: int  # varint
-    name: str
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-class NIBValueType(enum.IntEnum):
-    """Enum representing the possible value types in a NIB archive.
-
-    The value types define the type of data stored in a :class:`NIBValue` object.
-
-    :param INT8: 8-bit integer.
-    :param INT16: 16-bit integer.
-    :param INT32: 32-bit integer.
-    :param INT64: 64-bit integer.
-    :param BOOL_TRUE: Boolean value true.
-    :param BOOL_FALSE: Boolean value false.
-    :param FLOAT: Single-precision floating-point number.
-    :param DOUBLE: Double-precision floating-point number.
-    :param DATA: Data object.
-    :param NIL: Nil value.
-    :param OBJECT_REF: Object reference.
-    """
-    INT8 = 0
-    INT16 = 1
-    INT32 = 2
-    INT64 = 3
-    BOOL_TRUE = 4
-    BOOL_FALSE = 5
-    FLOAT = 6
-    DOUBLE = 7
-    DATA = 8
-    NIL = 9
-    OBJECT_REF = 10
-
-    @staticmethod
-    def from_byte(value: int) -> "NIBValueType":
-        """
-        Get the NIBValueType enum value from a byte representation.
-
-        :param value: Byte value representing the NIBValueType.
-        :type value: int
-        :return: Corresponding NIBValueType enum value.
-        :rtype: NIBValueType
-        :raises ValueError: If the byte value does not match any NIBValueType.
-        """
-        for value_type in NIBValueType:
-            if value == value_type.value:
-                return value_type
-
-        raise ValueError(f"Unknown value type: {value:#x}")
-
-
-@dataclass
-class NIBValue:
-    """Represents a value in a NIB archive.
-
-    Values are associated with keys and hold data for objects.
-
-    :param key_index: Index of the associated :class:`NIBKey` (varint).
-    :type key_index: int
-    :param type: Type of the value.
-    :type type: :class`NIBValueType`
-    :param data: Data associated with the value (default: None).
-    :type data: Any
-    """
-    key_index: int  # varint
-    type: NIBValueType
-    data: Any = None
-
-
-@dataclass
-class NIBObject:
-    """Represents an object in a NIB archive.
-
-    Objects are instances of classes defined in the archive.
-
-    :param class_name_index: Index of the associated :class:`ClassName` (varint).
-    :type class_name_index: int
-    :param values_index: Index of the first associated :class:`NIBValue` (varint).
-    :type values_index: int
-    :param value_count: Number of associated values (varint).
-    :type value_count: int
-    """
-    class_name_index: int  # varint
-    values_index: int  # varint
-    value_count: int  # varint
-
-
-@dataclass
-class NIBArchive:
-    """A simple NIB archive dataclass.
-
-    :param header: Header of the NIB archive.
-    :type header: :class:`NIBArchiveHeader`
-    :param objects: List of NIBObject instances (default: empty list).
-    :type objects: list[:class:`NIBObject`]
-    :param keys: List of NIBKey instances (default: empty list).
-    :type keys: list[:class:`NIBKey`]
-    :param values: List of NIBValue instances (default: empty list).
-    :type values: list[:class:`NIBValue`]
-    :param class_names: List of ClassName instances (default: empty list).
-    :type class_names: list[:class:`ClassName`]
-    """
-    header: NIBArchiveHeader
-    objects: list[NIBObject] = field(default_factory=list)
-    keys: list[NIBKey] = field(default_factory=list)
-    values: list[NIBValue] = field(default_factory=list)
-    class_names: list[ClassName] = field(default_factory=list)
-
-    def get_object_values(self, obj: NIBObject) -> list[NIBValue]:
-        """
-        Get the list of NIBValues associated with a given NIBObject.
-
-        :param obj: The NIBObject.
-        :type obj: NIBObject
-        :return: The list of NIBValues associated with the object.
-        :rtype: List[NIBValue]
-        """
-        return self.values[obj.values_index:obj.values_index+obj.value_count]
-
-    def get_object_items(self, obj: NIBObject) -> dict[NIBKey, NIBValue]:
-        """
-        Get a dictionary of NIBKey-NIBValue pairs associated with a given NIBObject.
-
-        :param obj: The NIBObject.
-        :type obj: NIBObject
-        :return: The dictionary of NIBKey-NIBValue pairs associated with the object.
-        :rtype: Dict[NIBKey, NIBValue]
-        """
-        items = {}
-        for value in self.get_object_values(obj):
-            items[self.get_value_key(value)] = value
-        return items
-
-    def get_value_key(self, value: NIBValue) -> NIBKey:
-        """
-        Get the NIBKey associated with a given NIBValue.
-
-        :param value: The NIBValue.
-        :type value: NIBValue
-        :return: The associated NIBKey.
-        :rtype: NIBKey
-        """
-        return self.keys[value.key_index]
-
-    def get_class_name(self, obj: NIBObject) -> ClassName:
-        """
-        Get the ClassName associated with a given NIBObject.
-
-        :param obj: The NIBObject.
-        :type obj: NIBObject
-        :return: The associated ClassName.
-        :rtype: ClassName
-        """
-        return self.class_names[obj.class_name_index]
+# Copyright (C) 2023 MatrixEditor
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
+
+import enum
+
+from typing import Any
+from dataclasses import dataclass, field
+
+__all__ = [
+    "NIBArchiveHeader",
+    "ClassName",
+    "NIBKey",
+    "NIBValueType",
+    "NIBValue",
+    "NIBObject",
+    "NIBArchive",
+]
+
+
+@dataclass
+class NIBArchiveHeader:
+    """Represents the header of a NIB archive.
+
+    The header contains information about the archive, such as the number of objects,
+    keys, values, and class names present in the archive.
+
+    :param unknown_1: Unknown value 1.
+    :type unknown_1: int
+    :param unknown_2: Unknown value 2.
+    :type unknown_2: int
+    :param object_count: Number of objects in the archive.
+    :type object_count: int
+    :param offset_objects: Offset to the objects in the archive.
+    :type offset_objects: int
+    :param key_count: Number of keys in the archive.
+    :type key_count: int
+    :param offset_keys: Offset to the keys in the archive.
+    :type offset_keys: int
+    :param value_count: Number of values in the archive.
+    :type value_count: int
+    :param offset_values: Offset to the values in the archive.
+    :type offset_values: int
+    :param class_name_count: Number of class names in the archive.
+    :type class_name_count: int
+    :param offset_class_names: Offset to the class names in the archive.
+    :type offset_class_names: int
+    """
+    unknown_1: int
+    unknown_2: int
+    object_count: int
+    offset_objects: int
+    key_count: int
+    offset_keys: int
+    value_count: int
+    offset_values: int
+    class_name_count: int
+    offset_class_names: int
+
+
+@dataclass
+class ClassName:
+    """Represents a class name in a NIB archive.
+
+    Class names are used to identify the class type of objects in the archive.
+
+    :param length: Length of the class name (varint).
+    :type length: int
+    :param extras_count: Number of extra integers following the name (varint).
+    :type extras_count: int
+    :param name: Name of the class.
+    :type name: str
+    :param extras: Extra integers associated with the class (default: empty list).
+    :type extras: list[int]
+    """
+    length: int  # varint
+    extras_count: int  # varint
+    name: str  # name definition comes after extra integers
+    extras: list[int] = field(default_factory=list)
+
+
+@dataclass
+class NIBKey:
+    """Represents a key in a NIB archive.
+
+    Keys are used to identify the values associated with objects.
+
+    :param length: Length of the key (varint).
+    :type length: int
+    :param name: Name of the key.
+    :type name: str
+    """
+    length: int  # varint
+    name: str
+
+    def __hash__(self) -> int:
+        return hash(self.name)
+
+
+class NIBValueType(enum.IntEnum):
+    """Enum representing the possible value types in a NIB archive.
+
+    The value types define the type of data stored in a :class:`NIBValue` object.
+
+    :param INT8: 8-bit integer.
+    :param INT16: 16-bit integer.
+    :param INT32: 32-bit integer.
+    :param INT64: 64-bit integer.
+    :param BOOL_TRUE: Boolean value true.
+    :param BOOL_FALSE: Boolean value false.
+    :param FLOAT: Single-precision floating-point number.
+    :param DOUBLE: Double-precision floating-point number.
+    :param DATA: Data object.
+    :param NIL: Nil value.
+    :param OBJECT_REF: Object reference.
+    """
+    NIBARCHIVE = -1
+    INT8 = 0
+    INT16 = 1
+    INT32 = 2
+    INT64 = 3
+    BOOL_TRUE = 4
+    BOOL_FALSE = 5
+    FLOAT = 6
+    DOUBLE = 7
+    DATA = 8
+    NIL = 9
+    OBJECT_REF = 10
+
+    @staticmethod
+    def from_byte(value: int) -> "NIBValueType":
+        """
+        Get the NIBValueType enum value from a byte representation.
+
+        :param value: Byte value representing the NIBValueType.
+        :type value: int
+        :return: Corresponding NIBValueType enum value.
+        :rtype: NIBValueType
+        :raises ValueError: If the byte value does not match any NIBValueType.
+        """
+        for value_type in NIBValueType:
+            if value == value_type.value:
+                return value_type
+
+        raise ValueError(f"Unknown value type: {value:#x}")
+
+
+@dataclass
+class NIBValue:
+    """Represents a value in a NIB archive.
+
+    Values are associated with keys and hold data for objects.
+
+    :param key_index: Index of the associated :class:`NIBKey` (varint).
+    :type key_index: int
+    :param type: Type of the value.
+    :type type: :class`NIBValueType`
+    :param data: Data associated with the value (default: None).
+    :type data: Any
+    """
+    key_index: int  # varint
+    type: NIBValueType
+    data: Any = None
+
+
+@dataclass
+class NIBObject:
+    """Represents an object in a NIB archive.
+
+    Objects are instances of classes defined in the archive.
+
+    :param class_name_index: Index of the associated :class:`ClassName` (varint).
+    :type class_name_index: int
+    :param values_index: Index of the first associated :class:`NIBValue` (varint).
+    :type values_index: int
+    :param value_count: Number of associated values (varint).
+    :type value_count: int
+    """
+    class_name_index: int  # varint
+    values_index: int  # varint
+    value_count: int  # varint
+
+
+@dataclass
+class NIBArchive:
+    """A simple NIB archive dataclass.
+
+    :param header: Header of the NIB archive.
+    :type header: :class:`NIBArchiveHeader`
+    :param objects: List of NIBObject instances (default: empty list).
+    :type objects: list[:class:`NIBObject`]
+    :param keys: List of NIBKey instances (default: empty list).
+    :type keys: list[:class:`NIBKey`]
+    :param values: List of NIBValue instances (default: empty list).
+    :type values: list[:class:`NIBValue`]
+    :param class_names: List of ClassName instances (default: empty list).
+    :type class_names: list[:class:`ClassName`]
+    """
+    header: NIBArchiveHeader
+    objects: list[NIBObject] = field(default_factory=list)
+    keys: list[NIBKey] = field(default_factory=list)
+    values: list[NIBValue] = field(default_factory=list)
+    class_names: list[ClassName] = field(default_factory=list)
+
+    def get_object_values(self, obj: NIBObject) -> list[NIBValue]:
+        """
+        Get the list of NIBValues associated with a given NIBObject.
+
+        :param obj: The NIBObject.
+        :type obj: NIBObject
+        :return: The list of NIBValues associated with the object.
+        :rtype: List[NIBValue]
+        """
+        return self.values[obj.values_index:obj.values_index+obj.value_count]
+
+    def get_object_items(self, obj: NIBObject) -> dict[NIBKey, NIBValue]:
+        """
+        Get a dictionary of NIBKey-NIBValue pairs associated with a given NIBObject.
+
+        :param obj: The NIBObject.
+        :type obj: NIBObject
+        :return: The dictionary of NIBKey-NIBValue pairs associated with the object.
+        :rtype: Dict[NIBKey, NIBValue]
+        """
+        items = {}
+        for value in self.get_object_values(obj):
+            items[self.get_value_key(value)] = value
+        return items
+
+    def get_value_key(self, value: NIBValue) -> NIBKey:
+        """
+        Get the NIBKey associated with a given NIBValue.
+
+        :param value: The NIBValue.
+        :type value: NIBValue
+        :return: The associated NIBKey.
+        :rtype: NIBKey
+        """
+        return self.keys[value.key_index]
+
+    def get_class_name(self, obj: NIBObject) -> ClassName:
+        """
+        Get the ClassName associated with a given NIBObject.
+
+        :param obj: The NIBObject.
+        :type obj: NIBObject
+        :return: The associated ClassName.
+        :rtype: ClassName
+        """
+        return self.class_names[obj.class_name_index]
```

### Comparing `nibarchive-1.0.0/nibarchive/parse.py` & `nibarchive-1.1.0/nibarchive/parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,279 @@
-# Copyright (C) 2023 MatrixEditor
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# For more information about the file format, visit:
-# https://github.com/matsmattsson/nibsqueeze/blob/master/NibArchive.md
-from __future__ import annotations
-
-import struct
-import io
-
-from nibarchive import (
-    NIBArchive,
-    NIBArchiveHeader,
-    NIBObject,
-    NIBKey,
-    NIBValue,
-    NIBValueType,
-    ClassName
-)
-
-MAGIC_BYTES = b"NIBArchive"
-"""Magic bytes at the start of all NIB archives."""
-
-__all__ = [
-    "NIBFormatError",
-    "is_nib",
-    "varint",
-    "NIBArchiveParser",
-    "MAGIC_BYTES",
-]
-
-class NIBFormatError(Exception):
-    """Exception raised for errors related to NIB format.
-
-    This exception is raised when there is an error or inconsistency in the parsed NIB archive.
-    """
-
-
-def is_nib(fp) -> bool:
-    """
-    Check if the given file or byte array represents a NIB archive.
-
-    This function reads the first 10 bytes of the file or byte array and compares it
-    with the expected magic bytes to determine if it is a NIB archive.
-
-    :param fp: File or byte array to check.
-    :type fp: Union[io.IOBase, bytes, bytearray]
-    :return: True if the file or byte array is a NIB archive, False otherwise.
-    :rtype: bool
-    :raises TypeError: If the input is not a file object or byte array.
-    :raises ValueError: If the length of the input is not 10 bytes.
-    """
-    if isinstance(fp, io.IOBase):
-        fp.seek(0)
-        data = fp.read(10)  # magic has 10 bytes
-    elif isinstance(fp, (bytes, bytearray)):
-        data = fp
-    else:
-        raise TypeError(f"Invalid input type: (IOBase or bytes) - got {type(fp)}")
-
-    if len(data) != 10:
-        raise ValueError(f"Expected 10-byte array - got {len(data)} bytes")
-
-    return MAGIC_BYTES == data
-
-
-def varint(buf: bytes | io.IOBase, offset: int = 0) -> int:
-    """Decode a variable-length integer (varint) from a byte buffer.
-
-    This function decodes a varint from the given byte buffer and returns the decoded
-    integer value. A variable integer can consume up to two bytes and is compressed into
-    the first 7 bits only.
-
-    :param buf: Byte buffer containing the varint.
-    :type buf: bytes
-    :param offset: Offset in the byte buffer to start decoding (default: 0).
-    :type offset: int
-    :return: The decoded integer value.
-    :rtype: int
-    """
-    if isinstance(buf, io.IOBase):
-        current_byte, = buf.read(1)
-    else:
-        current_byte, = buf[offset:offset+1]
-
-    if current_byte & 128 == 0:
-        if isinstance(buf, io.IOBase):
-            next_byte, = buf.read(1)
-        else:
-            next_byte, = buf[offset+1:offset+2]
-        # little endian encoding
-        current_byte = (next_byte ^ 128) | current_byte << 8
-    else:
-        current_byte ^= 128
-
-    return current_byte
-
-
-
-class NIBArchiveParser:
-    """A simple parser for NIB archives.
-
-    :param verify: Flag indicating whether to perform verification checks during parsing (default: True).
-    :type verify: bool
-    """
-
-    def __init__(self, verify: bool = True) -> None:
-        """
-        Initialize the NIBArchiveParser.
-
-        :param verify: Flag indicating whether to perform verification checks during parsing.
-        :type verify: bool
-        """
-        self.archive: NIBArchive = None
-        self.verify = verify
-
-    def parse(self, fp: io.IOBase) -> NIBArchive:
-        """Parses the NIB archive.
-
-        This method reads the NIB archive from the given file object (fp) and
-        constructs a NIBArchive object representing the parsed contents.
-
-        :param fp: File object containing the NIB archive.
-        :type fp: io.IOBase
-        :return: The parsed NIBArchive object.
-        :rtype: NIBArchive
-        :raises TypeError: If the input is not a file object.
-        :raises NIBFormatError: If a verification check fails.
-        """
-        if not fp or not isinstance(fp, io.IOBase):
-            raise TypeError(f"Invalid input type: {type(fp)} is not an instance of IOBase")
-
-        offset = self.parse_header(fp)
-        header = self.archive.header
-        if offset != header.offset_objects and self.verify:
-            raise NIBFormatError(f"Expected object offset at {offset} - got {header.offset_objects}")
-
-        offset = self.parse_objects(fp, offset)
-        if offset != header.offset_keys and self.verify:
-            raise NIBFormatError(f"Expected keys offset at {offset} - got {header.offset_keys}")
-
-        offset = self.parse_keys(fp, offset)
-        if offset != header.offset_values and self.verify:
-            raise NIBFormatError(f"Expected values offset at {offset} - got {header.offset_values}")
-
-        offset = self.parse_values(fp, offset)
-        if offset != header.offset_class_names and self.verify:
-            raise NIBFormatError(f"Expected class names' offset at {offset} - got {header.offset_class_names}")
-
-        self.parse_class_names(fp, offset)
-        return self.archive
-
-
-    def parse_header(self, fp: io.IOBase) -> int:
-        if not is_nib(fp):
-            raise NIBFormatError("Expected b'NIBArchive' magic at byte 0")
-
-        header = NIBArchiveHeader(*struct.unpack("<iiiiiiiiii", fp.read(40)))
-        self.archive = NIBArchive(header)
-        return len(MAGIC_BYTES) + 40
-
-    def parse_objects(self, fp: io.IOBase, offset: int) -> int:
-        for _ in range(self.archive.header.object_count):
-            obj = NIBObject(varint(fp), varint(fp), varint(fp))
-            self.archive.objects.append(obj)
-            offset += (
-                self._get_varint_offset(obj.class_name_index)
-                + self._get_varint_offset(obj.value_count)
-                + self._get_varint_offset(obj.values_index)
-            )
-        return offset
-
-    def parse_keys(self, fp: io.IOBase, offset: int) -> int:
-        for _ in range(self.archive.header.key_count):
-            length = varint(fp)
-            key = NIBKey(length, fp.read(length).decode("utf-8"))
-            self.archive.keys.append(key)
-            offset += self._get_varint_offset(length) + length
-        return offset
-
-    def parse_class_names(self, fp: io.IOBase, offset: int) -> int:
-        for _ in range(self.archive.header.class_name_count):
-            length = varint(fp)
-            extras_count = varint(fp)
-            extras = struct.unpack(
-                "<%s" % "i"*extras_count, fp.read(4*extras_count))
-            # Name is \0 terminated, so we have to remove the trailing \0
-            name = fp.read(length)
-            class_name = ClassName(
-                length, extras_count, extras=list(extras), name=name[:-1].decode("utf-8")
-            )
-            self.archive.class_names.append(class_name)
-            offset += (self._get_varint_offset(length) +
-                       self._get_varint_offset(extras_count) + 4*extras_count + length)
-        return offset
-
-    def parse_values(self, fp: io.IOBase, offset: int) -> int:
-        for _ in range(self.archive.header.value_count):
-            key_index = varint(fp)
-            value_type = NIBValueType.from_byte(*fp.read(1))
-            offset += self._get_varint_offset(key_index) + 1
-
-            value = NIBValue(key_index, value_type)
-            attr_name = f"_parse_{value_type.name.lower()}"
-            if value_type != NIBValueType.NIL:
-                if hasattr(self, attr_name):
-                    offset = getattr(self, attr_name)(fp, value, offset)
-                else:
-                    raise ValueError(f"Unknown data type: {value_type}")
-            self.archive.values.append(value)
-        return offset
-
-    def _parse_int8(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = fp.read(1)
-        return offset + 1
-
-    def _parse_int16(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = struct.unpack("<h", fp.read(2))
-        return offset + 2
-
-    def _parse_int32(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = struct.unpack("<i", fp.read(4))
-        return offset + 4
-
-    def _parse_int64(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = struct.unpack("<q", fp.read(8))
-        return offset + 8
-
-    def _parse_bool_true(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data = True
-        return offset
-
-    def _parse_bool_false(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data = False
-        return offset
-
-    def _parse_float(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = struct.unpack("<f", fp.read(4))
-        return offset + 4
-
-    def _parse_double(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        value.data, = struct.unpack("<d", fp.read(8))
-        return offset + 8
-
-    def _parse_object_ref(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        return self._parse_int32(fp, value, offset)
-
-    def _parse_data(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
-        length = varint(fp)
-        value.data = fp.read(length)
-        return offset + self._get_varint_offset(length) + length
-
-    def _get_varint_offset(self, value: int) -> int:
-        return 2 if value > 127 else 1
+# Copyright (C) 2023 MatrixEditor
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# For more information about the file format, visit:
+# https://github.com/matsmattsson/nibsqueeze/blob/master/NibArchive.md
+from __future__ import annotations
+
+import struct
+import io
+
+from nibarchive import (
+    NIBArchive,
+    NIBArchiveHeader,
+    NIBObject,
+    NIBKey,
+    NIBValue,
+    NIBValueType,
+    ClassName
+)
+
+MAGIC_BYTES = b"NIBArchive"
+"""Magic bytes at the start of all NIB archives."""
+
+__all__ = [
+    "NIBFormatError",
+    "is_nib",
+    "varint",
+    "NIBArchiveParser",
+    "MAGIC_BYTES",
+]
+
+class NIBFormatError(Exception):
+    """Exception raised for errors related to NIB format.
+
+    This exception is raised when there is an error or inconsistency in the parsed NIB archive.
+    """
+
+
+def is_nib(fp) -> bool:
+    """
+    Check if the given file or byte array represents a NIB archive.
+
+    This function reads the first 10 bytes of the file or byte array and compares it
+    with the expected magic bytes to determine if it is a NIB archive.
+
+    :param fp: File or byte array to check.
+    :type fp: Union[io.IOBase, bytes, bytearray]
+    :return: True if the file or byte array is a NIB archive, False otherwise.
+    :rtype: bool
+    :raises TypeError: If the input is not a file object or byte array.
+    :raises ValueError: If the length of the input is not 10 bytes.
+    """
+    if isinstance(fp, io.IOBase):
+        fp.seek(0)
+        data = fp.read(10)  # magic has 10 bytes
+    elif isinstance(fp, (bytes, bytearray)):
+        data = fp
+    else:
+        raise TypeError(f"Invalid input type: (IOBase or bytes) - got {type(fp)}")
+
+    if len(data) != 10:
+        raise ValueError(f"Expected 10-byte array - got {len(data)} bytes")
+
+    return MAGIC_BYTES == data
+
+
+def varint(buf: bytes | io.IOBase, offset: int = 0) -> tuple[int, int]:
+    """Decode a variable-length integer (varint) from a byte buffer.
+
+    This function decodes a varint from the given byte buffer and returns the decoded
+    integer value. A variable integer can consume up to two bytes and is compressed into
+    the first 7 bits only.
+
+    :param buf: Byte buffer containing the varint.
+    :type buf: bytes
+    :param offset: Offset in the byte buffer to start decoding (default: 0).
+    :type offset: int
+    :return: The decoded integer value and its byte count
+    :rtype: int
+    """
+    result = 0
+    shift = 0
+    count = 0
+    while True:
+        count += 1
+        if isinstance(buf, io.IOBase):
+            current_byte, = buf.read(1)
+        else:
+            current_byte, = buf[offset:offset+1]
+
+        result |= (current_byte & 0x7F) << shift
+        shift += 7
+        if current_byte & 128:
+            break
+
+    return result, count
+
+
+
+class NIBArchiveParser:
+    """A simple parser for NIB archives.
+
+    :param verify: Flag indicating whether to perform verification checks during parsing (default: True).
+    :type verify: bool
+    """
+
+    def __init__(self, verify: bool = True) -> None:
+        """
+        Initialize the NIBArchiveParser.
+
+        :param verify: Flag indicating whether to perform verification checks during parsing.
+        :type verify: bool
+        """
+        self.archive: NIBArchive = None
+        self.verify = verify
+
+    def parse(self, fp: io.IOBase) -> NIBArchive:
+        """Parses the NIB archive.
+
+        This method reads the NIB archive from the given file object (fp) and
+        constructs a NIBArchive object representing the parsed contents.
+
+        :param fp: File object containing the NIB archive.
+        :type fp: io.IOBase
+        :return: The parsed NIBArchive object.
+        :rtype: NIBArchive
+        :raises TypeError: If the input is not a file object.
+        :raises NIBFormatError: If a verification check fails.
+        """
+        if not fp or not isinstance(fp, io.IOBase):
+            raise TypeError(f"Invalid input type: {type(fp)} is not an instance of IOBase")
+
+        offset = self.parse_header(fp)
+        header = self.archive.header
+        if offset != header.offset_objects and self.verify:
+            raise NIBFormatError(f"Expected object offset at {offset} - got {header.offset_objects}")
+
+        offset = self.parse_objects(fp, offset)
+        if offset != header.offset_keys and self.verify:
+            raise NIBFormatError(f"Expected keys offset at {offset} - got {header.offset_keys}")
+
+        offset = self.parse_keys(fp, offset)
+        if offset != header.offset_values and self.verify:
+            raise NIBFormatError(f"Expected values offset at {offset} - got {header.offset_values}")
+
+        offset = self.parse_values(fp, offset)
+        if offset != header.offset_class_names and self.verify:
+            raise NIBFormatError(f"Expected class names' offset at {offset} - got {header.offset_class_names}")
+
+        self.parse_class_names(fp, offset)
+        return self.archive
+
+
+    def parse_header(self, fp: io.IOBase) -> int:
+        if not is_nib(fp):
+            raise NIBFormatError("Expected b'NIBArchive' magic at byte 0")
+
+        header = NIBArchiveHeader(*struct.unpack("<iiiiiiiiii", fp.read(40)))
+        self.archive = NIBArchive(header)
+        return len(MAGIC_BYTES) + 40
+
+    def parse_objects(self, fp: io.IOBase, offset: int) -> int:
+        for _ in range(self.archive.header.object_count):
+            cni, byte_cnt = varint(fp)
+            offset += byte_cnt
+            vi, byte_cnt = varint(fp)
+            offset += byte_cnt
+            vc, byte_cnt = varint(fp)
+            offset += byte_cnt
+
+            obj = NIBObject(cni, vi, vc)
+            self.archive.objects.append(obj)
+        return offset
+
+    def parse_keys(self, fp: io.IOBase, offset: int) -> int:
+        for _ in range(self.archive.header.key_count):
+            length, cnt = varint(fp)
+            offset += cnt + length
+            key = NIBKey(length, fp.read(length).decode("utf-8"))
+            self.archive.keys.append(key)
+        return offset
+
+    def parse_class_names(self, fp: io.IOBase, offset: int) -> int:
+        for _ in range(self.archive.header.class_name_count):
+            length, count = varint(fp)
+            offset += length + count
+            extras_count, bytes_count = varint(fp)
+            offset += 4*extras_count + bytes_count
+
+            extras = struct.unpack(
+                "<%s" % "i"*extras_count, fp.read(4*extras_count))
+            # Name is \0 terminated, so we have to remove the trailing \0
+            name = fp.read(length)
+            class_name = ClassName(
+                length, extras_count, extras=list(extras), name=name[:-1].decode("utf-8")
+            )
+            self.archive.class_names.append(class_name)
+        return offset
+
+    def parse_values(self, fp: io.IOBase, offset: int) -> int:
+        for _ in range(self.archive.header.value_count):
+            key_index, bytes_count = varint(fp)
+            offset += bytes_count + 1
+            value_type = NIBValueType.from_byte(*fp.read(1))
+
+            value = NIBValue(key_index, value_type)
+            attr_name = f"_parse_{value_type.name.lower()}"
+            if value_type != NIBValueType.NIL:
+                if hasattr(self, attr_name):
+                    offset = getattr(self, attr_name)(fp, value, offset)
+                else:
+                    raise ValueError(f"Unknown data type: {value_type}")
+            self.archive.values.append(value)
+        return offset
+
+    def _parse_int8(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = fp.read(1)
+        return offset + 1
+
+    def _parse_int16(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = struct.unpack("<h", fp.read(2))
+        return offset + 2
+
+    def _parse_int32(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = struct.unpack("<i", fp.read(4))
+        return offset + 4
+
+    def _parse_int64(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = struct.unpack("<q", fp.read(8))
+        return offset + 8
+
+    def _parse_bool_true(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data = True
+        return offset
+
+    def _parse_bool_false(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data = False
+        return offset
+
+    def _parse_float(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = struct.unpack("<f", fp.read(4))
+        return offset + 4
+
+    def _parse_double(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        value.data, = struct.unpack("<d", fp.read(8))
+        return offset + 8
+
+    def _parse_object_ref(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        return self._parse_int32(fp, value, offset)
+
+    def _parse_data(self, fp: io.IOBase, value: NIBValue, offset: int) -> int:
+        length, bytes_count = varint(fp)
+        value.data = fp.read(length)
+
+        if length > 10 and is_nib(io.BytesIO(value.data)):
+            parser = NIBArchiveParser(verify=self.verify)
+            value.data = parser.parse(io.BytesIO(value.data))
+            value.type = NIBValueType.NIBARCHIVE
+
+        elif length and value.data[0] == 0x07:
+            if length == 17:
+                value.data = list(struct.unpack("<dd", value.data[1:]))
+            elif length == 33:
+                value.data = list(struct.unpack("<dddd", value.data[1:]))
+
+        return offset + bytes_count + length
+
```

### Comparing `nibarchive-1.0.0/nibarchive.egg-info/PKG-INFO` & `nibarchive-1.1.0/nibarchive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibarchive
-Version: 1.0.0
+Version: 1.1.0
 Summary: Parser implementation of NeXTSTEP Interface Builder (NIB) files
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/nibarchive
 Project-URL: API-Docs, https://matrixeditor.github.io/nibarchive/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 License-File: LICENSE
 
 # NIBArchive-Parser
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.0&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.0&color=lightblue)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/nibarchive/actions/workflows/sphinx.yml)
 
 
 Parser implementation of NeXTSTEP Interface Builder (NIB) files in Python3.
 
 ## NIBArchive
 
@@ -61,15 +61,15 @@
 parser = NIBArchiveParser(verify=True)
 
 # Parse an input file from scratch
 with open("path/to/file.nib", "rb") as fp:
     archive: NIBArchive = parser.parse(fp)
 ```
 
-Or with `ByteIO`:
+Or with `BytesIO`:
 
 ```python
 from io import BytesIO
 
 # assue the file content is stored here
 buffer = bytes(...)
 parser = NIBArchiveParser()
```

### Comparing `nibarchive-1.0.0/pyproject.toml` & `nibarchive-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nibarchive"
-version = "1.0.0"
+version = "1.1.0"
 description="Parser implementation of NeXTSTEP Interface Builder (NIB) files"
 authors = [
   { name="MatrixEditor", email="not@supported.com" },
 ]
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

