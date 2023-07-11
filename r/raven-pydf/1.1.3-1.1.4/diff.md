# Comparing `tmp/raven-pydf-1.1.3.tar.gz` & `tmp/raven-pydf-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raven-pydf-1.1.3.tar", last modified: Sat Jan 15 23:55:49 2022, max compression
+gzip compressed data, was "raven-pydf-1.1.4.tar", last modified: Tue Jul 11 19:00:09 2023, max compression
```

## Comparing `raven-pydf-1.1.3.tar` & `raven-pydf-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.772509 raven-pydf-1.1.3/
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2574 2022-01-15 23:55:49.772509 raven-pydf-1.1.3/PKG-INFO
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2502 2022-01-15 22:43:39.000000 raven-pydf-1.1.3/README.md
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.768509 raven-pydf-1.1.3/raven/
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.768509 raven-pydf-1.1.3/raven/io/
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.768509 raven-pydf-1.1.3/raven/io/dataframe/
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)      689 2022-01-15 23:43:40.000000 raven-pydf-1.1.3/raven/io/dataframe/__init__.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    12884 2022-01-15 23:44:00.000000 raven-pydf-1.1.3/raven/io/dataframe/csvfiles.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    36874 2022-01-15 23:44:08.000000 raven-pydf-1.1.3/raven/io/dataframe/dataframes.py
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.768509 raven-pydf-1.1.3/raven/struct/
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.772509 raven-pydf-1.1.3/raven/struct/dataframe/
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     1997 2022-01-15 23:44:25.000000 raven-pydf-1.1.3/raven/struct/dataframe/__init__.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    11255 2022-01-15 23:44:37.000000 raven-pydf-1.1.3/raven/struct/dataframe/_columnutils.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    44189 2022-01-15 23:44:47.000000 raven-pydf-1.1.3/raven/struct/dataframe/_dataframeutils.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    25896 2022-01-15 23:44:54.000000 raven-pydf-1.1.3/raven/struct/dataframe/binarycolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19867 2022-01-15 23:45:01.000000 raven-pydf-1.1.3/raven/struct/dataframe/booleancolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19468 2022-01-15 23:45:06.000000 raven-pydf-1.1.3/raven/struct/dataframe/bytecolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    27993 2022-01-15 23:45:17.000000 raven-pydf-1.1.3/raven/struct/dataframe/charcolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19706 2022-01-15 23:45:30.000000 raven-pydf-1.1.3/raven/struct/dataframe/column.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)   213120 2022-01-15 23:45:54.000000 raven-pydf-1.1.3/raven/struct/dataframe/core.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19165 2022-01-15 23:46:02.000000 raven-pydf-1.1.3/raven/struct/dataframe/doublecolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19166 2022-01-15 23:46:10.000000 raven-pydf-1.1.3/raven/struct/dataframe/floatcolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19585 2022-01-15 23:46:17.000000 raven-pydf-1.1.3/raven/struct/dataframe/intcolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19669 2022-01-15 23:46:24.000000 raven-pydf-1.1.3/raven/struct/dataframe/longcolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19592 2022-01-15 23:46:32.000000 raven-pydf-1.1.3/raven/struct/dataframe/shortcolumn.py
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    23775 2022-01-15 23:46:40.000000 raven-pydf-1.1.3/raven/struct/dataframe/stringcolumn.py
-drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2022-01-15 23:55:49.772509 raven-pydf-1.1.3/raven_pydf.egg-info/
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2574 2022-01-15 23:55:49.000000 raven-pydf-1.1.3/raven_pydf.egg-info/PKG-INFO
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)      842 2022-01-15 23:55:49.000000 raven-pydf-1.1.3/raven_pydf.egg-info/SOURCES.txt
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)        1 2022-01-15 23:55:49.000000 raven-pydf-1.1.3/raven_pydf.egg-info/dependency_links.txt
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)       14 2022-01-15 23:55:49.000000 raven-pydf-1.1.3/raven_pydf.egg-info/requires.txt
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)        6 2022-01-15 23:55:49.000000 raven-pydf-1.1.3/raven_pydf.egg-info/top_level.txt
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)       38 2022-01-15 23:55:49.772509 raven-pydf-1.1.3/setup.cfg
--rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     1551 2022-01-15 23:53:01.000000 raven-pydf-1.1.3/setup.py
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2574 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/PKG-INFO
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2502 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/README.md
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven/
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven/io/
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven/io/dataframe/
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)      689 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/io/dataframe/__init__.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    12884 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/io/dataframe/csvfiles.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    36862 2023-07-11 18:35:35.000000 raven-pydf-1.1.4/raven/io/dataframe/dataframes.py
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven/struct/
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven/struct/dataframe/
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     1997 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/struct/dataframe/__init__.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    11255 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/struct/dataframe/_columnutils.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    44177 2023-07-11 18:35:44.000000 raven-pydf-1.1.4/raven/struct/dataframe/_dataframeutils.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    25818 2023-07-11 18:35:52.000000 raven-pydf-1.1.4/raven/struct/dataframe/binarycolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19750 2023-07-11 18:35:57.000000 raven-pydf-1.1.4/raven/struct/dataframe/booleancolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19378 2023-07-11 18:36:08.000000 raven-pydf-1.1.4/raven/struct/dataframe/bytecolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    27906 2023-07-11 18:36:16.000000 raven-pydf-1.1.4/raven/struct/dataframe/charcolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19706 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/struct/dataframe/column.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)   213120 2022-01-16 09:49:42.000000 raven-pydf-1.1.4/raven/struct/dataframe/core.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19075 2023-07-11 18:36:25.000000 raven-pydf-1.1.4/raven/struct/dataframe/doublecolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19076 2023-07-11 18:37:23.000000 raven-pydf-1.1.4/raven/struct/dataframe/floatcolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19495 2023-07-11 18:37:02.000000 raven-pydf-1.1.4/raven/struct/dataframe/intcolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19579 2023-07-11 18:36:55.000000 raven-pydf-1.1.4/raven/struct/dataframe/longcolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    19502 2023-07-11 18:36:48.000000 raven-pydf-1.1.4/raven/struct/dataframe/shortcolumn.py
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)    23679 2023-07-11 18:36:41.000000 raven-pydf-1.1.4/raven/struct/dataframe/stringcolumn.py
+drwxrwxr-x   0 kilo52    (1000) kilo52    (1000)        0 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/raven_pydf.egg-info/
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     2574 2023-07-11 19:00:09.000000 raven-pydf-1.1.4/raven_pydf.egg-info/PKG-INFO
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)      842 2023-07-11 19:00:09.000000 raven-pydf-1.1.4/raven_pydf.egg-info/SOURCES.txt
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)        1 2023-07-11 19:00:09.000000 raven-pydf-1.1.4/raven_pydf.egg-info/dependency_links.txt
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)       14 2023-07-11 19:00:09.000000 raven-pydf-1.1.4/raven_pydf.egg-info/requires.txt
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)        6 2023-07-11 19:00:09.000000 raven-pydf-1.1.4/raven_pydf.egg-info/top_level.txt
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)       38 2023-07-11 19:00:09.827933 raven-pydf-1.1.4/setup.cfg
+-rw-rw-r--   0 kilo52    (1000) kilo52    (1000)     1555 2023-07-11 18:39:29.000000 raven-pydf-1.1.4/setup.py
```

### Comparing `raven-pydf-1.1.3/PKG-INFO` & `raven-pydf-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-pydf
-Version: 1.1.3
+Version: 1.1.4
 Summary: An implementation of the DataFrame specification in Python
 Home-page: https://github.com/raven-computing/pydf
 Author: Phil Gaiser
 Author-email: phil.gaiser@raven-computing.com
 License: Apache Software License
 Description: This is the official implementation of the DataFrame specification provided by Raven Computing.
```

### Comparing `raven-pydf-1.1.3/README.md` & `raven-pydf-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/io/dataframe/__init__.py` & `raven-pydf-1.1.4/raven/io/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/io/dataframe/csvfiles.py` & `raven-pydf-1.1.4/raven/io/dataframe/csvfiles.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/io/dataframe/dataframes.py` & `raven-pydf-1.1.4/raven/io/dataframe/dataframes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -662,15 +662,15 @@
         if buffer[ptr] != 0x7d: # header closing brace '}' missing
             raise dataframe.DataFrameException("Invalid format")
 
         #END HEADER
 
         #PAYLOAD
         for i in range(cols):
-            val = np.empty(rows, dtype=np.object)
+            val = np.empty(rows, dtype=object)
             if types[i] == bytecolumn.NullableByteColumn.TYPE_CODE:
                 for j in range(rows):
                     ptr += 1
                     b = int.from_bytes(buffer[ptr:ptr+1], byteorder="big", signed=True)
                     if b == 0:
                         if not lookup_bits.get(li):
                             val[j] = 0
@@ -860,15 +860,15 @@
                 for j in range(rows):
                     ptr += 8
                     val[j] = int.from_bytes(buffer[ptr-7:ptr+1], byteorder="big", signed=True)
 
                 columns.append(longcolumn.LongColumn(names[i], val))
 
             elif types[i] == stringcolumn.StringColumn.TYPE_CODE:
-                val = np.empty(rows, dtype=np.object)
+                val = np.empty(rows, dtype=object)
                 for j in range(rows):
                     ptr += 1
                     c0 = ptr # marks the first character of each string
                     while buffer[ptr] != 0x00:
                         ptr += 1
 
                     if (ptr-c0) == 0:
@@ -902,26 +902,26 @@
                     ptr += 1
                     c = int.from_bytes(buffer[ptr:ptr+1], byteorder="big", signed=False)
                     val[j] = c
 
                 columns.append(charcolumn.CharColumn(names[i], val))
 
             elif types[i] == booleancolumn.BooleanColumn.TYPE_CODE:
-                val = np.empty(rows, dtype=np.bool)
+                val = np.empty(rows, dtype=bool)
                 length = int(rows/8 if (rows%8 == 0) else ((rows/8) + 1))
                 ptr += 1 # focus on next readable position
                 bits = BitVector(buffer[ptr:ptr+length])
                 for j in range(rows):
                     val[j] = bits.get(j)
 
                 ptr += (length-1)
                 columns.append(booleancolumn.BooleanColumn(names[i], val))
 
             elif types[i] == binarycolumn.BinaryColumn.TYPE_CODE:
-                val = np.empty(rows, dtype=np.object)
+                val = np.empty(rows, dtype=object)
                 for j in range(rows):
                     ptr += 1
                     length = int.from_bytes(buffer[ptr:ptr+4], byteorder="big", signed=False)
                     ptr += 3
                     data = bytearray(length)
                     for k in range(length):
                         ptr += 1
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/__init__.py` & `raven-pydf-1.1.4/raven/struct/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/_columnutils.py` & `raven-pydf-1.1.4/raven/struct/dataframe/_columnutils.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/_dataframeutils.py` & `raven-pydf-1.1.4/raven/struct/dataframe/_dataframeutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -286,15 +286,15 @@
                 vals = np.array([0] * rows, dtype=np.int64)
                 for i in range(rows):
                     val = col.get_value(i)
                     vals[i] = 0 if val is None else val
 
                 converted.add_column(longcolumn.LongColumn(col.get_name(), vals))
             elif tc == stringcolumn.NullableStringColumn.TYPE_CODE:
-                vals = np.array([None] * rows, dtype=np.object)
+                vals = np.array([None] * rows, dtype=object)
                 for i in range(rows):
                     val = col.get_value(i)
                     vals[i] = (stringcolumn.StringColumn.DEFAULT_VALUE
                                if val is None or val == ""
                                else val)
 
                 converted.add_column(stringcolumn.StringColumn(col.get_name(), vals))
@@ -317,37 +317,37 @@
                 default_val = ord(charcolumn.CharColumn.DEFAULT_VALUE)
                 for i in range(rows):
                     val = col._values[i]
                     vals[i] = default_val if val is None else val
 
                 converted.add_column(charcolumn.CharColumn(col.get_name(), vals))
             elif tc == booleancolumn.NullableBooleanColumn.TYPE_CODE:
-                vals = np.array([False] * rows, dtype=np.bool)
+                vals = np.array([False] * rows, dtype=bool)
                 for i in range(rows):
                     val = col.get_value(i)
                     vals[i] = False if val is None else val
 
                 converted.add_column(booleancolumn.BooleanColumn(col.get_name(), vals))
             elif tc == binarycolumn.NullableBinaryColumn.TYPE_CODE:
-                vals = np.array([None] * rows, dtype=np.object)
+                vals = np.array([None] * rows, dtype=object)
                 for i in range(rows):
                     val = col.get_value(i)
                     vals[i] = bytearray.fromhex("00") if val is None else val
 
                 converted.add_column(binarycolumn.BinaryColumn(col.get_name(), vals))
             else: # undefined type
                 raise dataframe.DataFrameException(
                     ("Unable to convert dataframe. Unrecognized "
                      "column type {}".format(type(col))))
 
     else: # convert from Default to Nullable
         converted = dataframe.NullableDataFrame()
         for col in df:
             tc = col.type_code()
-            vals = np.array([None] * rows, dtype=np.object)
+            vals = np.array([None] * rows, dtype=object)
             for i in range(rows):
                 vals[i] = col.get_value(i)
 
             if tc == bytecolumn.ByteColumn.TYPE_CODE:
                 converted.add_column(bytecolumn.NullableByteColumn(col.get_name(), vals))
             elif tc == shortcolumn.ShortColumn.TYPE_CODE:
                 converted.add_column(shortcolumn.NullableShortColumn(col.get_name(), vals))
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/binarycolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/binarycolumn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -169,15 +169,15 @@
                 if x is not None and len(x) >= 8:
                     vals[i] = int.from_bytes(x[0:8], byteorder="big", signed=True)
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = x.hex()
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -205,15 +205,15 @@
                 if x is not None and len(x) > 0:
                     vals[i] = int(x[0])
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     is_zero = True
                     for y in x:
                         if y != 0:
                             is_zero = False
                             break
@@ -222,102 +222,102 @@
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == BinaryColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     vals[i] = x[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 2:
                     vals[i] = int.from_bytes(x[0:2], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 4:
                     vals[i] = int.from_bytes(x[0:4], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 8:
                     vals[i] = int.from_bytes(x[0:8], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = x.hex()
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 4:
                     vals[i] = unpack(">f", x[0:4])[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 8:
                     vals[i] = unpack(">d", x[0:8])[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     vals[i] = int(x[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     is_zero = True
                     for y in x:
                         if y != 0:
                             is_zero = False
                             break
 
                     vals[i] = not is_zero
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == NullableBinaryColumn.TYPE_CODE:
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     b = bytearray(len(x))
                     b[:] = x
                     vals[i] = b
                 else:
                     vals[i] = None
@@ -328,15 +328,15 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        array = np.empty(size, dtype=np.object)
+        array = np.empty(size, dtype=object)
         for i in range(size):
             array[i] = self.get_default_value()
 
         return array
 
 class NullableBinaryColumn(column.Column):
     """A Column holding nullable binary values (bytearray).
@@ -476,15 +476,15 @@
                 if x is not None and len(x) >= 8:
                     vals[i] = int.from_bytes(x[0:8], byteorder="big", signed=True)
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = x.hex()
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -513,113 +513,113 @@
                 if x is not None and len(x) > 0:
                     vals[i] = int(x[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     is_zero = True
                     for y in x:
                         if y != 0:
                             is_zero = False
                             break
 
                     vals[i] = not is_zero
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == BinaryColumn.TYPE_CODE:
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     b = bytearray(len(x))
                     b[:] = x
                     vals[i] = b
                 else:
                     vals[i] = bytearray(b"\x00")
 
             converted = BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     vals[i] = x[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 2:
                     vals[i] = int.from_bytes(x[0:2], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 4:
                     vals[i] = int.from_bytes(x[0:4], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 8:
                     vals[i] = int.from_bytes(x[0:8], byteorder="big", signed=True)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = x.hex()
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 4:
                     vals[i] = unpack(">f", x[0:4])[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) >= 8:
                     vals[i] = unpack(">d", x[0:8])[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None and len(x) > 0:
                     vals[i] = int(x[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     is_zero = True
                     for y in x:
                         if y != 0:
                             is_zero = False
                             break
@@ -636,8 +636,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/booleancolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/longcolumn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,484 +1,479 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-Provides an implementation for BooleanColumn and NullableBooleanColumn
+Provides an implementation for LongColumn and NullableLongColumn
 """
 
 import numpy as np
 
 import raven.struct.dataframe.core as dataframe
 import raven.struct.dataframe.column as column
 import raven.struct.dataframe._columnutils as utils
 
-class BooleanColumn(column.Column):
-    """A Column holding boolean values (bool).
+class LongColumn(column.Column):
+    """A Column holding long values (int64).
     This implementation DOES NOT support null values.
     """
 
-    TYPE_CODE = 9
+    TYPE_CODE = 4
 
     def __init__(self, name=None, values=None):
-        """Constructs a new BooleanColumn.
+        """Constructs a new LongColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the BooleanColumn as a string
-            values: The content of the BooleanColumn.
-                Must be a list or numpy array with dtype bool, or an int
+            name: The name of the LongColumn as a string
+            values: The content of the LongColumn.
+                Must be a list or numpy array with dtype int64, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.bool)
+            values = np.empty(0, dtype=np.int64)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.bool)
+            values = np.array(values, dtype=np.int64)
 
         elif isinstance(values, np.ndarray):
-            if values.dtype != "bool":
+            if values.dtype != "int64":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "boolean array (bool) but found {}".format(values.dtype)))
+                     "long array (int64) but found {}".format(values.dtype)))
 
         elif isinstance(values, int):
-            values = np.zeros(values, dtype=np.bool)
+            values = np.zeros(values, dtype=np.int64)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
         if value is None:
             raise dataframe.DataFrameException(
                 ("Invalid argument. "
-                 "BooleanColumn cannot use None values"))
+                 "LongColumn cannot use None values"))
 
-        if not isinstance(value, (bool, np.bool, np.bool_)):
+        if isinstance(value, int):
+            if (value < -9223372036854775808) or (value > 9223372036854775807):
+                raise dataframe.DataFrameException(
+                    "Out of range long (int64): {}".format(value))
+
+        elif not isinstance(value, np.int64):
             raise dataframe.DataFrameException(
                 ("Invalid argument. Expected "
-                 "boolean (bool) but found {}").format(type(value)))
+                 "long (int64) but found {}".format(type(value))))
 
     def get_value(self, index):
-        """Gets the boolean value at the specified index
+        """Gets the long value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The boolean value at the specified index. Is never None
+            The long value at the specified index. Is never None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
-        val = self._values[index]
-        return bool(val)
-
-    def set_value(self, index, value):
-        """Sets the boolean value at the specified index
-
-        Args:
-            index: The index of the boolean value to set
-            value: The boolean value to set at the specified position.
-                Must be a boolean
-
-        Raises:
-            ValueError: If the specified index is out of bounds or of the
-                object provided is of the wrong type
-        """
-        self._check_bounds(index)
-        self._check_type(value)
-        self._values[index] = value
+        return int(self._values[index])
 
     def type_code(self):
-        return BooleanColumn.TYPE_CODE
+        return LongColumn.TYPE_CODE
 
     def type_name(self):
-        return "boolean"
+        return "long"
 
     def is_nullable(self):
         return False
 
     def is_numeric(self):
-        return False
+        return True
 
     def get_default_value(self):
-        return False
+        return 0
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=invalid-name
     def convert_to(self, typecode):
         converted = None
         if typecode == utils.type_code_byte_column():
             converted = dataframe.DataFrame.ByteColumn(values=self._values.astype(np.int8))
         elif typecode == utils.type_code_short_column():
             converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
-        elif typecode == utils.type_code_long_column():
-            converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
+        elif typecode == LongColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == utils.type_code_double_column():
             converted = dataframe.DataFrame.DoubleColumn(values=self._values.astype(np.float64))
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
-                if x:
-                    vals[i] = ord("1")
-                else:
-                    vals[i] = ord("0")
+                vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
-        elif typecode == BooleanColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_boolean_column():
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_short_column():
             vals = self._values.astype(np.int16)
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_int_column():
             vals = self._values.astype(np.int32)
-            converted = dataframe.DataFrame.NullableIntColumn(values=self._values.astype(np.object))
-        elif typecode == utils.type_code_nullable_long_column():
-            vals = self._values.astype(np.int64)
-            converted = dataframe.DataFrame.NullableLongColumn(
-                values=self._values.astype(np.object))
-
+            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(object))
+        elif typecode == NullableLongColumn.TYPE_CODE:
+            converted = NullableLongColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.uint8)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
-                if x:
-                    vals[i] = ord("1")
-                else:
-                    vals[i] = ord("0")
+                vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
-        elif typecode == NullableBooleanColumn.TYPE_CODE:
-            converted = NullableBooleanColumn(values=self._values.astype(np.object))
+        elif typecode == utils.type_code_nullable_boolean_column():
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
+            converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.zeros(size, dtype=np.bool)
+        return np.zeros(size, dtype=np.int64)
 
-class NullableBooleanColumn(column.Column):
-    """A Column holding nullable boolean values.
+class NullableLongColumn(column.Column):
+    """A Column holding nullable long values.
     Any values not explicitly set are considered None.
     """
 
-    TYPE_CODE = 18
+    TYPE_CODE = 13
 
     def __init__(self, name=None, values=None):
-        """Constructs a new NullableBooleanColumn.
+        """Constructs a new NullableLongColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the NullableBooleanColumn as a string
-            values: The content of the NullableBooleanColumn.
+            name: The name of the NullableLongColumn as a string
+            values: The content of the NullableLongColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "boolean array (object) but found {}".format(values.dtype)))
+                     "long array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
-        if value is not None:
-            if not isinstance(value, (bool, np.bool, np.bool_)):
+        if isinstance(value, int):
+            if (value < -9223372036854775808) or (value > 9223372036854775807):
                 raise dataframe.DataFrameException(
-                    ("Invalid argument. Expected "
-                     "boolean (bool) but found {}").format(type(value)))
+                    "Out of range long (int64): {}".format(value))
+
+        elif value is not None and not isinstance(value, np.int64):
+            raise dataframe.DataFrameException(
+                ("Invalid argument. Expected "
+                 "long (int64) but found {}".format(type(value))))
 
     def get_value(self, index):
-        """Gets the boolean value at the specified index
+        """Gets the long value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The boolean value at the specified index. May be None
+            The long value at the specified index. May be None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
         val = self._values[index]
         if val is None:
             return None
-
-        return bool(val)
-
-    def set_value(self, index, value):
-        """Sets the boolean value at the specified index
-
-        Args:
-            index: The index of the boolean value to set
-            value: The boolean value to set at the specified position.
-                Must be a boolean or None
-
-        Raises:
-            ValueError: If the specified index is out of bounds or of the
-                object provided is of the wrong type
-        """
-        self._check_bounds(index)
-        self._check_type(value)
-        self._values[index] = value
+        else:
+            return int(val)
 
     def type_code(self):
-        return NullableBooleanColumn.TYPE_CODE
+        return NullableLongColumn.TYPE_CODE
 
     def type_name(self):
-        return "boolean"
+        return "long"
 
     def is_nullable(self):
         return True
 
     def is_numeric(self):
-        return False
+        return True
 
     def get_default_value(self):
         return None
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=invalid-name
     def convert_to(self, typecode):
         converted = None
         if typecode == utils.type_code_byte_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int8)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else 0
+                if x is not None:
+                    vals[i] = int(np.int8(x))
+                else:
+                    vals[i] = 0
 
             converted = dataframe.DataFrame.ByteColumn(values=vals)
         elif typecode == utils.type_code_short_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int16)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else 0
+                if x is not None:
+                    vals[i] = int(np.int16(x))
+                else:
+                    vals[i] = 0
 
             converted = dataframe.DataFrame.ShortColumn(values=vals)
         elif typecode == utils.type_code_int_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int32)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else 0
+                if x is not None:
+                    vals[i] = int(np.int32(x))
+                else:
+                    vals[i] = 0
 
             converted = dataframe.DataFrame.IntColumn(values=vals)
-        elif typecode == utils.type_code_long_column():
+        elif typecode == LongColumn.TYPE_CODE:
             vals = np.empty([self._values.shape[0]], dtype=np.int64)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else 0
+                if x is not None:
+                    vals[i] = int(np.int64(x))
+                else:
+                    vals[i] = 0
 
-            converted = dataframe.DataFrame.LongColumn(values=vals)
+            converted = LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float32)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = float(x) if x is not None else 0.0
+                if x is not None:
+                    vals[i] = float(x)
+                else:
+                    vals[i] = 0.0
 
             converted = dataframe.DataFrame.FloatColumn(values=vals)
         elif typecode == utils.type_code_double_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float64)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = float(x) if x is not None else 0.0
+                if x is not None:
+                    vals[i] = float(x)
+                else:
+                    vals[i] = 0.0
 
             converted = dataframe.DataFrame.DoubleColumn(values=vals)
         elif typecode == utils.type_code_char_column():
             vals = np.zeros([self._values.shape[0]], dtype=np.uint8)
+            ord_default = ord(utils.default_value_char_column())
             for i, x in np.ndenumerate(self._values):
-                if x is not None and x is True:
-                    vals[i] = ord("1")
+                if x is not None:
+                    vals[i] = ord(str(x)[0])
                 else:
-                    vals[i] = ord("0")
+                    vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
-        elif typecode == BooleanColumn.TYPE_CODE:
-            vals = self._values.astype(np.bool)
-            for i, x in np.ndenumerate(vals):
-                if x is not None and x is True:
-                    vals[i] = True
+        elif typecode == utils.type_code_boolean_column():
+            vals = np.empty([self._values.shape[0]], dtype=bool)
+            for i, x in np.ndenumerate(self._values):
+                if x is not None:
+                    vals[i] = (x != 0)
                 else:
                     vals[i] = False
 
-            converted = BooleanColumn(values=vals)
+            converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
                 else:
-                    vals[i] = bytearray(int(0).to_bytes(1, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(0).to_bytes(8, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else None
+                vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else None
+                vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else None
+                vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
-        elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
-            for i, x in np.ndenumerate(self._values):
-                vals[i] = int(x) if x is not None else None
-
-            converted = dataframe.DataFrame.NullableLongColumn(values=vals)
+        elif typecode == NullableLongColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
-            for i, x in np.ndenumerate(vals):
-                vals[i] = str(x) if x is not None else None
+            vals = np.empty([self._values.shape[0]], dtype=object)
+            for i, x in np.ndenumerate(self._values):
+                if x is not None:
+                    vals[i] = str(x)
+                else:
+                    vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = float(x) if x is not None else None
+                if x is not None:
+                    vals[i] = float(x)
+                else:
+                    vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = float(x) if x is not None else None
+                if x is not None:
+                    vals[i] = float(x)
+                else:
+                    vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
-            vals = vals.astype(np.object)
-            for i, x in np.ndenumerate(vals):
+            vals = np.empty([self._values.shape[0]], dtype=object)
+            for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    if x is True:
-                        vals[i] = ord("1")
-                    else:
-                        vals[i] = ord("0")
+                    vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
-        elif typecode == NullableBooleanColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_nullable_boolean_column():
+            vals = np.empty([self._values.shape[0]], dtype=object)
+            for i, x in np.ndenumerate(self._values):
+                if x is not None:
+                    vals[i] = (x != 0)
+                else:
+                    vals[i] = None
+
+            converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/bytecolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/bytecolumn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -124,15 +124,15 @@
         elif typecode == utils.type_code_short_column():
             converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
         elif typecode == utils.type_code_long_column():
             converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == utils.type_code_double_column():
@@ -140,59 +140,59 @@
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == NullableByteColumn.TYPE_CODE:
-            converted = NullableByteColumn(values=self._values.astype(np.object))
+            converted = NullableByteColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_short_column():
             converted = dataframe.DataFrame.NullableShortColumn(
-                values=self._values.astype(np.object))
+                values=self._values.astype(object))
 
         elif typecode == utils.type_code_nullable_int_column():
-            converted = dataframe.DataFrame.NullableIntColumn(values=self._values.astype(np.object))
+            converted = dataframe.DataFrame.NullableIntColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_long_column():
             converted = dataframe.DataFrame.NullableLongColumn(
-                values=self._values.astype(np.object))
+                values=self._values.astype(object))
 
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
@@ -223,33 +223,33 @@
 
         Args:
             name: The name of the NullableByteColumn as a string
             values: The content of the NullableByteColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "byte array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
@@ -336,15 +336,15 @@
                 if x is not None:
                     vals[i] = int(x)
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -373,98 +373,98 @@
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
                 else:
                     vals[i] = bytearray(int(0).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == NullableByteColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int64(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -473,8 +473,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/charcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/charcolumn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -199,15 +199,15 @@
         elif typecode == utils.type_code_long_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int64)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x))
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = chr(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float32)
             for i, x in np.ndenumerate(self._values):
@@ -221,93 +221,93 @@
 
             converted = dataframe.DataFrame.DoubleColumn(values=vals)
         elif typecode == CharColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_boolean_column():
             values_true = {"t", "1", "y"}
             values_false = {"f", "0", "n"}
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 x = chr(x).lower()
                 is_true = x in values_true
                 is_false = x in values_false
                 if not is_true and not is_false:
                     raise dataframe.DataFrameException(
                         ("Invalid boolean character: '{}'".format(self._values[i])))
 
                 vals[i] = is_true
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(chr(x).encode("utf-8"))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x))
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x))
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x))
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x))
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = chr(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = float(chr(x))
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = float(chr(x))
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == NullableCharColumn.TYPE_CODE:
-            converted = NullableCharColumn(values=self._values.astype(np.object))
+            converted = NullableCharColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_boolean_column():
             values_true = {"t", "1", "y"}
             values_false = {"f", "0", "n"}
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 x = chr(x).lower()
                 is_true = x in values_true
                 is_false = x in values_false
                 if not is_true and not is_false:
                     raise dataframe.DataFrameException(
                         ("Invalid boolean character: '{}'".format(self._values[i])))
 
                 vals[i] = is_true
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(chr(x).encode("utf-8"))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
@@ -351,18 +351,18 @@
 
         Args:
             name: The name of the NullableCharColumn as a string
             values: The content of the NullableCharColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
-            charvals = np.zeros(len(values), dtype=np.object)
+            charvals = np.zeros(len(values), dtype=object)
             for i, value in enumerate(values):
                 self._check_type(value)
                 if value is None:
                     charvals[i] = None
                 else:
                     charvals[i] = ord(value)
 
@@ -399,15 +399,15 @@
 
                     else:
                         raise dataframe.DataFrameException(
                             ("Invalid argument. Expected "
                              "char (str) but found {}".format(type(value))))
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
@@ -532,15 +532,15 @@
         elif typecode == utils.type_code_long_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int64)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x)) if x is not None else 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = chr(x) if x is not None else utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float32)
             for i, x in np.ndenumerate(self._values):
@@ -559,15 +559,15 @@
             for i, x in np.ndenumerate(self._values):
                 vals[i] = x if x is not None else ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
             values_true = {"t", "1", "y"}
             values_false = {"f", "0", "n"}
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     x = chr(x).lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -575,70 +575,70 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(chr(x).encode("utf-8"))
                 else:
                     vals[i] = bytearray.fromhex("00")
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = chr(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = float(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = float(chr(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == NullableCharColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_boolean_column():
             values_true = {"t", "1", "y"}
             values_false = {"f", "0", "n"}
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     x = chr(x).lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -646,15 +646,15 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(chr(x).encode("utf-8"))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -663,8 +663,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/column.py` & `raven-pydf-1.1.4/raven/struct/dataframe/column.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/core.py` & `raven-pydf-1.1.4/raven/struct/dataframe/core.py`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/doublecolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/doublecolumn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -121,15 +121,15 @@
         elif typecode == utils.type_code_short_column():
             converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
         elif typecode == utils.type_code_long_column():
             converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == DoubleColumn.TYPE_CODE:
@@ -137,57 +137,57 @@
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(pack(">d", x))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_short_column():
             vals = self._values.astype(np.int16)
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_int_column():
             vals = self._values.astype(np.int32)
-            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_long_column():
             vals = self._values.astype(np.int64)
-            converted = dataframe.DataFrame.NullableLongColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableLongColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == NullableDoubleColumn.TYPE_CODE:
-            converted = NullableDoubleColumn(values=self._values.astype(np.object))
+            converted = NullableDoubleColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(pack(">d", x))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
@@ -218,33 +218,33 @@
 
         Args:
             name: The name of the NullableDoubleColumn as a string
             values: The content of the NullableDoubleColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "double array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
@@ -327,15 +327,15 @@
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -364,95 +364,95 @@
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0.0)
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(pack(">d", x))
                 else:
                     vals[i] = bytearray(pack(">d", 0.0))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int64(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(np.float32(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == NullableDoubleColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0.0)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(pack(">d", x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -461,8 +461,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/floatcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/floatcolumn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -121,15 +121,15 @@
         elif typecode == utils.type_code_short_column():
             converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
         elif typecode == utils.type_code_long_column():
             converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == FloatColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_double_column():
@@ -137,58 +137,58 @@
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(pack(">f", x))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_short_column():
             vals = self._values.astype(np.int16)
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_int_column():
             vals = self._values.astype(np.int32)
-            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_long_column():
             vals = self._values.astype(np.int64)
-            converted = dataframe.DataFrame.NullableLongColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableLongColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == NullableFloatColumn.TYPE_CODE:
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             converted = NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(pack(">f", x))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
@@ -219,33 +219,33 @@
 
         Args:
             name: The name of the NullableFloatColumn as a string
             values: The content of the NullableFloatColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "float array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
@@ -328,15 +328,15 @@
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -365,95 +365,95 @@
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0.0)
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(pack(">f", x))
                 else:
                     vals[i] = bytearray(pack(">f", 0.0))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int64(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == NullableFloatColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(np.float64(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0.0)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(pack(">f", x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -462,8 +462,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/intcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/intcolumn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -124,15 +124,15 @@
         elif typecode == utils.type_code_short_column():
             converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == IntColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_long_column():
             converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == utils.type_code_double_column():
@@ -140,59 +140,59 @@
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(int(x).to_bytes(4, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_short_column():
             vals = self._values.astype(np.int16)
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(object))
         elif typecode == NullableIntColumn.TYPE_CODE:
-            converted = NullableIntColumn(values=self._values.astype(np.object))
+            converted = NullableIntColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_long_column():
             converted = dataframe.DataFrame.NullableLongColumn(
-                values=self._values.astype(np.object))
+                values=self._values.astype(object))
 
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = bytearray(int(x).to_bytes(4, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
@@ -223,33 +223,33 @@
 
         Args:
             name: The name of the NullableIntColumn as a string
             values: The content of the NullableIntColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "int array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
@@ -336,15 +336,15 @@
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -373,98 +373,98 @@
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(int(x).to_bytes(4, byteorder="big", signed=True))
                 else:
                     vals[i] = bytearray(int(0).to_bytes(4, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == NullableIntColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int64(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray(int(x).to_bytes(4, byteorder="big", signed=True))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -473,8 +473,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/longcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/shortcolumn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-Provides an implementation for LongColumn and NullableLongColumn
+Provides an implementation for ShortColumn and NullableShortColumn
 """
 
 import numpy as np
 
 import raven.struct.dataframe.core as dataframe
 import raven.struct.dataframe.column as column
 import raven.struct.dataframe._columnutils as utils
 
-class LongColumn(column.Column):
-    """A Column holding long values (int64).
+class ShortColumn(column.Column):
+    """A Column holding short values (int16).
     This implementation DOES NOT support null values.
     """
 
-    TYPE_CODE = 4
+    TYPE_CODE = 2
 
     def __init__(self, name=None, values=None):
-        """Constructs a new LongColumn.
+        """Constructs a new ShortColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the LongColumn as a string
-            values: The content of the LongColumn.
-                Must be a list or numpy array with dtype int64, or an int
+            name: The name of the ShortColumn as a string
+            values: The content of the ShortColumn.
+                Must be a list or numpy array with dtype int16, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.int64)
+            values = np.empty(0, dtype=np.int16)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.int64)
+            values = np.array(values, dtype=np.int16)
 
         elif isinstance(values, np.ndarray):
-            if values.dtype != "int64":
+            if values.dtype != "int16":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "long array (int64) but found {}".format(values.dtype)))
+                     "short array (int16) but found {}".format(values.dtype)))
 
         elif isinstance(values, int):
-            values = np.zeros(values, dtype=np.int64)
+            values = np.zeros(values, dtype=np.int16)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
         if value is None:
             raise dataframe.DataFrameException(
                 ("Invalid argument. "
-                 "LongColumn cannot use None values"))
+                 "ShortColumn cannot use None values"))
 
         if isinstance(value, int):
-            if (value < -9223372036854775808) or (value > 9223372036854775807):
+            if (value < -32768) or (value > 32767):
                 raise dataframe.DataFrameException(
-                    "Out of range long (int64): {}".format(value))
+                    "Out of range short (int16): {}".format(value))
 
-        elif not isinstance(value, np.int64):
+        elif not isinstance(value, np.int16):
             raise dataframe.DataFrameException(
                 ("Invalid argument. Expected "
-                 "long (int64) but found {}".format(type(value))))
+                 "short (int16) but found {}".format(type(value))))
 
     def get_value(self, index):
-        """Gets the long value at the specified index
+        """Gets the short value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The long value at the specified index. Is never None
+            The short value at the specified index. Is never None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
         return int(self._values[index])
 
     def type_code(self):
-        return LongColumn.TYPE_CODE
+        return ShortColumn.TYPE_CODE
 
     def type_name(self):
-        return "long"
+        return "short"
 
     def is_nullable(self):
         return False
 
     def is_numeric(self):
         return True
 
@@ -117,22 +117,22 @@
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=invalid-name
     def convert_to(self, typecode):
         converted = None
         if typecode == utils.type_code_byte_column():
             converted = dataframe.DataFrame.ByteColumn(values=self._values.astype(np.int8))
-        elif typecode == utils.type_code_short_column():
-            converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
+        elif typecode == ShortColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
-        elif typecode == LongColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_long_column():
+            converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == utils.type_code_double_column():
@@ -140,157 +140,159 @@
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(bool))
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
-        elif typecode == utils.type_code_nullable_short_column():
-            vals = self._values.astype(np.int16)
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
+        elif typecode == NullableShortColumn.TYPE_CODE:
+            converted = NullableShortColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_int_column():
-            vals = self._values.astype(np.int32)
-            converted = dataframe.DataFrame.NullableIntColumn(values=vals.astype(np.object))
-        elif typecode == NullableLongColumn.TYPE_CODE:
-            converted = NullableLongColumn(values=self._values.astype(np.object))
+            converted = dataframe.DataFrame.NullableIntColumn(
+                values=self._values.astype(object))
+
+        elif typecode == utils.type_code_nullable_long_column():
+            converted = dataframe.DataFrame.NullableLongColumn(
+                values=self._values.astype(object))
+
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = ord(str(x)[0])
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
+            vals = self._values.astype(bool)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.zeros(size, dtype=np.int64)
+        return np.zeros(size, dtype=np.int16)
 
-class NullableLongColumn(column.Column):
-    """A Column holding nullable long values.
+class NullableShortColumn(column.Column):
+    """A Column holding nullable short values.
     Any values not explicitly set are considered None.
     """
 
-    TYPE_CODE = 13
+    TYPE_CODE = 11
 
     def __init__(self, name=None, values=None):
-        """Constructs a new NullableLongColumn.
+        """Constructs a new NullableShortColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the NullableLongColumn as a string
-            values: The content of the NullableLongColumn.
+            name: The name of the NullableShortColumn as a string
+            values: The content of the NullableShortColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "long array (object) but found {}".format(values.dtype)))
+                     "short array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
         if isinstance(value, int):
-            if (value < -9223372036854775808) or (value > 9223372036854775807):
+            if (value < -32768) or (value > 32767):
                 raise dataframe.DataFrameException(
-                    "Out of range long (int64): {}".format(value))
+                    "Out of range short (int16): {}".format(value))
 
-        elif value is not None and not isinstance(value, np.int64):
+        elif value is not None and not isinstance(value, np.int16):
             raise dataframe.DataFrameException(
                 ("Invalid argument. Expected "
-                 "long (int64) but found {}".format(type(value))))
+                 "short (int16) but found {}".format(type(value))))
 
     def get_value(self, index):
-        """Gets the long value at the specified index
+        """Gets the short value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The long value at the specified index. May be None
+            The short value at the specified index. May be None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
         val = self._values[index]
         if val is None:
             return None
         else:
             return int(val)
 
     def type_code(self):
-        return NullableLongColumn.TYPE_CODE
+        return NullableShortColumn.TYPE_CODE
 
     def type_name(self):
-        return "long"
+        return "short"
 
     def is_nullable(self):
         return True
 
     def is_numeric(self):
         return True
 
@@ -307,43 +309,43 @@
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int8(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.ByteColumn(values=vals)
-        elif typecode == utils.type_code_short_column():
+        elif typecode == ShortColumn.TYPE_CODE:
             vals = np.empty([self._values.shape[0]], dtype=np.int16)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int16(x))
                 else:
                     vals[i] = 0
 
-            converted = dataframe.DataFrame.ShortColumn(values=vals)
+            converted = ShortColumn(values=vals)
         elif typecode == utils.type_code_int_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int32)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int32(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.IntColumn(values=vals)
-        elif typecode == LongColumn.TYPE_CODE:
+        elif typecode == utils.type_code_long_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int64)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = 0
 
-            converted = LongColumn(values=vals)
+            converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
@@ -372,108 +374,108 @@
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
                 else:
-                    vals[i] = bytearray(int(0).to_bytes(8, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(0).to_bytes(2, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
-        elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
-            for i, x in np.ndenumerate(self._values):
-                vals[i] = int(np.int16(x)) if x is not None else None
-
-            converted = dataframe.DataFrame.NullableShortColumn(values=vals)
+        elif typecode == NullableShortColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
-        elif typecode == NullableLongColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_nullable_long_column():
+            vals = np.empty([self._values.shape[0]], dtype=object)
+            for i, x in np.ndenumerate(self._values):
+                vals[i] = int(np.int64(x)) if x is not None else None
+
+            converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(str(x)[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = (x != 0)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(8, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/shortcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/booleancolumn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,481 +1,484 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-Provides an implementation for ShortColumn and NullableShortColumn
+Provides an implementation for BooleanColumn and NullableBooleanColumn
 """
 
 import numpy as np
 
 import raven.struct.dataframe.core as dataframe
 import raven.struct.dataframe.column as column
 import raven.struct.dataframe._columnutils as utils
 
-class ShortColumn(column.Column):
-    """A Column holding short values (int16).
+class BooleanColumn(column.Column):
+    """A Column holding boolean values (bool).
     This implementation DOES NOT support null values.
     """
 
-    TYPE_CODE = 2
+    TYPE_CODE = 9
 
     def __init__(self, name=None, values=None):
-        """Constructs a new ShortColumn.
+        """Constructs a new BooleanColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the ShortColumn as a string
-            values: The content of the ShortColumn.
-                Must be a list or numpy array with dtype int16, or an int
+            name: The name of the BooleanColumn as a string
+            values: The content of the BooleanColumn.
+                Must be a list or numpy array with dtype bool, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.int16)
+            values = np.empty(0, dtype=bool)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.int16)
+            values = np.array(values, dtype=bool)
 
         elif isinstance(values, np.ndarray):
-            if values.dtype != "int16":
+            if values.dtype != "bool":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "short array (int16) but found {}".format(values.dtype)))
+                     "boolean array (bool) but found {}".format(values.dtype)))
 
         elif isinstance(values, int):
-            values = np.zeros(values, dtype=np.int16)
+            values = np.zeros(values, dtype=bool)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
         if value is None:
             raise dataframe.DataFrameException(
                 ("Invalid argument. "
-                 "ShortColumn cannot use None values"))
+                 "BooleanColumn cannot use None values"))
 
-        if isinstance(value, int):
-            if (value < -32768) or (value > 32767):
-                raise dataframe.DataFrameException(
-                    "Out of range short (int16): {}".format(value))
-
-        elif not isinstance(value, np.int16):
+        if not isinstance(value, (bool, np.bool_)):
             raise dataframe.DataFrameException(
                 ("Invalid argument. Expected "
-                 "short (int16) but found {}".format(type(value))))
+                 "boolean (bool) but found {}").format(type(value)))
 
     def get_value(self, index):
-        """Gets the short value at the specified index
+        """Gets the boolean value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The short value at the specified index. Is never None
+            The boolean value at the specified index. Is never None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
-        return int(self._values[index])
+        val = self._values[index]
+        return bool(val)
+
+    def set_value(self, index, value):
+        """Sets the boolean value at the specified index
+
+        Args:
+            index: The index of the boolean value to set
+            value: The boolean value to set at the specified position.
+                Must be a boolean
+
+        Raises:
+            ValueError: If the specified index is out of bounds or of the
+                object provided is of the wrong type
+        """
+        self._check_bounds(index)
+        self._check_type(value)
+        self._values[index] = value
 
     def type_code(self):
-        return ShortColumn.TYPE_CODE
+        return BooleanColumn.TYPE_CODE
 
     def type_name(self):
-        return "short"
+        return "boolean"
 
     def is_nullable(self):
         return False
 
     def is_numeric(self):
-        return True
+        return False
 
     def get_default_value(self):
-        return 0
+        return False
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=invalid-name
     def convert_to(self, typecode):
         converted = None
         if typecode == utils.type_code_byte_column():
             converted = dataframe.DataFrame.ByteColumn(values=self._values.astype(np.int8))
-        elif typecode == ShortColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_short_column():
+            converted = dataframe.DataFrame.ShortColumn(values=self._values.astype(np.int16))
         elif typecode == utils.type_code_int_column():
             converted = dataframe.DataFrame.IntColumn(values=self._values.astype(np.int32))
         elif typecode == utils.type_code_long_column():
             converted = dataframe.DataFrame.LongColumn(values=self._values.astype(np.int64))
         elif typecode == utils.type_code_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             converted = dataframe.DataFrame.FloatColumn(values=self._values.astype(np.float32))
         elif typecode == utils.type_code_double_column():
             converted = dataframe.DataFrame.DoubleColumn(values=self._values.astype(np.float64))
         elif typecode == utils.type_code_char_column():
             vals = self._values.astype(np.uint8)
             for i, x in np.ndenumerate(vals):
-                vals[i] = ord(str(x)[0])
+                if x:
+                    vals[i] = ord("1")
+                else:
+                    vals[i] = ord("0")
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
-        elif typecode == utils.type_code_boolean_column():
-            converted = dataframe.DataFrame.BooleanColumn(values=self._values.astype(np.bool))
+        elif typecode == BooleanColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
             vals = self._values.astype(np.int8)
-            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(np.object))
-        elif typecode == NullableShortColumn.TYPE_CODE:
-            converted = NullableShortColumn(values=self._values.astype(np.object))
+            converted = dataframe.DataFrame.NullableByteColumn(values=vals.astype(object))
+        elif typecode == utils.type_code_nullable_short_column():
+            vals = self._values.astype(np.int16)
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals.astype(object))
         elif typecode == utils.type_code_nullable_int_column():
-            converted = dataframe.DataFrame.NullableIntColumn(
-                values=self._values.astype(np.object))
-
+            vals = self._values.astype(np.int32)
+            converted = dataframe.DataFrame.NullableIntColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_long_column():
+            vals = self._values.astype(np.int64)
             converted = dataframe.DataFrame.NullableLongColumn(
-                values=self._values.astype(np.object))
+                values=self._values.astype(object))
 
         elif typecode == utils.type_code_nullable_string_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = str(x)
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
             vals = self._values.astype(np.float32)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
             vals = self._values.astype(np.float64)
-            vals = vals.astype(np.object)
+            vals = vals.astype(object)
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = self._values.astype(np.object)
+            vals = self._values.astype(np.uint8)
+            vals = vals.astype(object)
             for i, x in np.ndenumerate(vals):
-                vals[i] = ord(str(x)[0])
+                if x:
+                    vals[i] = ord("1")
+                else:
+                    vals[i] = ord("0")
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
-        elif typecode == utils.type_code_nullable_boolean_column():
-            vals = self._values.astype(np.bool)
-            vals = vals.astype(np.object)
-            converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
+        elif typecode == NullableBooleanColumn.TYPE_CODE:
+            converted = NullableBooleanColumn(values=self._values.astype(object))
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
+                vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.zeros(size, dtype=np.int16)
+        return np.zeros(size, dtype=bool)
 
-class NullableShortColumn(column.Column):
-    """A Column holding nullable short values.
+class NullableBooleanColumn(column.Column):
+    """A Column holding nullable boolean values.
     Any values not explicitly set are considered None.
     """
 
-    TYPE_CODE = 11
+    TYPE_CODE = 18
 
     def __init__(self, name=None, values=None):
-        """Constructs a new NullableShortColumn.
+        """Constructs a new NullableBooleanColumn.
 
         The constructed Column will have the specified name or is unlabeled
         if the specified name is None or empty.
         The constructed Column has the content of the specified list
         or numpy array. If the argument specifying the Column values is
         an int, then the constructed Column is initialized with the given
         length and all Column entries are set to default values.
 
         Args:
-            name: The name of the NullableShortColumn as a string
-            values: The content of the NullableShortColumn.
+            name: The name of the NullableBooleanColumn as a string
+            values: The content of the NullableBooleanColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
-                     "short array (object) but found {}".format(values.dtype)))
+                     "boolean array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
 
     def _check_type(self, value):
-        if isinstance(value, int):
-            if (value < -32768) or (value > 32767):
+        if value is not None:
+            if not isinstance(value, (bool, np.bool_)):
                 raise dataframe.DataFrameException(
-                    "Out of range short (int16): {}".format(value))
-
-        elif value is not None and not isinstance(value, np.int16):
-            raise dataframe.DataFrameException(
-                ("Invalid argument. Expected "
-                 "short (int16) but found {}".format(type(value))))
+                    ("Invalid argument. Expected "
+                     "boolean (bool) but found {}").format(type(value)))
 
     def get_value(self, index):
-        """Gets the short value at the specified index
+        """Gets the boolean value at the specified index
 
         Args:
             index: The index of the value to get
 
         Returns:
-            The short value at the specified index. May be None
+            The boolean value at the specified index. May be None
 
         Raises:
             ValueError: If the specified index is out of bounds
         """
         self._check_bounds(index)
         val = self._values[index]
         if val is None:
             return None
-        else:
-            return int(val)
+
+        return bool(val)
+
+    def set_value(self, index, value):
+        """Sets the boolean value at the specified index
+
+        Args:
+            index: The index of the boolean value to set
+            value: The boolean value to set at the specified position.
+                Must be a boolean or None
+
+        Raises:
+            ValueError: If the specified index is out of bounds or of the
+                object provided is of the wrong type
+        """
+        self._check_bounds(index)
+        self._check_type(value)
+        self._values[index] = value
 
     def type_code(self):
-        return NullableShortColumn.TYPE_CODE
+        return NullableBooleanColumn.TYPE_CODE
 
     def type_name(self):
-        return "short"
+        return "boolean"
 
     def is_nullable(self):
         return True
 
     def is_numeric(self):
-        return True
+        return False
 
     def get_default_value(self):
         return None
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=invalid-name
     def convert_to(self, typecode):
         converted = None
         if typecode == utils.type_code_byte_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int8)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = int(np.int8(x))
-                else:
-                    vals[i] = 0
+                vals[i] = int(x) if x is not None else 0
 
             converted = dataframe.DataFrame.ByteColumn(values=vals)
-        elif typecode == ShortColumn.TYPE_CODE:
+        elif typecode == utils.type_code_short_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int16)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = int(np.int16(x))
-                else:
-                    vals[i] = 0
+                vals[i] = int(x) if x is not None else 0
 
-            converted = ShortColumn(values=vals)
+            converted = dataframe.DataFrame.ShortColumn(values=vals)
         elif typecode == utils.type_code_int_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int32)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = int(np.int32(x))
-                else:
-                    vals[i] = 0
+                vals[i] = int(x) if x is not None else 0
 
             converted = dataframe.DataFrame.IntColumn(values=vals)
         elif typecode == utils.type_code_long_column():
             vals = np.empty([self._values.shape[0]], dtype=np.int64)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = int(np.int64(x))
-                else:
-                    vals[i] = 0
+                vals[i] = int(x) if x is not None else 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == utils.type_code_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = utils.default_value_string_column()
 
             converted = dataframe.DataFrame.StringColumn(values=vals)
         elif typecode == utils.type_code_float_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float32)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = float(x)
-                else:
-                    vals[i] = 0.0
+                vals[i] = float(x) if x is not None else 0.0
 
             converted = dataframe.DataFrame.FloatColumn(values=vals)
         elif typecode == utils.type_code_double_column():
             vals = np.empty([self._values.shape[0]], dtype=np.float64)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = float(x)
-                else:
-                    vals[i] = 0.0
+                vals[i] = float(x) if x is not None else 0.0
 
             converted = dataframe.DataFrame.DoubleColumn(values=vals)
         elif typecode == utils.type_code_char_column():
             vals = np.zeros([self._values.shape[0]], dtype=np.uint8)
-            ord_default = ord(utils.default_value_char_column())
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = ord(str(x)[0])
+                if x is not None and x is True:
+                    vals[i] = ord("1")
                 else:
-                    vals[i] = ord_default
+                    vals[i] = ord("0")
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
-        elif typecode == utils.type_code_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
-            for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = (x != 0)
+        elif typecode == BooleanColumn.TYPE_CODE:
+            vals = self._values.astype(bool)
+            for i, x in np.ndenumerate(vals):
+                if x is not None and x is True:
+                    vals[i] = True
                 else:
                     vals[i] = False
 
-            converted = dataframe.DataFrame.BooleanColumn(values=vals)
+            converted = BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
                 else:
-                    vals[i] = bytearray(int(0).to_bytes(2, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(0).to_bytes(1, byteorder="big", signed=True))
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(np.int8(x)) if x is not None else None
+                vals[i] = int(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
-        elif typecode == NullableShortColumn.TYPE_CODE:
-            converted = self.clone()
+        elif typecode == utils.type_code_nullable_short_column():
+            vals = np.empty([self._values.shape[0]], dtype=object)
+            for i, x in np.ndenumerate(self._values):
+                vals[i] = int(x) if x is not None else None
+
+            converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(np.int32(x)) if x is not None else None
+                vals[i] = int(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                vals[i] = int(np.int64(x)) if x is not None else None
+                vals[i] = int(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == utils.type_code_nullable_string_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
-            for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = str(x)
-                else:
-                    vals[i] = None
+            vals = self._values.astype(object)
+            for i, x in np.ndenumerate(vals):
+                vals[i] = str(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = float(x)
-                else:
-                    vals[i] = None
+                vals[i] = float(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = float(x)
-                else:
-                    vals[i] = None
+                vals[i] = float(x) if x is not None else None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
-            for i, x in np.ndenumerate(self._values):
+            vals = self._values.astype(object)
+            vals = vals.astype(object)
+            for i, x in np.ndenumerate(vals):
                 if x is not None:
-                    vals[i] = ord(str(x)[0])
+                    if x is True:
+                        vals[i] = ord("1")
+                    else:
+                        vals[i] = ord("0")
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
-        elif typecode == utils.type_code_nullable_boolean_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
-            for i, x in np.ndenumerate(self._values):
-                if x is not None:
-                    vals[i] = (x != 0)
-                else:
-                    vals[i] = None
-
-            converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
+        elif typecode == NullableBooleanColumn.TYPE_CODE:
+            converted = self.clone()
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
-                    vals[i] = bytearray(int(x).to_bytes(2, byteorder="big", signed=True))
+                    vals[i] = bytearray(int(x).to_bytes(1, byteorder="big", signed=True))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
         else:
             raise dataframe.DataFrameException(
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven/struct/dataframe/stringcolumn.py` & `raven-pydf-1.1.4/raven/struct/dataframe/stringcolumn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,23 +42,23 @@
 
         Args:
             name: The name of the StringColumn as a string
             values: The content of the StringColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for i, value in enumerate(values):
                 self._check_type(value)
                 if not value:
                     values[i] = StringColumn.DEFAULT_VALUE
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "string array (object) but found {}".format(values.dtype)))
 
@@ -68,15 +68,15 @@
                         ("Invalid element in argument array. Expected "
                          "string (str) but found {}".format(values.dtype)))
 
                 if not value:
                     values[i] = StringColumn.DEFAULT_VALUE
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
             for i in range(values.shape[0]):
                 values[i] = StringColumn.DEFAULT_VALUE
 
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
@@ -174,15 +174,15 @@
                 else:
                     vals[i] = utils.default_value_char_column()
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
             values_true = {"true", "t", "1", "yes", "y", "on"}
             values_false = {"false", "f", "0", "no", "n", "off"}
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     x = x.lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -190,95 +190,95 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray.fromhex(x)
                 else:
                     vals[i] = bytearray(b'\x00')
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int8(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int16(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int32(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == NullableStringColumn.TYPE_CODE:
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(vals):
                 vals[i] = x
 
             converted = NullableStringColumn(values=vals)
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(np.float32(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = float(np.float64(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = ord(x[0])
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
             values_true = {"true", "t", "1", "yes", "y", "on"}
             values_false = {"false", "f", "0", "no", "n", "off"}
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     x = x.lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -286,15 +286,15 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = bytearray.fromhex(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -303,15 +303,15 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
 
 class NullableStringColumn(column.Column):
     """A Column holding nullable string values.
     Any values not explicitly set are considered None.
     """
 
     TYPE_CODE = 14
@@ -328,33 +328,33 @@
 
         Args:
             name: The name of the NullableStringColumn as a string
             values: The content of the NullableStringColumn.
                 Must be a list or numpy array with dtype object, or an int
         """
         if values is None:
-            values = np.empty(0, dtype=np.object)
+            values = np.empty(0, dtype=object)
 
         if isinstance(values, list):
             for value in values:
                 self._check_type(value)
 
-            values = np.array(values, dtype=np.object)
+            values = np.array(values, dtype=object)
 
         elif isinstance(values, np.ndarray):
             if values.dtype != "object":
                 raise dataframe.DataFrameException(
                     ("Invalid argument array. Expected "
                      "string array (object) but found {}".format(values.dtype)))
 
             for value in values:
                 self._check_type(value)
 
         elif isinstance(values, int):
-            values = np.empty(values, dtype=np.object)
+            values = np.empty(values, dtype=object)
 
         else:
             raise dataframe.DataFrameException(
                 ("Invalid argument array. Expected "
                  "list or numpy array but found {}".format(type(values))))
 
         super().__init__(name, values)
@@ -418,15 +418,15 @@
                 if x is not None:
                     vals[i] = int(np.int64(x))
                 else:
                     vals[i] = 0
 
             converted = dataframe.DataFrame.LongColumn(values=vals)
         elif typecode == StringColumn.TYPE_CODE:
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x is not None:
                     vals[i] = str(x)
                 else:
                     vals[i] = StringColumn.DEFAULT_VALUE
 
             converted = StringColumn(values=vals)
@@ -457,15 +457,15 @@
                 else:
                     vals[i] = ord_default
 
             converted = dataframe.DataFrame.CharColumn(values=vals)
         elif typecode == utils.type_code_boolean_column():
             values_true = {"true", "t", "1", "yes", "y", "on"}
             values_false = {"false", "f", "0", "no", "n", "off"}
-            vals = np.empty([self._values.shape[0]], dtype=np.bool)
+            vals = np.empty([self._values.shape[0]], dtype=bool)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     x = x.lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -473,79 +473,79 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = False
 
             converted = dataframe.DataFrame.BooleanColumn(values=vals)
         elif typecode == utils.type_code_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     vals[i] = bytearray.fromhex(x)
                 else:
                     vals[i] = bytearray(b'\x00')
 
             converted = dataframe.DataFrame.BinaryColumn(values=vals)
         elif typecode == utils.type_code_nullable_byte_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int8(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableByteColumn(values=vals)
         elif typecode == utils.type_code_nullable_short_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int16(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableShortColumn(values=vals)
         elif typecode == utils.type_code_nullable_int_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int32(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableIntColumn(values=vals)
         elif typecode == utils.type_code_nullable_long_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 vals[i] = int(np.int64(x)) if x is not None else None
 
             converted = dataframe.DataFrame.NullableLongColumn(values=vals)
         elif typecode == NullableStringColumn.TYPE_CODE:
             converted = self.clone()
         elif typecode == utils.type_code_nullable_float_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     vals[i] = float(np.float32(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableFloatColumn(values=vals)
         elif typecode == utils.type_code_nullable_double_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     vals[i] = float(np.float64(x))
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableDoubleColumn(values=vals)
         elif typecode == utils.type_code_nullable_char_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     vals[i] = str(x)[0]
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableCharColumn(values=vals)
         elif typecode == utils.type_code_nullable_boolean_column():
             values_true = {"true", "t", "1", "yes", "y", "on"}
             values_false = {"false", "f", "0", "no", "n", "off"}
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     x = x.lower()
                     is_true = x in values_true
                     is_false = x in values_false
                     if not is_true and not is_false:
                         raise dataframe.DataFrameException(
@@ -553,15 +553,15 @@
 
                     vals[i] = is_true
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBooleanColumn(values=vals)
         elif typecode == utils.type_code_nullable_binary_column():
-            vals = np.empty([self._values.shape[0]], dtype=np.object)
+            vals = np.empty([self._values.shape[0]], dtype=object)
             for i, x in np.ndenumerate(self._values):
                 if x:
                     vals[i] = bytearray.fromhex(x)
                 else:
                     vals[i] = None
 
             converted = dataframe.DataFrame.NullableBinaryColumn(values=vals)
@@ -570,8 +570,8 @@
                 "Unknown column type code: {}".format(typecode))
 
         # pylint: disable=protected-access
         converted._name = self._name
         return converted
 
     def _create_array(self, size=0):
-        return np.empty(size, dtype=np.object)
+        return np.empty(size, dtype=object)
```

### Comparing `raven-pydf-1.1.3/raven_pydf.egg-info/PKG-INFO` & `raven-pydf-1.1.4/raven_pydf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-pydf
-Version: 1.1.3
+Version: 1.1.4
 Summary: An implementation of the DataFrame specification in Python
 Home-page: https://github.com/raven-computing/pydf
 Author: Phil Gaiser
 Author-email: phil.gaiser@raven-computing.com
 License: Apache Software License
 Description: This is the official implementation of the DataFrame specification provided by Raven Computing.
```

### Comparing `raven-pydf-1.1.3/raven_pydf.egg-info/SOURCES.txt` & `raven-pydf-1.1.4/raven_pydf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raven-pydf-1.1.3/setup.py` & `raven-pydf-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Raven Computing
+# Copyright (C) 2023 Raven Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +20,15 @@
 PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(PROJECT_ROOT, "pypi.md")) as f:
     README = f.read()
 
 setup(
     name="raven-pydf",
-    version="1.1.3",
+    version="1.1.4",
     description="An implementation of the DataFrame specification in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/raven-computing/pydf",
     author="Phil Gaiser",
     author_email="phil.gaiser@raven-computing.com",
     license="Apache Software License",
```

