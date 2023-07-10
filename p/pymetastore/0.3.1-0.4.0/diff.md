# Comparing `tmp/pymetastore-0.3.1.tar.gz` & `tmp/pymetastore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetastore-0.3.1.tar", last modified: Wed Jul  5 21:40:10 2023, max compression
+gzip compressed data, was "pymetastore-0.4.0.tar", last modified: Mon Jul 10 21:56:27 2023, max compression
```

## Comparing `pymetastore-0.3.1.tar` & `pymetastore-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.3.1/LICENSE
--rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.3.1/pymetastore/__init__.py
--rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.3.1/pymetastore/hive_metastore/ThriftHiveMetastore-remote
--rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.3.1/pymetastore/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.3.1/pymetastore/hive_metastore/__init__.py
--rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.3.1/pymetastore/hive_metastore/constants.py
--rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.3.1/pymetastore/hive_metastore/ttypes.py
--rw-r--r--   0        0        0    19260 2023-06-29 00:42:02.585443 pymetastore-0.3.1/pymetastore/htypes.py
--rw-r--r--   0        0        0    26171 2023-07-05 21:36:14.864892 pymetastore-0.3.1/pymetastore/metastore.py
--rw-r--r--   0        0        0     3266 2023-06-30 15:36:42.940073 pymetastore-0.3.1/pymetastore/stats.py
--rw-r--r--   0        0        0     1393 2023-07-05 21:40:10.990019 pymetastore-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    22253 2023-06-30 15:55:18.493675 pymetastore-0.3.1/tests/integration/test_metastore.py
--rw-r--r--   0        0        0    19596 2023-06-29 00:42:02.587038 pymetastore-0.3.1/tests/unit/test_htypes.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 pymetastore-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.4.0/pymetastore/__init__.py
+-rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote
+-rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.4.0/pymetastore/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.4.0/pymetastore/hive_metastore/constants.py
+-rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.4.0/pymetastore/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0    21240 2023-07-10 21:52:23.632268 pymetastore-0.4.0/pymetastore/htypes.py
+-rw-r--r--   0        0        0    26176 2023-07-10 21:52:23.632813 pymetastore-0.4.0/pymetastore/metastore.py
+-rw-r--r--   0        0        0     3381 2023-07-10 21:52:23.633402 pymetastore-0.4.0/pymetastore/stats.py
+-rw-r--r--   0        0        0     1393 2023-07-10 21:56:27.253183 pymetastore-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    26646 2023-07-10 21:52:23.633742 pymetastore-0.4.0/tests/integration/test_metastore.py
+-rw-r--r--   0        0        0    19596 2023-06-29 00:42:02.587038 pymetastore-0.4.0/tests/unit/test_htypes.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 pymetastore-0.4.0/PKG-INFO
```

### Comparing `pymetastore-0.3.1/LICENSE` & `pymetastore-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/README.md` & `pymetastore-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/pymetastore/hive_metastore/ThriftHiveMetastore-remote` & `pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/pymetastore/hive_metastore/ThriftHiveMetastore.py` & `pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/pymetastore/hive_metastore/constants.py` & `pymetastore-0.4.0/pymetastore/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/pymetastore/hive_metastore/ttypes.py` & `pymetastore-0.4.0/pymetastore/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/pymetastore/htypes.py` & `pymetastore-0.4.0/pymetastore/htypes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+"""
+htypes module contains the Hive metastore types, including primitive and complex types.
+User defined types are defined by the user, using a combination of complex 
+and primitive types and thus are not included in this module.
+there are also some helper functions to convert between Hive metastore types and HType objects.
+"""
 from collections import namedtuple
 from enum import Enum
 from typing import Any, List, Optional
 
 
 class PrimitiveCategory(Enum):
+    """An Enumeration holding all the primitive types supported by Hive."""
+
     VOID = "VOID"
     BOOLEAN = "BOOLEAN"
     BYTE = "BYTE"
     SHORT = "SHORT"
     INT = "INT"
     LONG = "LONG"
     FLOAT = "FLOAT"
@@ -22,52 +30,71 @@
     CHAR = "CHAR"
     INTERVAL_YEAR_MONTH = "INTERVAL_YEAR_MONTH"
     INTERVAL_DAY_TIME = "INTERVAL_DAY_TIME"
     UNKNOWN = "UNKNOWN"
 
 
 class HTypeCategory(Enum):
+    """
+    An Enumeration holding all the complex types supported by Hive plus
+    the primitive types.
+    """
+
     PRIMITIVE = PrimitiveCategory
     STRUCT = "STRUCT"
     MAP = "MAP"
     LIST = "LIST"
     UNION = "UNION"
 
 
 class HType:
+    """
+    The base class for all Hive metastore types.
+    It contains the name of the type and the category of the type.
+    """
+
     def __init__(self, name: str, category: HTypeCategory):
         self.name = name
         self.category = category
 
     def __str__(self):
         return f"{self.__class__.__name__}(name={self.name}, category={self.category})"
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.name}', {self.category})"
 
     def __eq__(self, other):
         if isinstance(other, HType):
             return (self.name == other.name) and (self.category == other.category)
-        else:
-            return False
+        return False
 
 
 class HPrimitiveType(HType):
+    """
+    A class representing a primitive type in Hive metastore.
+    It is initialized by passing a PrimitiveCategory enum value.
+    """
+
     def __init__(self, primitive_type: PrimitiveCategory):
         super().__init__(primitive_type.value, HTypeCategory.PRIMITIVE)
         self.primitive_type = primitive_type
 
     def __str__(self):
         return f"{self.__class__.__name__}(name={self.name}, category={self.category})"
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.primitive_type})"
 
 
 class HMapType(HType):
+    """
+    A class representing a map type in Hive metastore.
+    It is initialized by passing two lists. A list of field names and a list of field types.
+    """
+
     def __init__(self, key_type: HType, value_type: HType):
         super().__init__("MAP", HTypeCategory.MAP)
         self.key_type = key_type
         self.value_type = value_type
 
     def __str__(self):
         return f"{super().__str__()}, key_type={str(self.key_type)}, value_type={str(self.value_type)})"
@@ -78,55 +105,68 @@
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return (
                 super().__eq__(other)
                 and (self.key_type == other.key_type)
                 and (self.value_type == other.value_type)
             )
-        else:
-            return False
+        return False
 
 
 class HListType(HType):
+    """
+    A class representing a List or array type in Hive metastore.
+    It is initialized by passing the element type of the list.
+    """
+
     def __init__(self, element_type: HType):
         super().__init__("LIST", HTypeCategory.LIST)
         self.element_type = element_type
 
     def __str__(self):
         return f"{super().__str__()}, element_type={str(self.element_type)})"
 
     def __repr__(self):
         return f"HListType({repr(self.element_type)})"
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return super().__eq__(other) and (self.element_type == other.element_type)
-        else:
-            return False
+        return False
 
 
 class HUnionType(HType):
+    """
+    A class representing a Union type in Hive metastore.
+    It is initialized by passing a list of types.
+    """
+
     def __init__(self, types: List[HType]):
         super().__init__("UNION", HTypeCategory.UNION)
         self.types = types
 
     def __str__(self):
         return f"{super().__str__()}, types={str(self.types)})"
 
     def __repr__(self):
         return f"HUnionType({repr(self.types)})"
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return super().__eq__(other) and (self.types == other.types)
-        else:
-            return False
+        return False
 
 
 class HVarcharType(HType):
+    """
+    A class representing a Varchar type in Hive metastore.
+    Varchar is primitive but parameterized by length.
+    Varchar by definition has a maximum length of 65535.
+    """
+
     def __init__(self, length: int):
         MAX_VARCHAR_LENGTH = 65535
         if length > MAX_VARCHAR_LENGTH:
             raise ValueError("Varchar length cannot exceed 65535")
         super().__init__("VARCHAR", HTypeCategory.PRIMITIVE)
         self.length = length
 
@@ -135,19 +175,24 @@
 
     def __repr__(self):
         return f"HVarcharType({self.length})"
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return super().__eq__(other) and (self.length == other.length)
-        else:
-            return False
+        return False
 
 
 class HCharType(HType):
+    """
+    A class representing a Char type in Hive metastore.
+    Char is primitive but parameterized by length.
+    Char by definition has a maximum length of 255.
+    """
+
     def __init__(self, length: int):
         MAX_CHAR_LENGTH = 255
         if length > MAX_CHAR_LENGTH:
             raise ValueError("Char length cannot exceed 255")
         super().__init__("CHAR", HTypeCategory.PRIMITIVE)
         self.length = length
 
@@ -156,19 +201,24 @@
 
     def __repr__(self):
         return f"HCharType({self.length})"
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return super().__eq__(other) and (self.length == other.length)
-        else:
-            return False
+        return False
 
 
 class HDecimalType(HType):
+    """
+    A class representing a Decimal type in Hive metastore.
+    Decimal is primitive but parameterized by precision and scale.
+    Decimal by definition has a maximum precision and scale of 38.
+    """
+
     def __init__(self, precision: int, scale: int):
         MAX_PRECISION = 38
         MAX_SCALE = 38
         if precision > MAX_PRECISION:
             raise ValueError("Decimal precision cannot exceed 38")
         if scale > MAX_SCALE:
             raise ValueError("Decimal scale cannot exceed 38")
@@ -185,19 +235,23 @@
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return (
                 super().__eq__(other)
                 and (self.precision == other.precision)
                 and (self.scale == other.scale)
             )
-        else:
-            return False
+        return False
 
 
 class HStructType(HType):
+    """
+    A class representing a Struct type in Hive metastore.
+    Struct is parameterized by a list of names and types.
+    """
+
     def __init__(self, names: List[str], types: List[HType]):
         if len(names) != len(types):
             raise ValueError("mismatched size of names and types.")
         if None in names:
             raise ValueError("names cannot contain None")
         if None in types:
             raise ValueError("types cannot contain None")
@@ -215,21 +269,25 @@
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return (
                 super().__eq__(other)
                 and (self.names == other.names)
                 and (self.types == other.types)
             )
-        else:
-            return False
+        return False
 
 
 # We need to maintain a list of the expected serialized type names.
 # Thrift will return the type in string format and we will have to parse it to get the type.
 class SerdeTypeNameConstants(Enum):
+    """
+    Serde TypeNameConstants is an enum class that contains the list of expected type names
+    as they are used by Thrift.
+    """
+
     # Primitive types
     VOID = "void"
     BOOLEAN = "boolean"
     TINYINT = "tinyint"
     SMALLINT = "smallint"
     INT = "int"
     BIGINT = "bigint"
@@ -273,38 +331,48 @@
     PrimitiveCategory.VARCHAR: SerdeTypeNameConstants.VARCHAR,
     PrimitiveCategory.CHAR: SerdeTypeNameConstants.CHAR,
     PrimitiveCategory.INTERVAL_YEAR_MONTH: SerdeTypeNameConstants.INTERVAL_YEAR_MONTH,
     PrimitiveCategory.INTERVAL_DAY_TIME: SerdeTypeNameConstants.INTERVAL_DAY_TIME,
     PrimitiveCategory.UNKNOWN: SerdeTypeNameConstants.UNKNOWN,
 }
 
-# We also need the inverse though.
+""" We also need the inverse though.
+"""
 serde_to_primitive_mapping = {v.name: k for k, v in primitive_to_serde_mapping.items()}
 
+""" This function gets us the serde type name from the primitive one."""
+
 
-# This function gets us the serde type name from the primitive one.
 def primitive_to_serde(primitive_category: PrimitiveCategory) -> SerdeTypeNameConstants:
     return primitive_to_serde_mapping[primitive_category]
 
 
-# This function gets us the primitive type name from the serde one.
+""" This function gets us the primitive type name from the serde one."""
+
+
 def serde_to_primitive(serde_type_name: str) -> Optional[PrimitiveCategory]:
     return serde_to_primitive_mapping.get(serde_type_name)
 
 
-# We also need a way to get the serde enum key from the string we get from Thrift.
+"""This function returns the serde enum key from the string we get from Thrift"""
+
+
 def get_serde_type_by_value(value):
     for member in SerdeTypeNameConstants:
         if member.value == value:
             return member.name
     return None
 
 
-# To be used for tokening the Thrift type string. We need to tokenize the
-# string to get the type name and the type parameters.
+"""
+To be used for tokening the Thrift type string. We need to tokenize the
+string to get the type name and the type parameters.
+"""
+
+
 class Token(namedtuple("Token", ["position", "text", "type"])):
     def __new__(cls, position: int, text: str, type_: bool) -> Any:
         if text is None:
             raise ValueError("text is null")
         return super().__new__(cls, position, text, type_)
 
     def __str__(self):
@@ -319,17 +387,20 @@
             raise ValueError("type_params is null")
         return super().__new__(cls, type_name, type_params)
 
     def __str__(self):
         return f"{self.type_name}:{self.type_params}"
 
 
-# Util functions to parse the Thrift column types (as strings) and return the
-# expected hive type
 class TypeParser:
+    """
+    Util functions to parse the Thrift column types (as strings) and return the
+    expected hive type
+    """
+
     def __init__(self, type_info_string: str):
         self.type_string = type_info_string
         self.type_tokens = self.tokenize(type_info_string)
         self.index = 0
 
     # we want the base name of the type, in general the format of a
     # parameterized type is <base_name>(<type1>, <type2>, ...), so the base
```

### Comparing `pymetastore-0.3.1/pymetastore/metastore.py` & `pymetastore-0.4.0/pymetastore/metastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,22 +629,22 @@
             table.writeId,
             table.owner,
         )
 
     def get_table_stats(
         self,
         table: HTable,
-        columns: List[HColumn],
+        columns: List[HColumn] | None = None,
     ) -> List[ColumnStats]:
-        assert isinstance(table, HTable)
-        assert isinstance(columns, list)
+        columns = columns or []
 
         if len(columns) > 0:
             assert all(isinstance(column, HColumn) for column in columns)
 
+        assert isinstance(table, HTable)
         assert table.name is not None
         assert table.database_name is not None
         assert table.columns is not None
         assert len(table.columns) > 0
 
         if len(columns) == 0:
             columns = table.columns
```

### Comparing `pymetastore-0.3.1/pymetastore/stats.py` & `pymetastore-0.4.0/pymetastore/stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
+from pymetastore.hive_metastore import ttypes
+
 
 @dataclass
 class TypeStats:
     numNulls: int
     typeName: str
 
 
@@ -82,42 +84,42 @@
         self.maxColLen = maxColLen
         self.avgColLen = avgColLen
 
 
 @dataclass
 class DecimalTypeStats(TypeStats):
     cardinality: int
-    lowValue: Optional[float]
-    highValue: Optional[float]
+    lowValue: Optional[ttypes.Decimal]
+    highValue: Optional[ttypes.Decimal]
 
     def __init__(
         self,
         cardinality: int,
         numNulls: int,
-        lowValue: Optional[float] = None,
-        highValue: Optional[float] = None,
+        lowValue: Optional[ttypes.Decimal] = None,
+        highValue: Optional[ttypes.Decimal] = None,
     ):
         super().__init__(typeName="decimal", numNulls=numNulls)
         self.cardinality = cardinality
         self.lowValue = lowValue
         self.highValue = highValue
 
 
 @dataclass
 class DateTypeStats(TypeStats):
     cardinality: int
-    lowValue: Optional[int]
-    highValue: Optional[int]
+    lowValue: Optional[ttypes.Date]
+    highValue: Optional[ttypes.Date]
 
     def __init__(
         self,
         cardinality: int,
         numNulls: int,
-        lowValue: Optional[int] = None,
-        highValue: Optional[int] = None,
+        lowValue: Optional[ttypes.Date] = None,
+        highValue: Optional[ttypes.Date] = None,
     ):
         super().__init__(typeName="date", numNulls=numNulls)
         self.cardinality = cardinality
         self.lowValue = lowValue
         self.highValue = highValue
```

### Comparing `pymetastore-0.3.1/pyproject.toml` & `pymetastore-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymetastore"
-version = "0.3.1"
+version = "0.4.0"
 description = "A Python client for the Thrift interface to Hive Metastore"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
     { name = "Kostas Pardalis" },
 ]
 dependencies = [
     "thrift>=0.16.0",
```

### Comparing `pymetastore-0.3.1/tests/integration/test_metastore.py` & `pymetastore-0.4.0/tests/integration/test_metastore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Integration tests for the metastore module.
+"""
 import os
 
 import pytest
 from thrift.protocol import TBinaryProtocol
 from thrift.transport import TSocket, TTransport
 
 from pymetastore.hive_metastore import ttypes
@@ -13,27 +16,28 @@
     HMapType,
     HPrimitiveType,
     HStructType,
     HType,
     HTypeCategory,
     HUnionType,
     HVarcharType,
+    PrimitiveCategory,
 )
 from pymetastore.metastore import (
     HMS,
     BucketingVersion,
     HColumn,
     HDatabase,
     HPartition,
     HStorage,
     HTable,
     HiveBucketProperty,
     StorageFormat,
 )
-from pymetastore.stats import BooleanTypeStats
+from pymetastore.stats import *
 
 
 @pytest.fixture(scope="module")
 def hive_client():
     host = os.environ.get("HMS_HOST", "localhost")
     port = int(os.environ.get("HMS_PORT", 9083))
     transport = TSocket.TSocket(host, port)
@@ -62,23 +66,23 @@
     hive_client.create_database(db)
 
     cols = [
         ttypes.FieldSchema(name="col1", type="int", comment="c1"),
         ttypes.FieldSchema(name="col2", type="string", comment="c2"),
     ]
 
-    partitionKeys = [ttypes.FieldSchema(name="partition", type="string", comment="")]
+    partition_keys = [ttypes.FieldSchema(name="partition", type="string", comment="")]
 
     serde_info = ttypes.SerDeInfo(
         name="test_serde",
         serializationLib="org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe",
         parameters={"field.delim": ","},
     )
 
-    storageDesc = ttypes.StorageDescriptor(
+    storage_desc = ttypes.StorageDescriptor(
         location="/tmp/test_db/test_table",
         cols=cols,
         inputFormat="org.apache.hadoop.mapred.TextInputFormat",
         outputFormat="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
         compressed=False,
         numBuckets=-1,
         serdeInfo=serde_info,
@@ -88,30 +92,30 @@
     table = ttypes.Table(
         tableName="test_table",
         dbName="test_db",
         owner="owner",
         createTime=0,
         lastAccessTime=0,
         retention=0,
-        sd=storageDesc,
-        partitionKeys=partitionKeys,
+        sd=storage_desc,
+        partitionKeys=partition_keys,
         parameters={},
         tableType="EXTERNAL_TABLE",
     )
 
     if "test_table" in hive_client.get_all_tables("test_db"):
         hive_client.drop_table("test_db", "test_table", True)
     hive_client.create_table(table)
 
     for i in range(1, 6):
         partition = ttypes.Partition(
             dbName="test_db",
             tableName="test_table",
             values=[str(i)],
-            sd=storageDesc,
+            sd=storage_desc,
             parameters={},
         )
         hive_client.add_partition(partition)
 
     # testing primitive Types
     cols2 = [
         ttypes.FieldSchema(name="col3", type="void", comment="c3"),
@@ -127,15 +131,15 @@
             name="col12", type="timestamp with local time zone", comment="c12"
         ),
         ttypes.FieldSchema(name="col13", type="interval_year_month", comment="c13"),
         ttypes.FieldSchema(name="col14", type="interval_day_time", comment="c14"),
         ttypes.FieldSchema(name="col15", type="binary", comment="c15"),
     ]
 
-    storageDesc = ttypes.StorageDescriptor(
+    storage_desc = ttypes.StorageDescriptor(
         location="/tmp/test_db/test_table2",
         cols=cols2,
         inputFormat="org.apache.hadoop.mapred.TextInputFormat",
         outputFormat="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
         compressed=False,
         numBuckets=-1,
         serdeInfo=serde_info,
@@ -145,16 +149,16 @@
     table = ttypes.Table(
         tableName="test_table2",
         dbName="test_db",
         owner="owner",
         createTime=0,
         lastAccessTime=0,
         retention=0,
-        sd=storageDesc,
-        partitionKeys=partitionKeys,
+        sd=storage_desc,
+        partitionKeys=partition_keys,
         parameters={},
         tableType="EXTERNAL_TABLE",
     )
 
     if "test_table2" in hive_client.get_all_tables("test_db"):
         hive_client.drop_table("test_db", "test_table2", True)
     hive_client.create_table(table)
@@ -166,15 +170,15 @@
         ttypes.FieldSchema(name="col18", type="char(10)", comment="c18"),
         ttypes.FieldSchema(name="col19", type="array<int>", comment="c19"),
         ttypes.FieldSchema(name="col20", type="map<int,string>", comment="c20"),
         ttypes.FieldSchema(name="col21", type="struct<a:int,b:string>", comment="c21"),
         ttypes.FieldSchema(name="col22", type="uniontype<int,string>", comment="c22"),
     ]
 
-    storageDesc = ttypes.StorageDescriptor(
+    storage_desc = ttypes.StorageDescriptor(
         location="/tmp/test_db/test_table3",
         cols=cols3,
         inputFormat="org.apache.hadoop.mapred.TextInputFormat",
         outputFormat="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
         compressed=False,
         numBuckets=-1,
         serdeInfo=serde_info,
@@ -184,27 +188,35 @@
     table = ttypes.Table(
         tableName="test_table3",
         dbName="test_db",
         owner="owner",
         createTime=0,
         lastAccessTime=0,
         retention=0,
-        sd=storageDesc,
-        partitionKeys=partitionKeys,
+        sd=storage_desc,
+        partitionKeys=partition_keys,
         parameters={},
         tableType="EXTERNAL_TABLE",
     )
 
     if "test_table3" in hive_client.get_all_tables("test_db"):
         hive_client.drop_table("test_db", "test_table3", True)
     hive_client.create_table(table)
 
-    cols4 = [ttypes.FieldSchema(name="col4", type="boolean", comment="c4")]
+    cols4 = [
+        ttypes.FieldSchema(name="col4", type="boolean", comment="c4"),
+        ttypes.FieldSchema(name="col5", type="double", comment="c5"),
+        ttypes.FieldSchema(name="col6", type="bigint", comment="c6"),
+        ttypes.FieldSchema(name="col7", type="string", comment="c7"),
+        ttypes.FieldSchema(name="col8", type="binary", comment="c8"),
+        ttypes.FieldSchema(name="col9", type="decimal(10,2)", comment="c9"),
+        ttypes.FieldSchema(name="col10", type="date", comment="c10"),
+    ]
 
-    storageDesc = ttypes.StorageDescriptor(
+    storage_desc = ttypes.StorageDescriptor(
         location="/tmp/test_db/test_table4",
         cols=cols4,
         inputFormat="org.apache.hadoop.mapred.TextInputFormat",
         outputFormat="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
         compressed=False,
         numBuckets=-1,
         serdeInfo=serde_info,
@@ -214,32 +226,80 @@
     table = ttypes.Table(
         tableName="test_table4",
         dbName="test_db",
         owner="owner",
         createTime=0,
         lastAccessTime=0,
         retention=0,
-        sd=storageDesc,
-        partitionKeys=partitionKeys,
+        sd=storage_desc,
+        partitionKeys=partition_keys,
         parameters={},
         tableType="EXTERNAL_TABLE",
     )
 
     if "test_table4" in hive_client.get_all_tables("test_db"):
         hive_client.drop_table("test_db", "test_table4", True)
     hive_client.create_table(table)
 
-    stats_desc = ttypes.ColumnStatisticsDesc(True, "test_db", "test_table4", "col4")
+    stats_desc = ttypes.ColumnStatisticsDesc(True, "test_db", "test_table4")
 
-    stats = ttypes.BooleanColumnStatsData(10, 10, 0)
-    stats_obj = ttypes.ColumnStatisticsObj(
-        "col4", "boolean", ttypes.ColumnStatisticsData(stats)
+    stats_bool = ttypes.BooleanColumnStatsData(numTrues=10, numFalses=10, numNulls=0)
+    stats_obj_bool = ttypes.ColumnStatisticsObj(
+        "col4", "boolean", ttypes.ColumnStatisticsData(booleanStats=stats_bool)
     )
-    col_stats = ttypes.ColumnStatistics(stats_desc, [stats_obj])
 
+    stats_double = ttypes.DoubleColumnStatsData(
+        lowValue=0, highValue=1, numNulls=0, numDVs=100
+    )
+    stats_obj_double = ttypes.ColumnStatisticsObj(
+        "col5", "double", ttypes.ColumnStatisticsData(doubleStats=stats_double)
+    )
+    stats_long = ttypes.LongColumnStatsData(
+        lowValue=0, highValue=100, numNulls=0, numDVs=100
+    )
+    stats_obj_long = ttypes.ColumnStatisticsObj(
+        "col6", "bigint", ttypes.ColumnStatisticsData(longStats=stats_long)
+    )
+    stats_string = ttypes.StringColumnStatsData(
+        avgColLen=10, maxColLen=10, numNulls=5, numDVs=10
+    )
+    stats_obj_string = ttypes.ColumnStatisticsObj(
+        "col7", "string", ttypes.ColumnStatisticsData(stringStats=stats_string)
+    )
+    stats_binary = ttypes.BinaryColumnStatsData(avgColLen=10, maxColLen=10, numNulls=5)
+    stats_obj_binary = ttypes.ColumnStatisticsObj(
+        "col8", "binary", ttypes.ColumnStatisticsData(binaryStats=stats_binary)
+    )
+    stats_decimal = ttypes.DecimalColumnStatsData(
+        lowValue=ttypes.Decimal(1, b"123445.3"),
+        highValue=ttypes.Decimal(1, b"1232324124"),
+        numNulls=0,
+        numDVs=100,
+    )
+    stats_obj_decimal = ttypes.ColumnStatisticsObj(
+        "col9", "decimal(10,2)", ttypes.ColumnStatisticsData(decimalStats=stats_decimal)
+    )
+    stats_date = ttypes.DateColumnStatsData(
+        lowValue=ttypes.Date(0), highValue=ttypes.Date(1), numNulls=0, numDVs=100
+    )
+    stats_obj_date = ttypes.ColumnStatisticsObj(
+        "col10", "date", ttypes.ColumnStatisticsData(dateStats=stats_date)
+    )
+    col_stats = ttypes.ColumnStatistics(
+        stats_desc,
+        [
+            stats_obj_bool,
+            stats_obj_double,
+            stats_obj_long,
+            stats_obj_string,
+            stats_obj_binary,
+            stats_obj_decimal,
+            stats_obj_date,
+        ],
+    )
     hive_client.update_table_column_statistics(col_stats)
 
 
 def test_list_databases(hive_client):
     assert "test_db" in HMS(hive_client).list_databases()
 
 
@@ -271,17 +331,16 @@
     assert len(table.columns) == 2
     assert isinstance(table.columns[0], HColumn)
     assert isinstance(table.columns[1], HColumn)
     assert len(table.partition_columns) == 1
     assert isinstance(table.partition_columns[0], HColumn)
     assert isinstance(table.parameters, dict)
     assert len(table.parameters) == 1
-    assert (
-        table.parameters.get("transient_lastDdlTime") is not None
-    )  # this is not a parameter of the table we created, but the metastore adds it
+    # this is not a parameter of the table we created, but the metastore adds it
+    assert table.parameters.get("transient_lastDdlTime") is not None
     # This assertion fails, I leave it here on purpose. My current assumption is that
     # the metastore overrides some of the passed options with defaults. "MANAGEd_TABLE"
     # is the default value for tableType. See here for the defaults:
     # https://github.com/apache/hive/blob/14a1f70607db5ae6cf71b6d4343f308a5167581c/standalone-metastore/metastore-server/src/main/java/org/apache/hadoop/hive/metastore/client/builder/TableBuilder.java#L69C43-L69C43
     # Something similar happens also when you choose a "VIRTUAL_VIEW" table type, where
     # the metastore overrides the storage descriptor removing in the location the file::
     # prefix.
@@ -595,17 +654,64 @@
     assert columns[6].type.types[1].name == "STRING"
 
 
 def test_table_stats(hive_client):
     hms = HMS(hive_client)
     table = hms.get_table("test_db", "test_table4")
 
-    statistics = hms.get_table_stats(table, [])
+    statistics = hms.get_table_stats(
+        table,
+        [
+            HColumn("col4", HPrimitiveType(PrimitiveCategory.BOOLEAN)),
+            HColumn("col5", HPrimitiveType(PrimitiveCategory.DOUBLE)),
+            HColumn("col7", HPrimitiveType(PrimitiveCategory.STRING)),
+            HColumn("col8", HPrimitiveType(PrimitiveCategory.BINARY)),
+            HColumn("col9", HDecimalType(1, 1)),
+            HColumn("col10", HPrimitiveType(PrimitiveCategory.DATE)),
+            HColumn("col6", HPrimitiveType(PrimitiveCategory.LONG)),
+        ],
+    )
 
-    assert len(statistics) == 1
+    assert len(statistics) == 7
     assert statistics[0].tableName == "test_table4"
     assert statistics[0].dbName == "test_db"
     assert statistics[0].stats is not None
+
     assert isinstance(statistics[0].stats, BooleanTypeStats)
     assert statistics[0].stats.numTrues == 10
     assert statistics[0].stats.numFalses == 10
     assert statistics[0].stats.numNulls == 0
+
+    assert isinstance(statistics[1].stats, DoubleTypeStats)
+    assert statistics[1].stats.lowValue == 0
+    assert statistics[1].stats.highValue == 1
+    assert statistics[1].stats.numNulls == 0
+    assert statistics[1].stats.cardinality == 100
+
+    assert isinstance(statistics[2].stats, StringTypeStats)
+    assert statistics[2].stats.avgColLen == 10
+    assert statistics[2].stats.maxColLen == 10
+    assert statistics[2].stats.numNulls == 5
+    assert statistics[2].stats.cardinality == 10
+
+    assert isinstance(statistics[3].stats, BinaryTypeStats)
+    assert statistics[3].stats.avgColLen == 10
+    assert statistics[3].stats.maxColLen == 10
+    assert statistics[3].stats.numNulls == 5
+
+    assert isinstance(statistics[4].stats, DecimalTypeStats)
+    assert statistics[4].stats.lowValue == ttypes.Decimal(scale=1, unscaled=b"123445.3")
+    assert statistics[4].stats.highValue == ttypes.Decimal(1, b"1232324124")
+    assert statistics[4].stats.numNulls == 0
+    assert statistics[4].stats.cardinality == 100
+
+    assert isinstance(statistics[5].stats, DateTypeStats)
+    assert statistics[5].stats.lowValue == ttypes.Date(0)
+    assert statistics[5].stats.highValue == ttypes.Date(1)
+    assert statistics[5].stats.numNulls == 0
+    assert statistics[5].stats.cardinality == 100
+
+    assert isinstance(statistics[6].stats, LongTypeStats)
+    assert statistics[6].stats.lowValue == 0
+    assert statistics[6].stats.highValue == 100
+    assert statistics[6].stats.numNulls == 0
+    assert statistics[6].stats.cardinality == 100
```

### Comparing `pymetastore-0.3.1/tests/unit/test_htypes.py` & `pymetastore-0.4.0/tests/unit/test_htypes.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.3.1/PKG-INFO` & `pymetastore-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetastore
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python client for the Thrift interface to Hive Metastore
 Author: Kostas Pardalis
 Author-Email: Chris Riccomini <criccomini@apache.org>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: thrift>=0.16.0
 Description-Content-Type: text/markdown
```

