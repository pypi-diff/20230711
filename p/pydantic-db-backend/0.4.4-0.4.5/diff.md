# Comparing `tmp/pydantic_db_backend-0.4.4.tar.gz` & `tmp/pydantic_db_backend-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.4.4.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.4.5.tar", max compression
```

## Comparing `pydantic_db_backend-0.4.4.tar` & `pydantic_db_backend-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.4/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.4/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6182 2023-07-05 12:04:36.107157 pydantic_db_backend-0.4.4/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     6047 2023-06-28 09:24:42.810581 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.4/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.4/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-05 12:05:58.214172 pydantic_db_backend-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.5/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6242 2023-07-11 07:48:12.508755 pydantic_db_backend-0.4.5/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     6594 2023-07-11 09:30:35.122968 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.5/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.5/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-11 11:13:08.181974 pydantic_db_backend-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.5/PKG-INFO
```

### Comparing `pydantic_db_backend-0.4.4/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.4.5/pydantic_db_backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
     def collection_name(cls, model: Type[BaseModel]) -> str:
         if model not in cls._collections:
             name = re.sub('([A-Z]+)', r'_\1', model.__name__).lower().removeprefix("_").removesuffix("_model")
             cls._collections[model] = name
         return cls._collections[model]
 
     @classmethod
-    def indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None) -> str:
-        if model not in cls._indexes:
+    def indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None, force_index_creation: bool = False) -> str:
+        if model not in cls._indexes or force_index_creation:
             index = cls.create_indexes(model, create_index_kwargs)
             cls._indexes[model] = index
         return cls._indexes[model]
 
     @classmethod
     def create_indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None):
```

### Comparing `pydantic_db_backend-0.4.4/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.4.5/pydantic_db_backend/backends/couchdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import logging
 import os
 from typing import Dict, Type, List
 
 import pydash
-from couchdb import ResourceConflict
+from couchdb import ResourceConflict, ServerError
 from pydantic import BaseModel, Field
 
 import couchdb
 from pydantic_db_backend.backend import BackendBase, BackendModel
 from pydantic_db_backend.exceptions import RevisionConflict, NotFound, AlreadyExists
 from pydantic_db_backend.utils import CustomJSONEncoder
 
@@ -145,20 +145,35 @@
         query_filter = json.loads(json.dumps(query_filter, cls=CustomJSONEncoder))
 
         db = cls.get_db(model)
 
         find_dict = {
             "selector": query_filter,
             "skip": skip,
-            "limit": limit
+            "limit": limit,
+            "fields": ['_id']
         }
         if sort is not None:
             find_dict["sort"] = sort
 
-        result = [x["_id"] for x in (db.find(find_dict))]
+        try:
+            find_result = db.find(find_dict)
+        except ServerError as e:
+
+            error_code = pydash.get(e, ["args", 0, 0])
+
+            if error_code == 400:
+                # @asc:  not what I expected the system to do. Better would be to modify the
+                # index cache and initiate a new get_db... and a loop
+                cls.indexes(model, dict(db=db), force_index_creation=True)
+                find_result = db.find(find_dict)
+            else:
+                raise e
+
+        result = [x["_id"] for x in find_result]
         return result
 
     @classmethod
     def get_instances(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
```

### Comparing `pydantic_db_backend-0.4.4/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.4.5/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.4/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.4.5/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.4/pyproject.toml` & `pydantic_db_backend-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.4.4/PKG-INFO` & `pydantic_db_backend-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

