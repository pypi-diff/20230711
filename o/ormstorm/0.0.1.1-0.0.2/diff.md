# Comparing `tmp/ormstorm-0.0.1.1.tar.gz` & `tmp/ormstorm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormstorm-0.0.1.1.tar", last modified: Mon Jul 10 20:13:37 2023, max compression
+gzip compressed data, was "ormstorm-0.0.2.tar", last modified: Tue Jul 11 17:48:52 2023, max compression
```

## Comparing `ormstorm-0.0.1.1.tar` & `ormstorm-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 20:13:37.112773 ormstorm-0.0.1.1/
--rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstorm-0.0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2148 2023-07-10 20:13:37.112773 ormstorm-0.0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 20:13:37.092520 ormstorm-0.0.1.1/ormstorm/
--rw-rw-rw-   0        0        0     5563 2023-07-10 17:21:01.000000 ormstorm-0.0.1.1/ormstorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:13:37.112773 ormstorm-0.0.1.1/ormstorm/orm/
--rw-rw-rw-   0        0        0        0 2023-07-10 20:02:40.000000 ormstorm-0.0.1.1/ormstorm/orm/__init__.py
--rw-rw-rw-   0        0        0     2324 2023-07-10 13:13:31.000000 ormstorm-0.0.1.1/ormstorm/orm/column.py
--rw-rw-rw-   0        0        0      455 2023-07-10 13:15:35.000000 ormstorm-0.0.1.1/ormstorm/orm/constants.py
--rw-rw-rw-   0        0        0     2674 2023-07-10 13:26:33.000000 ormstorm-0.0.1.1/ormstorm/orm/table.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:13:37.110325 ormstorm-0.0.1.1/ormstorm.egg-info/
--rw-rw-rw-   0        0        0     2148 2023-07-10 20:13:37.000000 ormstorm-0.0.1.1/ormstorm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-10 20:13:37.000000 ormstorm-0.0.1.1/ormstorm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 20:13:37.000000 ormstorm-0.0.1.1/ormstorm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 20:13:37.000000 ormstorm-0.0.1.1/ormstorm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 20:13:37.112773 ormstorm-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-07-10 20:13:35.000000 ormstorm-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/
+-rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstorm-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3393 2023-07-11 17:48:52.612443 ormstorm-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.578669 ormstorm-0.0.2/ormstorm/
+-rw-rw-rw-   0        0        0     7431 2023-07-11 17:20:56.000000 ormstorm-0.0.2/ormstorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/ormstorm/orm/
+-rw-rw-rw-   0        0        0        0 2023-07-10 20:02:40.000000 ormstorm-0.0.2/ormstorm/orm/__init__.py
+-rw-rw-rw-   0        0        0     2480 2023-07-11 17:16:41.000000 ormstorm-0.0.2/ormstorm/orm/column.py
+-rw-rw-rw-   0        0        0      455 2023-07-10 13:15:35.000000 ormstorm-0.0.2/ormstorm/orm/constants.py
+-rw-rw-rw-   0        0        0       48 2023-07-11 13:35:28.000000 ormstorm-0.0.2/ormstorm/orm/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/ormstorm/orm/filters/
+-rw-rw-rw-   0        0        0       32 2023-07-11 17:16:41.000000 ormstorm-0.0.2/ormstorm/orm/filters/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-07-11 17:29:00.000000 ormstorm-0.0.2/ormstorm/orm/filters/magic.py
+-rw-rw-rw-   0        0        0     2674 2023-07-10 13:26:33.000000 ormstorm-0.0.2/ormstorm/orm/table.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.594805 ormstorm-0.0.2/ormstorm.egg-info/
+-rw-rw-rw-   0        0        0     3393 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:48:52.612443 ormstorm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-07-11 17:48:29.000000 ormstorm-0.0.2/setup.py
```

### Comparing `ormstorm-0.0.1.1/LICENSE.txt` & `ormstorm-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.1.1/ormstorm/orm/column.py` & `ormstorm-0.0.2/ormstorm/orm/column.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-class Column(object):
+from .filters import MagicFilter
+
+
+class Column(MagicFilter):
     def __init__(self, type: str, not_null: bool = False, default: object = None, autoincrement: bool = False,
                  unique: bool = False, primary_key: bool = False, check: str = None) -> None:
 
         """
         Standard class for creating a column object.
 
         :param type: Data type
@@ -10,14 +13,16 @@
         :param default: Sets the default value for the insert
         :param autoincrement: Causes a unique number to be generated automatically
         :param unique: Ensures that all values in a column are distinct
         :param primary_key: Uniquely identifies each entry in a table
         :param check: Used to limit the range of values that can be placed in a column
         """
 
+        super().__init__("")
+
         self.type = type
         self.options = self._serialize_options(
             not_null, default, autoincrement, unique, primary_key, check
         )
 
     @staticmethod
     def _serialize_options(not_null: bool = False, default: object = None, autoincrement: bool = False,
@@ -36,26 +41,28 @@
             options.append(f"DEFAULT {default}")
         if check:
             options.append(f"CHECK({check})")
 
         return " ".join(options)
 
 
-class ColumnType(object):
+class ColumnType(MagicFilter):
     def __init__(self, table: str, name: str, type: str, options: str = "") -> None:
 
         """
         System class used to store additional column values.
 
         :param table: Parent table name
         :param name: Column name
         :param type: Column type
         :param options: Column options
         """
 
+        super().__init__(f"{table}.{name}", parameters={"table": table})
+
         self.table = table
         self.name = name
         self.type = type
         self.options = options
 
     def serialize(self) -> str:
         """
```

### Comparing `ormstorm-0.0.1.1/ormstorm/orm/table.py` & `ormstorm-0.0.2/ormstorm/orm/table.py`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.1.1/setup.py` & `ormstorm-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.1.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Small library for easy work with databases."
 
 with open("READ ME.md", mode="r", encoding="utf-8") as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name="ormstorm",
```

