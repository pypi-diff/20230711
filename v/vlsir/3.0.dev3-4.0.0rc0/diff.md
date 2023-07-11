# Comparing `tmp/vlsir-3.0.dev3.tar.gz` & `tmp/vlsir-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsir-3.0.dev3.tar", last modified: Tue Jan 17 23:17:06 2023, max compression
+gzip compressed data, was "vlsir-4.0.0rc0.tar", last modified: Tue Jul 11 16:48:05 2023, max compression
```

## Comparing `vlsir-3.0.dev3.tar` & `vlsir-4.0.0rc0.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:06.554854 vlsir-3.0.dev3/
--rw-r--r--   0 dan        (501) staff       (20)     2762 2022-06-13 20:36:42.000000 vlsir-3.0.dev3/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     1521 2022-06-15 18:46:18.000000 vlsir-3.0.dev3/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)      390 2023-01-17 23:17:06.554670 vlsir-3.0.dev3/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)       98 2022-06-15 18:46:18.000000 vlsir-3.0.dev3/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:17:06.554904 vlsir-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1077 2023-01-17 23:14:16.000000 vlsir-3.0.dev3/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:06.550096 vlsir-3.0.dev3/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsir-3.0.dev3/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     2903 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/tests/test_vlsir.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:06.553180 vlsir-3.0.dev3/vlsir/
--rw-r--r--   0 dan        (501) staff       (20)      545 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     7686 2022-12-05 04:35:07.000000 vlsir-3.0.dev3/vlsir/circuit_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     5885 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/geometry_pb2.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:06.554365 vlsir-3.0.dev3/vlsir/layout/
--rw-r--r--   0 dan        (501) staff       (20)     9022 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/layout/raw_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    17716 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/layout/tetris_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     1038 2022-06-13 20:36:42.000000 vlsir-3.0.dev3/vlsir/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     8929 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/raw_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    27500 2022-12-05 04:35:07.000000 vlsir-3.0.dev3/vlsir/spice_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     3536 2022-12-05 04:35:07.000000 vlsir-3.0.dev3/vlsir/tech_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    17523 2022-07-19 02:39:52.000000 vlsir-3.0.dev3/vlsir/tetris_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     6038 2022-12-05 04:35:07.000000 vlsir-3.0.dev3/vlsir/utils_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    14067 2022-12-06 02:10:08.000000 vlsir-3.0.dev3/vlsir/vlsir.primitives.pb.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:06.554036 vlsir-3.0.dev3/vlsir.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      390 2023-01-17 23:17:06.000000 vlsir-3.0.dev3/vlsir.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      474 2023-01-17 23:17:06.000000 vlsir-3.0.dev3/vlsir.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:17:06.000000 vlsir-3.0.dev3/vlsir.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       74 2023-01-17 23:17:06.000000 vlsir-3.0.dev3/vlsir.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       12 2023-01-17 23:17:06.000000 vlsir-3.0.dev3/vlsir.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:05.533943 vlsir-4.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2762 2023-04-26 23:15:43.000000 vlsir-4.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-04-26 23:15:43.000000 vlsir-4.0.0rc0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)      415 2023-07-11 16:48:05.533744 vlsir-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)       98 2023-06-26 21:21:08.000000 vlsir-4.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:48:05.533986 vlsir-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1631 2023-07-11 16:44:54.000000 vlsir-4.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:05.531206 vlsir-4.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2023-04-26 23:15:43.000000 vlsir-4.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1186 2023-06-28 18:09:23.000000 vlsir-4.0.0rc0/tests/test_vlsir.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:05.532799 vlsir-4.0.0rc0/vlsir/
+-rw-r--r--   0 dan        (501) staff       (20)      506 2023-06-26 23:54:24.000000 vlsir-4.0.0rc0/vlsir/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4553 2023-06-28 18:09:27.000000 vlsir-4.0.0rc0/vlsir/circuit_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     5885 2023-06-27 00:04:47.000000 vlsir-4.0.0rc0/vlsir/geometry_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     8929 2023-06-27 00:06:34.000000 vlsir-4.0.0rc0/vlsir/raw_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)    13234 2023-06-28 18:09:23.000000 vlsir-4.0.0rc0/vlsir/spice_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     1978 2023-06-27 00:37:13.000000 vlsir-4.0.0rc0/vlsir/tech_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)    17523 2023-06-27 00:06:34.000000 vlsir-4.0.0rc0/vlsir/tetris_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     3319 2023-06-28 18:09:23.000000 vlsir-4.0.0rc0/vlsir/utils_pb2.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:05.533505 vlsir-4.0.0rc0/vlsir.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      415 2023-07-11 16:48:05.000000 vlsir-4.0.0rc0/vlsir.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      373 2023-07-11 16:48:05.000000 vlsir-4.0.0rc0/vlsir.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:48:05.000000 vlsir-4.0.0rc0/vlsir.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       72 2023-07-11 16:48:05.000000 vlsir-4.0.0rc0/vlsir.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       12 2023-07-11 16:48:05.000000 vlsir-4.0.0rc0/vlsir.egg-info/top_level.txt
```

### Comparing `vlsir-3.0.dev3/.gitignore` & `vlsir-4.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `vlsir-3.0.dev3/LICENSE` & `vlsir-4.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlsir-3.0.dev3/vlsir/circuit_pb2.py` & `vlsir-4.0.0rc0/vlsir/raw_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,219 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: circuit.proto
+# source: raw.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import utils_pb2 as utils__pb2
+from . import circuit_pb2 as circuit__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\rcircuit.proto\x12\rvlsir.circuit\x1a\x0butils.proto"\x83\x01\n\x07Package\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12&\n\x07modules\x18\x02 \x03(\x0b\x32\x15.vlsir.circuit.Module\x12\x32\n\x0b\x65xt_modules\x18\x03 \x03(\x0b\x32\x1d.vlsir.circuit.ExternalModule\x12\x0c\n\x04\x64\x65sc\x18\n \x01(\t"\x81\x01\n\x04Port\x12\x0e\n\x06signal\x18\x01 \x01(\t\x12\x30\n\tdirection\x18\x02 \x01(\x0e\x32\x1d.vlsir.circuit.Port.Direction"7\n\tDirection\x12\t\n\x05INPUT\x10\x00\x12\n\n\x06OUTPUT\x10\x01\x12\t\n\x05INOUT\x10\x02\x12\x08\n\x04NONE\x10\x03"%\n\x06Signal\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05width\x18\x02 \x01(\x03"1\n\x05Slice\x12\x0e\n\x06signal\x18\x01 \x01(\t\x12\x0b\n\x03top\x18\x02 \x01(\x03\x12\x0b\n\x03\x62ot\x18\x03 \x01(\x03"8\n\x06\x43oncat\x12.\n\x05parts\x18\x01 \x03(\x0b\x32\x1f.vlsir.circuit.ConnectionTarget"z\n\x10\x43onnectionTarget\x12\r\n\x03sig\x18\x01 \x01(\tH\x00\x12%\n\x05slice\x18\x02 \x01(\x0b\x32\x14.vlsir.circuit.SliceH\x00\x12\'\n\x06\x63oncat\x18\x03 \x01(\x0b\x32\x15.vlsir.circuit.ConcatH\x00\x42\x07\n\x05stype"O\n\nConnection\x12\x10\n\x08portname\x18\x01 \x01(\t\x12/\n\x06target\x18\x02 \x01(\x0b\x32\x1f.vlsir.circuit.ConnectionTarget"\x98\x01\n\x08Instance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x06module\x18\x02 \x01(\x0b\x32\x16.vlsir.utils.Reference\x12&\n\nparameters\x18\x03 \x03(\x0b\x32\x12.vlsir.utils.Param\x12.\n\x0b\x63onnections\x18\x04 \x03(\x0b\x32\x19.vlsir.circuit.Connection"\xb6\x01\n\x06Module\x12\x0c\n\x04name\x18\x01 \x01(\t\x12"\n\x05ports\x18\x02 \x03(\x0b\x32\x13.vlsir.circuit.Port\x12&\n\x07signals\x18\x03 \x03(\x0b\x32\x15.vlsir.circuit.Signal\x12*\n\tinstances\x18\x04 \x03(\x0b\x32\x17.vlsir.circuit.Instance\x12&\n\nparameters\x18\x05 \x03(\x0b\x32\x12.vlsir.utils.Param"\xbc\x01\n\x0e\x45xternalModule\x12(\n\x04name\x18\x01 \x01(\x0b\x32\x1a.vlsir.utils.QualifiedName\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12"\n\x05ports\x18\x03 \x03(\x0b\x32\x13.vlsir.circuit.Port\x12&\n\x07signals\x18\x04 \x03(\x0b\x32\x15.vlsir.circuit.Signal\x12&\n\nparameters\x18\x05 \x03(\x0b\x32\x12.vlsir.utils.Param"=\n\tInterface\x12\x0c\n\x04name\x18\x01 \x01(\t\x12"\n\x05ports\x18\n \x03(\x0b\x32\x13.vlsir.circuit.Portb\x06proto3'
+    b'\n\traw.proto\x12\tvlsir.raw\x1a\x0butils.proto\x1a\rcircuit.proto"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x03\x12\t\n\x01y\x18\x02 \x01(\x03"(\n\x05Layer\x12\x0e\n\x06number\x18\x01 \x01(\x03\x12\x0f\n\x07purpose\x18\x02 \x01(\x03"]\n\tRectangle\x12\x0b\n\x03net\x18\x01 \x01(\t\x12$\n\nlower_left\x18\x02 \x01(\x0b\x32\x10.vlsir.raw.Point\x12\r\n\x05width\x18\x03 \x01(\x03\x12\x0e\n\x06height\x18\x04 \x01(\x03":\n\x07Polygon\x12\x0b\n\x03net\x18\x01 \x01(\t\x12"\n\x08vertices\x18\x02 \x03(\x0b\x32\x10.vlsir.raw.Point"D\n\x04Path\x12\x0b\n\x03net\x18\x01 \x01(\t\x12 \n\x06points\x18\x02 \x03(\x0b\x32\x10.vlsir.raw.Point\x12\r\n\x05width\x18\x03 \x01(\x03"\x9e\x01\n\x0bLayerShapes\x12\x1f\n\x05layer\x18\x01 \x01(\x0b\x32\x10.vlsir.raw.Layer\x12(\n\nrectangles\x18\x02 \x03(\x0b\x32\x14.vlsir.raw.Rectangle\x12$\n\x08polygons\x18\x03 \x03(\x0b\x32\x12.vlsir.raw.Polygon\x12\x1e\n\x05paths\x18\x04 \x03(\x0b\x32\x0f.vlsir.raw.Path"<\n\x0bTextElement\x12\x0e\n\x06string\x18\x01 \x01(\t\x12\x1d\n\x03loc\x18\x02 \x01(\x0b\x32\x10.vlsir.raw.Point"\xa3\x01\n\x08Instance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x04\x63\x65ll\x18\x03 \x01(\x0b\x32\x16.vlsir.utils.Reference\x12)\n\x0forigin_location\x18\x04 \x01(\x0b\x32\x10.vlsir.raw.Point\x12\x14\n\x0creflect_vert\x18\x06 \x01(\x08\x12"\n\x1arotation_clockwise_degrees\x18\x07 \x01(\x05"\x93\x01\n\x06Layout\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x06shapes\x18\x02 \x03(\x0b\x32\x16.vlsir.raw.LayerShapes\x12&\n\tinstances\x18\x03 \x03(\x0b\x32\x13.vlsir.raw.Instance\x12+\n\x0b\x61nnotations\x18\x04 \x03(\x0b\x32\x16.vlsir.raw.TextElement"\x90\x01\n\x08\x41\x62stract\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x07outline\x18\x02 \x01(\x0b\x32\x12.vlsir.raw.Polygon\x12&\n\x05ports\x18\x04 \x03(\x0b\x32\x17.vlsir.raw.AbstractPort\x12)\n\tblockages\x18\x05 \x03(\x0b\x32\x16.vlsir.raw.LayerShapes"C\n\x0c\x41\x62stractPort\x12\x0b\n\x03net\x18\x01 \x01(\t\x12&\n\x06shapes\x18\x02 \x03(\x0b\x32\x16.vlsir.raw.LayerShapes"\xb2\x01\n\x04\x43\x65ll\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\tinterface\x18\n \x01(\x0b\x32\x18.vlsir.circuit.Interface\x12%\n\x06module\x18\x0b \x01(\x0b\x32\x15.vlsir.circuit.Module\x12%\n\x08\x61\x62stract\x18\x0c \x01(\x0b\x32\x13.vlsir.raw.Abstract\x12!\n\x06layout\x18\r \x01(\x0b\x32\x11.vlsir.raw.Layout"\x87\x01\n\x07Library\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x1f\n\x05units\x18\x02 \x01(\x0e\x32\x10.vlsir.raw.Units\x12\x1e\n\x05\x63\x65lls\x18\n \x03(\x0b\x32\x0f.vlsir.raw.Cell\x12+\n\x06\x61uthor\x18\x14 \x01(\x0b\x32\x1b.vlsir.utils.AuthorMetadata**\n\x05Units\x12\t\n\x05MICRO\x10\x00\x12\x08\n\x04NANO\x10\x01\x12\x0c\n\x08\x41NGSTROM\x10\x02\x62\x06proto3'
 )
 
-
-_PACKAGE = DESCRIPTOR.message_types_by_name["Package"]
-_PORT = DESCRIPTOR.message_types_by_name["Port"]
-_SIGNAL = DESCRIPTOR.message_types_by_name["Signal"]
-_SLICE = DESCRIPTOR.message_types_by_name["Slice"]
-_CONCAT = DESCRIPTOR.message_types_by_name["Concat"]
-_CONNECTIONTARGET = DESCRIPTOR.message_types_by_name["ConnectionTarget"]
-_CONNECTION = DESCRIPTOR.message_types_by_name["Connection"]
+_UNITS = DESCRIPTOR.enum_types_by_name["Units"]
+Units = enum_type_wrapper.EnumTypeWrapper(_UNITS)
+MICRO = 0
+NANO = 1
+ANGSTROM = 2
+
+
+_POINT = DESCRIPTOR.message_types_by_name["Point"]
+_LAYER = DESCRIPTOR.message_types_by_name["Layer"]
+_RECTANGLE = DESCRIPTOR.message_types_by_name["Rectangle"]
+_POLYGON = DESCRIPTOR.message_types_by_name["Polygon"]
+_PATH = DESCRIPTOR.message_types_by_name["Path"]
+_LAYERSHAPES = DESCRIPTOR.message_types_by_name["LayerShapes"]
+_TEXTELEMENT = DESCRIPTOR.message_types_by_name["TextElement"]
 _INSTANCE = DESCRIPTOR.message_types_by_name["Instance"]
-_MODULE = DESCRIPTOR.message_types_by_name["Module"]
-_EXTERNALMODULE = DESCRIPTOR.message_types_by_name["ExternalModule"]
-_INTERFACE = DESCRIPTOR.message_types_by_name["Interface"]
-_PORT_DIRECTION = _PORT.enum_types_by_name["Direction"]
-Package = _reflection.GeneratedProtocolMessageType(
-    "Package",
+_LAYOUT = DESCRIPTOR.message_types_by_name["Layout"]
+_ABSTRACT = DESCRIPTOR.message_types_by_name["Abstract"]
+_ABSTRACTPORT = DESCRIPTOR.message_types_by_name["AbstractPort"]
+_CELL = DESCRIPTOR.message_types_by_name["Cell"]
+_LIBRARY = DESCRIPTOR.message_types_by_name["Library"]
+Point = _reflection.GeneratedProtocolMessageType(
+    "Point",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PACKAGE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Package)
+        "DESCRIPTOR": _POINT,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Point)
     },
 )
-_sym_db.RegisterMessage(Package)
+_sym_db.RegisterMessage(Point)
 
-Port = _reflection.GeneratedProtocolMessageType(
-    "Port",
+Layer = _reflection.GeneratedProtocolMessageType(
+    "Layer",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PORT,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Port)
+        "DESCRIPTOR": _LAYER,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Layer)
     },
 )
-_sym_db.RegisterMessage(Port)
+_sym_db.RegisterMessage(Layer)
 
-Signal = _reflection.GeneratedProtocolMessageType(
-    "Signal",
+Rectangle = _reflection.GeneratedProtocolMessageType(
+    "Rectangle",
     (_message.Message,),
     {
-        "DESCRIPTOR": _SIGNAL,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Signal)
+        "DESCRIPTOR": _RECTANGLE,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Rectangle)
     },
 )
-_sym_db.RegisterMessage(Signal)
+_sym_db.RegisterMessage(Rectangle)
 
-Slice = _reflection.GeneratedProtocolMessageType(
-    "Slice",
+Polygon = _reflection.GeneratedProtocolMessageType(
+    "Polygon",
     (_message.Message,),
     {
-        "DESCRIPTOR": _SLICE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Slice)
+        "DESCRIPTOR": _POLYGON,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Polygon)
     },
 )
-_sym_db.RegisterMessage(Slice)
+_sym_db.RegisterMessage(Polygon)
 
-Concat = _reflection.GeneratedProtocolMessageType(
-    "Concat",
+Path = _reflection.GeneratedProtocolMessageType(
+    "Path",
     (_message.Message,),
     {
-        "DESCRIPTOR": _CONCAT,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Concat)
+        "DESCRIPTOR": _PATH,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Path)
     },
 )
-_sym_db.RegisterMessage(Concat)
+_sym_db.RegisterMessage(Path)
 
-ConnectionTarget = _reflection.GeneratedProtocolMessageType(
-    "ConnectionTarget",
+LayerShapes = _reflection.GeneratedProtocolMessageType(
+    "LayerShapes",
     (_message.Message,),
     {
-        "DESCRIPTOR": _CONNECTIONTARGET,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.ConnectionTarget)
+        "DESCRIPTOR": _LAYERSHAPES,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.LayerShapes)
     },
 )
-_sym_db.RegisterMessage(ConnectionTarget)
+_sym_db.RegisterMessage(LayerShapes)
 
-Connection = _reflection.GeneratedProtocolMessageType(
-    "Connection",
+TextElement = _reflection.GeneratedProtocolMessageType(
+    "TextElement",
     (_message.Message,),
     {
-        "DESCRIPTOR": _CONNECTION,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Connection)
+        "DESCRIPTOR": _TEXTELEMENT,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.TextElement)
     },
 )
-_sym_db.RegisterMessage(Connection)
+_sym_db.RegisterMessage(TextElement)
 
 Instance = _reflection.GeneratedProtocolMessageType(
     "Instance",
     (_message.Message,),
     {
         "DESCRIPTOR": _INSTANCE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Instance)
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Instance)
     },
 )
 _sym_db.RegisterMessage(Instance)
 
-Module = _reflection.GeneratedProtocolMessageType(
-    "Module",
+Layout = _reflection.GeneratedProtocolMessageType(
+    "Layout",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _LAYOUT,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Layout)
+    },
+)
+_sym_db.RegisterMessage(Layout)
+
+Abstract = _reflection.GeneratedProtocolMessageType(
+    "Abstract",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _ABSTRACT,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Abstract)
+    },
+)
+_sym_db.RegisterMessage(Abstract)
+
+AbstractPort = _reflection.GeneratedProtocolMessageType(
+    "AbstractPort",
     (_message.Message,),
     {
-        "DESCRIPTOR": _MODULE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Module)
+        "DESCRIPTOR": _ABSTRACTPORT,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.AbstractPort)
     },
 )
-_sym_db.RegisterMessage(Module)
+_sym_db.RegisterMessage(AbstractPort)
 
-ExternalModule = _reflection.GeneratedProtocolMessageType(
-    "ExternalModule",
+Cell = _reflection.GeneratedProtocolMessageType(
+    "Cell",
     (_message.Message,),
     {
-        "DESCRIPTOR": _EXTERNALMODULE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.ExternalModule)
+        "DESCRIPTOR": _CELL,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Cell)
     },
 )
-_sym_db.RegisterMessage(ExternalModule)
+_sym_db.RegisterMessage(Cell)
 
-Interface = _reflection.GeneratedProtocolMessageType(
-    "Interface",
+Library = _reflection.GeneratedProtocolMessageType(
+    "Library",
     (_message.Message,),
     {
-        "DESCRIPTOR": _INTERFACE,
-        "__module__": "circuit_pb2"
-        # @@protoc_insertion_point(class_scope:vlsir.circuit.Interface)
+        "DESCRIPTOR": _LIBRARY,
+        "__module__": "raw_pb2"
+        # @@protoc_insertion_point(class_scope:vlsir.raw.Library)
     },
 )
-_sym_db.RegisterMessage(Interface)
+_sym_db.RegisterMessage(Library)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _PACKAGE._serialized_start = 46
-    _PACKAGE._serialized_end = 177
-    _PORT._serialized_start = 180
-    _PORT._serialized_end = 309
-    _PORT_DIRECTION._serialized_start = 254
-    _PORT_DIRECTION._serialized_end = 309
-    _SIGNAL._serialized_start = 311
-    _SIGNAL._serialized_end = 348
-    _SLICE._serialized_start = 350
-    _SLICE._serialized_end = 399
-    _CONCAT._serialized_start = 401
-    _CONCAT._serialized_end = 457
-    _CONNECTIONTARGET._serialized_start = 459
-    _CONNECTIONTARGET._serialized_end = 581
-    _CONNECTION._serialized_start = 583
-    _CONNECTION._serialized_end = 662
-    _INSTANCE._serialized_start = 665
-    _INSTANCE._serialized_end = 817
-    _MODULE._serialized_start = 820
-    _MODULE._serialized_end = 1002
-    _EXTERNALMODULE._serialized_start = 1005
-    _EXTERNALMODULE._serialized_end = 1193
-    _INTERFACE._serialized_start = 1195
-    _INTERFACE._serialized_end = 1256
+    _UNITS._serialized_start = 1424
+    _UNITS._serialized_end = 1466
+    _POINT._serialized_start = 52
+    _POINT._serialized_end = 81
+    _LAYER._serialized_start = 83
+    _LAYER._serialized_end = 123
+    _RECTANGLE._serialized_start = 125
+    _RECTANGLE._serialized_end = 218
+    _POLYGON._serialized_start = 220
+    _POLYGON._serialized_end = 278
+    _PATH._serialized_start = 280
+    _PATH._serialized_end = 348
+    _LAYERSHAPES._serialized_start = 351
+    _LAYERSHAPES._serialized_end = 509
+    _TEXTELEMENT._serialized_start = 511
+    _TEXTELEMENT._serialized_end = 571
+    _INSTANCE._serialized_start = 574
+    _INSTANCE._serialized_end = 737
+    _LAYOUT._serialized_start = 740
+    _LAYOUT._serialized_end = 887
+    _ABSTRACT._serialized_start = 890
+    _ABSTRACT._serialized_end = 1034
+    _ABSTRACTPORT._serialized_start = 1036
+    _ABSTRACTPORT._serialized_end = 1103
+    _CELL._serialized_start = 1106
+    _CELL._serialized_end = 1284
+    _LIBRARY._serialized_start = 1287
+    _LIBRARY._serialized_end = 1422
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vlsir-3.0.dev3/vlsir/geometry_pb2.py` & `vlsir-4.0.0rc0/vlsir/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-3.0.dev3/vlsir/layout/tetris_pb2.py` & `vlsir-4.0.0rc0/vlsir/tetris_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: layout/tetris.proto
+# source: tetris.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import utils_pb2 as utils__pb2
-from layout import raw_pb2 as layout_dot_raw__pb2
-import circuit_pb2 as circuit__pb2
+from . import utils_pb2 as utils__pb2
+from . import raw_pb2 as raw__pb2
+from . import circuit_pb2 as circuit__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x13layout/tetris.proto\x12\x0cvlsir.tetris\x1a\x0butils.proto\x1a\x10layout/raw.proto\x1a\rcircuit.proto"i\n\x07Library\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12!\n\x05\x63\x65lls\x18\n \x03(\x0b\x32\x12.vlsir.tetris.Cell\x12+\n\x06\x61uthor\x18\x14 \x01(\x0b\x32\x1b.vlsir.utils.AuthorMetadata"\xb8\x01\n\x04\x43\x65ll\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\tinterface\x18\n \x01(\x0b\x32\x18.vlsir.circuit.Interface\x12%\n\x06module\x18\x0b \x01(\x0b\x32\x15.vlsir.circuit.Module\x12(\n\x08\x61\x62stract\x18\x0c \x01(\x0b\x32\x16.vlsir.tetris.Abstract\x12$\n\x06layout\x18\r \x01(\x0b\x32\x14.vlsir.tetris.Layout"\xbc\x01\n\x06Layout\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x07outline\x18\n \x01(\x0b\x32\x15.vlsir.tetris.Outline\x12)\n\tinstances\x18\x14 \x03(\x0b\x32\x16.vlsir.tetris.Instance\x12)\n\x0b\x61ssignments\x18\x15 \x03(\x0b\x32\x14.vlsir.tetris.Assign\x12&\n\x04\x63uts\x18\x16 \x03(\x0b\x32\x18.vlsir.tetris.TrackCross";\n\x06\x41ssign\x12\x0b\n\x03net\x18\x01 \x01(\t\x12$\n\x02\x61t\x18\x02 \x01(\x0b\x32\x18.vlsir.tetris.TrackCross"Z\n\nTrackCross\x12%\n\x05track\x18\x01 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x12%\n\x05\x63ross\x18\x02 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef"(\n\x08TrackRef\x12\r\n\x05layer\x18\x01 \x01(\x03\x12\r\n\x05track\x18\x02 \x01(\x03"/\n\x07Outline\x12\t\n\x01x\x18\x01 \x03(\x03\x12\t\n\x01y\x18\x02 \x03(\x03\x12\x0e\n\x06metals\x18\x03 \x01(\x03"k\n\x08\x41\x62stract\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x07outline\x18\n \x01(\x0b\x32\x15.vlsir.tetris.Outline\x12)\n\x05ports\x18\x14 \x03(\x0b\x32\x1a.vlsir.tetris.AbstractPort"\x97\x04\n\x0c\x41\x62stractPort\x12\x0b\n\x03net\x18\x01 \x01(\t\x12\x33\n\x04\x65\x64ge\x18\n \x01(\x0b\x32#.vlsir.tetris.AbstractPort.EdgePortH\x00\x12<\n\tztop_edge\x18\x0b \x01(\x0b\x32\'.vlsir.tetris.AbstractPort.ZTopEdgePortH\x00\x12:\n\nztop_inner\x18\x0c \x01(\x0b\x32$.vlsir.tetris.AbstractPort.ZTopInnerH\x00\x1a\x64\n\x08\x45\x64gePort\x12%\n\x05track\x18\x01 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x12\x31\n\x04side\x18\x02 \x01(\x0e\x32#.vlsir.tetris.AbstractPort.PortSide\x1av\n\x0cZTopEdgePort\x12\r\n\x05track\x18\x01 \x01(\x03\x12\x31\n\x04side\x18\x02 \x01(\x0e\x32#.vlsir.tetris.AbstractPort.PortSide\x12$\n\x04into\x18\x03 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x1a\x33\n\tZTopInner\x12&\n\x04locs\x18\x01 \x03(\x0b\x32\x18.vlsir.tetris.TrackCross"0\n\x08PortSide\x12\x12\n\x0e\x42OTTOM_OR_LEFT\x10\x00\x12\x10\n\x0cTOP_OR_RIGHT\x10\x01\x42\x06\n\x04kind"\x8d\x01\n\x08Instance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x04\x63\x65ll\x18\x03 \x01(\x0b\x32\x16.vlsir.utils.Reference\x12 \n\x03loc\x18\x04 \x01(\x0b\x32\x13.vlsir.tetris.Place\x12\x15\n\rreflect_horiz\x18\x06 \x01(\x08\x12\x14\n\x0creflect_vert\x18\x07 \x01(\x08"X\n\x05Place\x12\x1f\n\x03\x61\x62s\x18\x01 \x01(\x0b\x32\x10.vlsir.raw.PointH\x00\x12%\n\x03rel\x18\x02 \x01(\x0b\x32\x16.vlsir.tetris.RelPlaceH\x00\x42\x07\n\x05place"\n\n\x08RelPlace"\xce\x01\n\x05Stack\x12\x1f\n\x05units\x18\x01 \x01(\x0e\x32\x10.vlsir.raw.Units\x12*\n\x04prim\x18\x02 \x01(\x0b\x32\x1c.vlsir.tetris.PrimitiveLayer\x12(\n\x06metals\x18\x03 \x03(\x0b\x32\x18.vlsir.tetris.MetalLayer\x12$\n\x04vias\x18\x04 \x03(\x0b\x32\x16.vlsir.tetris.ViaLayer\x12(\n\x0e\x62oundary_layer\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"{\n\tLayerEnum\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.vlsir.tetris.LayerEnum.LayerType\x12\r\n\x05index\x18\x02 \x01(\x03".\n\tLayerType\x12\r\n\tPRIMITIVE\x10\x00\x12\t\n\x05METAL\x10\x01\x12\x07\n\x03VIA\x10\x02"\xd1\x02\n\nMetalLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x03\x64ir\x18\x02 \x01(\x0e\x32\x1c.vlsir.tetris.MetalLayer.Dir\x12\x0f\n\x07\x63utsize\x18\x03 \x01(\x03\x12(\n\x07\x65ntries\x18\x04 \x03(\x0b\x32\x17.vlsir.tetris.TrackSpec\x12\x0e\n\x06offset\x18\x05 \x01(\x03\x12\x0f\n\x07overlap\x18\x06 \x01(\x03\x12\x0c\n\x04\x66lip\x18\x07 \x01(\x08\x12\x34\n\x04prim\x18\x08 \x01(\x0e\x32&.vlsir.tetris.MetalLayer.PrimitiveMode\x12\x1d\n\x03raw\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"\x1a\n\x03\x44ir\x12\t\n\x05HORIZ\x10\x00\x12\x08\n\x04VERT\x10\x01"/\n\rPrimitiveMode\x12\x08\n\x04PRIM\x10\x00\x12\t\n\x05SPLIT\x10\x01\x12\t\n\x05STACK\x10\x02"\xa3\x01\n\x08ViaLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x03top\x18\x02 \x01(\x0b\x32\x17.vlsir.tetris.LayerEnum\x12$\n\x03\x62ot\x18\x03 \x01(\x0b\x32\x17.vlsir.tetris.LayerEnum\x12\x1e\n\x04size\x18\x04 \x01(\x0b\x32\x10.vlsir.tetris.Xy\x12\x1d\n\x03raw\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"3\n\x0ePrimitiveLayer\x12!\n\x07pitches\x18\x01 \x01(\x0b\x32\x10.vlsir.tetris.Xy"\xce\x02\n\tTrackSpec\x12\x33\n\x05\x65ntry\x18\x01 \x01(\x0b\x32".vlsir.tetris.TrackSpec.TrackEntryH\x00\x12\x30\n\x06repeat\x18\x02 \x01(\x0b\x32\x1e.vlsir.tetris.TrackSpec.RepeatH\x00\x1a\x84\x01\n\nTrackEntry\x12;\n\x05ttype\x18\x01 \x01(\x0e\x32,.vlsir.tetris.TrackSpec.TrackEntry.TrackType\x12\r\n\x05width\x18\x02 \x01(\x03"*\n\tTrackType\x12\x07\n\x03GAP\x10\x00\x12\n\n\x06SIGNAL\x10\x01\x12\x08\n\x04RAIL\x10\x02\x1aK\n\x06Repeat\x12\x33\n\x07\x65ntries\x18\x01 \x03(\x0b\x32".vlsir.tetris.TrackSpec.TrackEntry\x12\x0c\n\x04nrep\x18\x02 \x01(\x03\x42\x06\n\x04spec"\x1a\n\x02Xy\x12\t\n\x01x\x18\x01 \x01(\x03\x12\t\n\x01y\x18\x02 \x01(\x03\x62\x06proto3'
+    b'\n\x0ctetris.proto\x12\x0cvlsir.tetris\x1a\x0butils.proto\x1a\traw.proto\x1a\rcircuit.proto"i\n\x07Library\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12!\n\x05\x63\x65lls\x18\n \x03(\x0b\x32\x12.vlsir.tetris.Cell\x12+\n\x06\x61uthor\x18\x14 \x01(\x0b\x32\x1b.vlsir.utils.AuthorMetadata"\xb8\x01\n\x04\x43\x65ll\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\tinterface\x18\n \x01(\x0b\x32\x18.vlsir.circuit.Interface\x12%\n\x06module\x18\x0b \x01(\x0b\x32\x15.vlsir.circuit.Module\x12(\n\x08\x61\x62stract\x18\x0c \x01(\x0b\x32\x16.vlsir.tetris.Abstract\x12$\n\x06layout\x18\r \x01(\x0b\x32\x14.vlsir.tetris.Layout"\xbc\x01\n\x06Layout\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x07outline\x18\n \x01(\x0b\x32\x15.vlsir.tetris.Outline\x12)\n\tinstances\x18\x14 \x03(\x0b\x32\x16.vlsir.tetris.Instance\x12)\n\x0b\x61ssignments\x18\x15 \x03(\x0b\x32\x14.vlsir.tetris.Assign\x12&\n\x04\x63uts\x18\x16 \x03(\x0b\x32\x18.vlsir.tetris.TrackCross";\n\x06\x41ssign\x12\x0b\n\x03net\x18\x01 \x01(\t\x12$\n\x02\x61t\x18\x02 \x01(\x0b\x32\x18.vlsir.tetris.TrackCross"Z\n\nTrackCross\x12%\n\x05track\x18\x01 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x12%\n\x05\x63ross\x18\x02 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef"(\n\x08TrackRef\x12\r\n\x05layer\x18\x01 \x01(\x03\x12\r\n\x05track\x18\x02 \x01(\x03"/\n\x07Outline\x12\t\n\x01x\x18\x01 \x03(\x03\x12\t\n\x01y\x18\x02 \x03(\x03\x12\x0e\n\x06metals\x18\x03 \x01(\x03"k\n\x08\x41\x62stract\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x07outline\x18\n \x01(\x0b\x32\x15.vlsir.tetris.Outline\x12)\n\x05ports\x18\x14 \x03(\x0b\x32\x1a.vlsir.tetris.AbstractPort"\x97\x04\n\x0c\x41\x62stractPort\x12\x0b\n\x03net\x18\x01 \x01(\t\x12\x33\n\x04\x65\x64ge\x18\n \x01(\x0b\x32#.vlsir.tetris.AbstractPort.EdgePortH\x00\x12<\n\tztop_edge\x18\x0b \x01(\x0b\x32\'.vlsir.tetris.AbstractPort.ZTopEdgePortH\x00\x12:\n\nztop_inner\x18\x0c \x01(\x0b\x32$.vlsir.tetris.AbstractPort.ZTopInnerH\x00\x1a\x64\n\x08\x45\x64gePort\x12%\n\x05track\x18\x01 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x12\x31\n\x04side\x18\x02 \x01(\x0e\x32#.vlsir.tetris.AbstractPort.PortSide\x1av\n\x0cZTopEdgePort\x12\r\n\x05track\x18\x01 \x01(\x03\x12\x31\n\x04side\x18\x02 \x01(\x0e\x32#.vlsir.tetris.AbstractPort.PortSide\x12$\n\x04into\x18\x03 \x01(\x0b\x32\x16.vlsir.tetris.TrackRef\x1a\x33\n\tZTopInner\x12&\n\x04locs\x18\x01 \x03(\x0b\x32\x18.vlsir.tetris.TrackCross"0\n\x08PortSide\x12\x12\n\x0e\x42OTTOM_OR_LEFT\x10\x00\x12\x10\n\x0cTOP_OR_RIGHT\x10\x01\x42\x06\n\x04kind"\x8d\x01\n\x08Instance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x04\x63\x65ll\x18\x03 \x01(\x0b\x32\x16.vlsir.utils.Reference\x12 \n\x03loc\x18\x04 \x01(\x0b\x32\x13.vlsir.tetris.Place\x12\x15\n\rreflect_horiz\x18\x06 \x01(\x08\x12\x14\n\x0creflect_vert\x18\x07 \x01(\x08"X\n\x05Place\x12\x1f\n\x03\x61\x62s\x18\x01 \x01(\x0b\x32\x10.vlsir.raw.PointH\x00\x12%\n\x03rel\x18\x02 \x01(\x0b\x32\x16.vlsir.tetris.RelPlaceH\x00\x42\x07\n\x05place"\n\n\x08RelPlace"\xce\x01\n\x05Stack\x12\x1f\n\x05units\x18\x01 \x01(\x0e\x32\x10.vlsir.raw.Units\x12*\n\x04prim\x18\x02 \x01(\x0b\x32\x1c.vlsir.tetris.PrimitiveLayer\x12(\n\x06metals\x18\x03 \x03(\x0b\x32\x18.vlsir.tetris.MetalLayer\x12$\n\x04vias\x18\x04 \x03(\x0b\x32\x16.vlsir.tetris.ViaLayer\x12(\n\x0e\x62oundary_layer\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"{\n\tLayerEnum\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.vlsir.tetris.LayerEnum.LayerType\x12\r\n\x05index\x18\x02 \x01(\x03".\n\tLayerType\x12\r\n\tPRIMITIVE\x10\x00\x12\t\n\x05METAL\x10\x01\x12\x07\n\x03VIA\x10\x02"\xd1\x02\n\nMetalLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x03\x64ir\x18\x02 \x01(\x0e\x32\x1c.vlsir.tetris.MetalLayer.Dir\x12\x0f\n\x07\x63utsize\x18\x03 \x01(\x03\x12(\n\x07\x65ntries\x18\x04 \x03(\x0b\x32\x17.vlsir.tetris.TrackSpec\x12\x0e\n\x06offset\x18\x05 \x01(\x03\x12\x0f\n\x07overlap\x18\x06 \x01(\x03\x12\x0c\n\x04\x66lip\x18\x07 \x01(\x08\x12\x34\n\x04prim\x18\x08 \x01(\x0e\x32&.vlsir.tetris.MetalLayer.PrimitiveMode\x12\x1d\n\x03raw\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"\x1a\n\x03\x44ir\x12\t\n\x05HORIZ\x10\x00\x12\x08\n\x04VERT\x10\x01"/\n\rPrimitiveMode\x12\x08\n\x04PRIM\x10\x00\x12\t\n\x05SPLIT\x10\x01\x12\t\n\x05STACK\x10\x02"\xa3\x01\n\x08ViaLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x03top\x18\x02 \x01(\x0b\x32\x17.vlsir.tetris.LayerEnum\x12$\n\x03\x62ot\x18\x03 \x01(\x0b\x32\x17.vlsir.tetris.LayerEnum\x12\x1e\n\x04size\x18\x04 \x01(\x0b\x32\x10.vlsir.tetris.Xy\x12\x1d\n\x03raw\x18\x0b \x01(\x0b\x32\x10.vlsir.raw.Layer"3\n\x0ePrimitiveLayer\x12!\n\x07pitches\x18\x01 \x01(\x0b\x32\x10.vlsir.tetris.Xy"\xce\x02\n\tTrackSpec\x12\x33\n\x05\x65ntry\x18\x01 \x01(\x0b\x32".vlsir.tetris.TrackSpec.TrackEntryH\x00\x12\x30\n\x06repeat\x18\x02 \x01(\x0b\x32\x1e.vlsir.tetris.TrackSpec.RepeatH\x00\x1a\x84\x01\n\nTrackEntry\x12;\n\x05ttype\x18\x01 \x01(\x0e\x32,.vlsir.tetris.TrackSpec.TrackEntry.TrackType\x12\r\n\x05width\x18\x02 \x01(\x03"*\n\tTrackType\x12\x07\n\x03GAP\x10\x00\x12\n\n\x06SIGNAL\x10\x01\x12\x08\n\x04RAIL\x10\x02\x1aK\n\x06Repeat\x12\x33\n\x07\x65ntries\x18\x01 \x03(\x0b\x32".vlsir.tetris.TrackSpec.TrackEntry\x12\x0c\n\x04nrep\x18\x02 \x01(\x03\x42\x06\n\x04spec"\x1a\n\x02Xy\x12\t\n\x01x\x18\x01 \x01(\x03\x12\t\n\x01y\x18\x02 \x01(\x03\x62\x06proto3'
 )
 
 
 _LIBRARY = DESCRIPTOR.message_types_by_name["Library"]
 _CELL = DESCRIPTOR.message_types_by_name["Cell"]
 _LAYOUT = DESCRIPTOR.message_types_by_name["Layout"]
 _ASSIGN = DESCRIPTOR.message_types_by_name["Assign"]
@@ -53,323 +53,323 @@
 _METALLAYER_PRIMITIVEMODE = _METALLAYER.enum_types_by_name["PrimitiveMode"]
 _TRACKSPEC_TRACKENTRY_TRACKTYPE = _TRACKSPEC_TRACKENTRY.enum_types_by_name["TrackType"]
 Library = _reflection.GeneratedProtocolMessageType(
     "Library",
     (_message.Message,),
     {
         "DESCRIPTOR": _LIBRARY,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Library)
     },
 )
 _sym_db.RegisterMessage(Library)
 
 Cell = _reflection.GeneratedProtocolMessageType(
     "Cell",
     (_message.Message,),
     {
         "DESCRIPTOR": _CELL,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Cell)
     },
 )
 _sym_db.RegisterMessage(Cell)
 
 Layout = _reflection.GeneratedProtocolMessageType(
     "Layout",
     (_message.Message,),
     {
         "DESCRIPTOR": _LAYOUT,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Layout)
     },
 )
 _sym_db.RegisterMessage(Layout)
 
 Assign = _reflection.GeneratedProtocolMessageType(
     "Assign",
     (_message.Message,),
     {
         "DESCRIPTOR": _ASSIGN,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Assign)
     },
 )
 _sym_db.RegisterMessage(Assign)
 
 TrackCross = _reflection.GeneratedProtocolMessageType(
     "TrackCross",
     (_message.Message,),
     {
         "DESCRIPTOR": _TRACKCROSS,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.TrackCross)
     },
 )
 _sym_db.RegisterMessage(TrackCross)
 
 TrackRef = _reflection.GeneratedProtocolMessageType(
     "TrackRef",
     (_message.Message,),
     {
         "DESCRIPTOR": _TRACKREF,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.TrackRef)
     },
 )
 _sym_db.RegisterMessage(TrackRef)
 
 Outline = _reflection.GeneratedProtocolMessageType(
     "Outline",
     (_message.Message,),
     {
         "DESCRIPTOR": _OUTLINE,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Outline)
     },
 )
 _sym_db.RegisterMessage(Outline)
 
 Abstract = _reflection.GeneratedProtocolMessageType(
     "Abstract",
     (_message.Message,),
     {
         "DESCRIPTOR": _ABSTRACT,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Abstract)
     },
 )
 _sym_db.RegisterMessage(Abstract)
 
 AbstractPort = _reflection.GeneratedProtocolMessageType(
     "AbstractPort",
     (_message.Message,),
     {
         "EdgePort": _reflection.GeneratedProtocolMessageType(
             "EdgePort",
             (_message.Message,),
             {
                 "DESCRIPTOR": _ABSTRACTPORT_EDGEPORT,
-                "__module__": "layout.tetris_pb2"
+                "__module__": "tetris_pb2"
                 # @@protoc_insertion_point(class_scope:vlsir.tetris.AbstractPort.EdgePort)
             },
         ),
         "ZTopEdgePort": _reflection.GeneratedProtocolMessageType(
             "ZTopEdgePort",
             (_message.Message,),
             {
                 "DESCRIPTOR": _ABSTRACTPORT_ZTOPEDGEPORT,
-                "__module__": "layout.tetris_pb2"
+                "__module__": "tetris_pb2"
                 # @@protoc_insertion_point(class_scope:vlsir.tetris.AbstractPort.ZTopEdgePort)
             },
         ),
         "ZTopInner": _reflection.GeneratedProtocolMessageType(
             "ZTopInner",
             (_message.Message,),
             {
                 "DESCRIPTOR": _ABSTRACTPORT_ZTOPINNER,
-                "__module__": "layout.tetris_pb2"
+                "__module__": "tetris_pb2"
                 # @@protoc_insertion_point(class_scope:vlsir.tetris.AbstractPort.ZTopInner)
             },
         ),
         "DESCRIPTOR": _ABSTRACTPORT,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.AbstractPort)
     },
 )
 _sym_db.RegisterMessage(AbstractPort)
 _sym_db.RegisterMessage(AbstractPort.EdgePort)
 _sym_db.RegisterMessage(AbstractPort.ZTopEdgePort)
 _sym_db.RegisterMessage(AbstractPort.ZTopInner)
 
 Instance = _reflection.GeneratedProtocolMessageType(
     "Instance",
     (_message.Message,),
     {
         "DESCRIPTOR": _INSTANCE,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Instance)
     },
 )
 _sym_db.RegisterMessage(Instance)
 
 Place = _reflection.GeneratedProtocolMessageType(
     "Place",
     (_message.Message,),
     {
         "DESCRIPTOR": _PLACE,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Place)
     },
 )
 _sym_db.RegisterMessage(Place)
 
 RelPlace = _reflection.GeneratedProtocolMessageType(
     "RelPlace",
     (_message.Message,),
     {
         "DESCRIPTOR": _RELPLACE,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.RelPlace)
     },
 )
 _sym_db.RegisterMessage(RelPlace)
 
 Stack = _reflection.GeneratedProtocolMessageType(
     "Stack",
     (_message.Message,),
     {
         "DESCRIPTOR": _STACK,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Stack)
     },
 )
 _sym_db.RegisterMessage(Stack)
 
 LayerEnum = _reflection.GeneratedProtocolMessageType(
     "LayerEnum",
     (_message.Message,),
     {
         "DESCRIPTOR": _LAYERENUM,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.LayerEnum)
     },
 )
 _sym_db.RegisterMessage(LayerEnum)
 
 MetalLayer = _reflection.GeneratedProtocolMessageType(
     "MetalLayer",
     (_message.Message,),
     {
         "DESCRIPTOR": _METALLAYER,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.MetalLayer)
     },
 )
 _sym_db.RegisterMessage(MetalLayer)
 
 ViaLayer = _reflection.GeneratedProtocolMessageType(
     "ViaLayer",
     (_message.Message,),
     {
         "DESCRIPTOR": _VIALAYER,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.ViaLayer)
     },
 )
 _sym_db.RegisterMessage(ViaLayer)
 
 PrimitiveLayer = _reflection.GeneratedProtocolMessageType(
     "PrimitiveLayer",
     (_message.Message,),
     {
         "DESCRIPTOR": _PRIMITIVELAYER,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.PrimitiveLayer)
     },
 )
 _sym_db.RegisterMessage(PrimitiveLayer)
 
 TrackSpec = _reflection.GeneratedProtocolMessageType(
     "TrackSpec",
     (_message.Message,),
     {
         "TrackEntry": _reflection.GeneratedProtocolMessageType(
             "TrackEntry",
             (_message.Message,),
             {
                 "DESCRIPTOR": _TRACKSPEC_TRACKENTRY,
-                "__module__": "layout.tetris_pb2"
+                "__module__": "tetris_pb2"
                 # @@protoc_insertion_point(class_scope:vlsir.tetris.TrackSpec.TrackEntry)
             },
         ),
         "Repeat": _reflection.GeneratedProtocolMessageType(
             "Repeat",
             (_message.Message,),
             {
                 "DESCRIPTOR": _TRACKSPEC_REPEAT,
-                "__module__": "layout.tetris_pb2"
+                "__module__": "tetris_pb2"
                 # @@protoc_insertion_point(class_scope:vlsir.tetris.TrackSpec.Repeat)
             },
         ),
         "DESCRIPTOR": _TRACKSPEC,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.TrackSpec)
     },
 )
 _sym_db.RegisterMessage(TrackSpec)
 _sym_db.RegisterMessage(TrackSpec.TrackEntry)
 _sym_db.RegisterMessage(TrackSpec.Repeat)
 
 Xy = _reflection.GeneratedProtocolMessageType(
     "Xy",
     (_message.Message,),
     {
         "DESCRIPTOR": _XY,
-        "__module__": "layout.tetris_pb2"
+        "__module__": "tetris_pb2"
         # @@protoc_insertion_point(class_scope:vlsir.tetris.Xy)
     },
 )
 _sym_db.RegisterMessage(Xy)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _LIBRARY._serialized_start = 83
-    _LIBRARY._serialized_end = 188
-    _CELL._serialized_start = 191
-    _CELL._serialized_end = 375
-    _LAYOUT._serialized_start = 378
-    _LAYOUT._serialized_end = 566
-    _ASSIGN._serialized_start = 568
-    _ASSIGN._serialized_end = 627
-    _TRACKCROSS._serialized_start = 629
-    _TRACKCROSS._serialized_end = 719
-    _TRACKREF._serialized_start = 721
-    _TRACKREF._serialized_end = 761
-    _OUTLINE._serialized_start = 763
-    _OUTLINE._serialized_end = 810
-    _ABSTRACT._serialized_start = 812
-    _ABSTRACT._serialized_end = 919
-    _ABSTRACTPORT._serialized_start = 922
-    _ABSTRACTPORT._serialized_end = 1457
-    _ABSTRACTPORT_EDGEPORT._serialized_start = 1126
-    _ABSTRACTPORT_EDGEPORT._serialized_end = 1226
-    _ABSTRACTPORT_ZTOPEDGEPORT._serialized_start = 1228
-    _ABSTRACTPORT_ZTOPEDGEPORT._serialized_end = 1346
-    _ABSTRACTPORT_ZTOPINNER._serialized_start = 1348
-    _ABSTRACTPORT_ZTOPINNER._serialized_end = 1399
-    _ABSTRACTPORT_PORTSIDE._serialized_start = 1401
-    _ABSTRACTPORT_PORTSIDE._serialized_end = 1449
-    _INSTANCE._serialized_start = 1460
-    _INSTANCE._serialized_end = 1601
-    _PLACE._serialized_start = 1603
-    _PLACE._serialized_end = 1691
-    _RELPLACE._serialized_start = 1693
-    _RELPLACE._serialized_end = 1703
-    _STACK._serialized_start = 1706
-    _STACK._serialized_end = 1912
-    _LAYERENUM._serialized_start = 1914
-    _LAYERENUM._serialized_end = 2037
-    _LAYERENUM_LAYERTYPE._serialized_start = 1991
-    _LAYERENUM_LAYERTYPE._serialized_end = 2037
-    _METALLAYER._serialized_start = 2040
-    _METALLAYER._serialized_end = 2377
-    _METALLAYER_DIR._serialized_start = 2302
-    _METALLAYER_DIR._serialized_end = 2328
-    _METALLAYER_PRIMITIVEMODE._serialized_start = 2330
-    _METALLAYER_PRIMITIVEMODE._serialized_end = 2377
-    _VIALAYER._serialized_start = 2380
-    _VIALAYER._serialized_end = 2543
-    _PRIMITIVELAYER._serialized_start = 2545
-    _PRIMITIVELAYER._serialized_end = 2596
-    _TRACKSPEC._serialized_start = 2599
-    _TRACKSPEC._serialized_end = 2933
-    _TRACKSPEC_TRACKENTRY._serialized_start = 2716
-    _TRACKSPEC_TRACKENTRY._serialized_end = 2848
-    _TRACKSPEC_TRACKENTRY_TRACKTYPE._serialized_start = 2806
-    _TRACKSPEC_TRACKENTRY_TRACKTYPE._serialized_end = 2848
-    _TRACKSPEC_REPEAT._serialized_start = 2850
-    _TRACKSPEC_REPEAT._serialized_end = 2925
-    _XY._serialized_start = 2935
-    _XY._serialized_end = 2961
+    _LIBRARY._serialized_start = 69
+    _LIBRARY._serialized_end = 174
+    _CELL._serialized_start = 177
+    _CELL._serialized_end = 361
+    _LAYOUT._serialized_start = 364
+    _LAYOUT._serialized_end = 552
+    _ASSIGN._serialized_start = 554
+    _ASSIGN._serialized_end = 613
+    _TRACKCROSS._serialized_start = 615
+    _TRACKCROSS._serialized_end = 705
+    _TRACKREF._serialized_start = 707
+    _TRACKREF._serialized_end = 747
+    _OUTLINE._serialized_start = 749
+    _OUTLINE._serialized_end = 796
+    _ABSTRACT._serialized_start = 798
+    _ABSTRACT._serialized_end = 905
+    _ABSTRACTPORT._serialized_start = 908
+    _ABSTRACTPORT._serialized_end = 1443
+    _ABSTRACTPORT_EDGEPORT._serialized_start = 1112
+    _ABSTRACTPORT_EDGEPORT._serialized_end = 1212
+    _ABSTRACTPORT_ZTOPEDGEPORT._serialized_start = 1214
+    _ABSTRACTPORT_ZTOPEDGEPORT._serialized_end = 1332
+    _ABSTRACTPORT_ZTOPINNER._serialized_start = 1334
+    _ABSTRACTPORT_ZTOPINNER._serialized_end = 1385
+    _ABSTRACTPORT_PORTSIDE._serialized_start = 1387
+    _ABSTRACTPORT_PORTSIDE._serialized_end = 1435
+    _INSTANCE._serialized_start = 1446
+    _INSTANCE._serialized_end = 1587
+    _PLACE._serialized_start = 1589
+    _PLACE._serialized_end = 1677
+    _RELPLACE._serialized_start = 1679
+    _RELPLACE._serialized_end = 1689
+    _STACK._serialized_start = 1692
+    _STACK._serialized_end = 1898
+    _LAYERENUM._serialized_start = 1900
+    _LAYERENUM._serialized_end = 2023
+    _LAYERENUM_LAYERTYPE._serialized_start = 1977
+    _LAYERENUM_LAYERTYPE._serialized_end = 2023
+    _METALLAYER._serialized_start = 2026
+    _METALLAYER._serialized_end = 2363
+    _METALLAYER_DIR._serialized_start = 2288
+    _METALLAYER_DIR._serialized_end = 2314
+    _METALLAYER_PRIMITIVEMODE._serialized_start = 2316
+    _METALLAYER_PRIMITIVEMODE._serialized_end = 2363
+    _VIALAYER._serialized_start = 2366
+    _VIALAYER._serialized_end = 2529
+    _PRIMITIVELAYER._serialized_start = 2531
+    _PRIMITIVELAYER._serialized_end = 2582
+    _TRACKSPEC._serialized_start = 2585
+    _TRACKSPEC._serialized_end = 2919
+    _TRACKSPEC_TRACKENTRY._serialized_start = 2702
+    _TRACKSPEC_TRACKENTRY._serialized_end = 2834
+    _TRACKSPEC_TRACKENTRY_TRACKTYPE._serialized_start = 2792
+    _TRACKSPEC_TRACKENTRY_TRACKTYPE._serialized_end = 2834
+    _TRACKSPEC_REPEAT._serialized_start = 2836
+    _TRACKSPEC_REPEAT._serialized_end = 2911
+    _XY._serialized_start = 2921
+    _XY._serialized_end = 2947
 # @@protoc_insertion_point(module_scope)
```

