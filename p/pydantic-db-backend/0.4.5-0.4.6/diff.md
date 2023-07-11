# Comparing `tmp/pydantic_db_backend-0.4.5.tar.gz` & `tmp/pydantic_db_backend-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.4.5.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.4.6.tar", max compression
```

## Comparing `pydantic_db_backend-0.4.5.tar` & `pydantic_db_backend-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.5/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.5/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6242 2023-07-11 07:48:12.508755 pydantic_db_backend-0.4.5/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     6594 2023-07-11 09:30:35.122968 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.5/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.5/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.5/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-11 11:13:08.181974 pydantic_db_backend-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.6/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6242 2023-07-11 07:48:12.508755 pydantic_db_backend-0.4.6/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     6703 2023-07-11 13:02:38.177598 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.6/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.6/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-11 13:06:46.348152 pydantic_db_backend-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.6/PKG-INFO
```

### Comparing `pydantic_db_backend-0.4.5/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.4.6/pydantic_db_backend/backend.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.5/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.4.6/pydantic_db_backend/backends/couchdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,26 +130,31 @@
             raise NotFound(uid=uid)
 
     @classmethod
     def get_uids(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
-        limit: int = 0,
+        limit: int = 25,
         query_filter: dict = None,
         sort: List = None
     ) -> List[str]:
+
+        # fix 0 limit, since couchdb does not know this
+        limit = 9999999 if limit == 0 else limit
+
         if query_filter is None:
             query_filter = {}
 
         # convert to json and back again, to have iso datetime strings
         query_filter = json.loads(json.dumps(query_filter, cls=CustomJSONEncoder))
 
         db = cls.get_db(model)
 
+
         find_dict = {
             "selector": query_filter,
             "skip": skip,
             "limit": limit,
             "fields": ['_id']
         }
         if sort is not None:
```

### Comparing `pydantic_db_backend-0.4.5/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.4.6/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.5/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.4.6/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.5/pyproject.toml` & `pydantic_db_backend-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.4.5"
+version = "0.4.6"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.4.5/PKG-INFO` & `pydantic_db_backend-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

