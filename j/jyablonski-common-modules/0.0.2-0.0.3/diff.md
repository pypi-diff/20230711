# Comparing `tmp/jyablonski_common_modules-0.0.2.tar.gz` & `tmp/jyablonski_common_modules-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyablonski_common_modules-0.0.2.tar", max compression
+gzip compressed data, was "jyablonski_common_modules-0.0.3.tar", max compression
```

## Comparing `jyablonski_common_modules-0.0.2.tar` & `jyablonski_common_modules-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/__init__.py
--rw-r--r--   0        0        0      276 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/__init__.py
--rw-r--r--   0        0        0       49 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/exceptions.py
--rw-r--r--   0        0        0      887 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/s3.py
--rw-r--r--   0        0        0      560 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/secrets_manager.py
--rw-r--r--   0        0        0      784 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/ssm.py
--rw-r--r--   0        0        0      218 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/__init__.py
--rw-r--r--   0        0        0      465 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/core.py
--rw-r--r--   0        0        0      542 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/feature_flags.py
--rw-r--r--   0        0        0       22 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/logger.py
--rw-r--r--   0        0        0      146 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/__init__.py
--rw-r--r--   0        0        0     1152 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/connection.py
--rw-r--r--   0        0        0     5352 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/writers.py
--rw-r--r--   0        0        0      775 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 jyablonski_common_modules-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/exceptions.py
+-rw-r--r--   0        0        0      825 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/s3.py
+-rw-r--r--   0        0        0      560 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/secrets_manager.py
+-rw-r--r--   0        0        0      784 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/ssm.py
+-rw-r--r--   0        0        0      218 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/general/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/general/core.py
+-rw-r--r--   0        0        0      542 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/general/feature_flags.py
+-rw-r--r--   0        0        0      145 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/logging/__init__.py
+-rw-r--r--   0        0        0      456 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/logging/base_logger.py
+-rw-r--r--   0        0        0     1053 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/logging/os_logger.py
+-rw-r--r--   0        0        0      146 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/sql/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/sql/connection.py
+-rw-r--r--   0        0        0     5403 2023-07-11 00:02:12.373262 jyablonski_common_modules-0.0.3/jyablonski_common_modules/sql/writers.py
+-rw-r--r--   0        0        0      847 2023-07-11 00:02:12.377262 jyablonski_common_modules-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 jyablonski_common_modules-0.0.3/PKG-INFO
```

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/s3.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import botocore
 
-try:
-    from .exceptions import S3PrefixCheckFail
-except:
-    from exceptions import S3PrefixCheckFail
+from .exceptions import S3PrefixCheckFail
 
 
 def check_s3_file_exists(client: botocore.client, bucket: str, file_prefix: str):
     """
     Function to check if a file exists in an S3 Bucket.
 
     Args:
```

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/secrets_manager.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/ssm.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/feature_flags.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/general/feature_flags.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/logger.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/logging/os_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import logging
 
 from opensearch_logger import OpenSearchHandler
 
 
-def create_logger(es_index: str, es_host_endpoint: str):
+def create_os_logger(index: str, host_endpoint: str):
     """
     Logger which writes to both STDOUT as well as an Opensearch Endpoint
 
     Args:
         es_index (str): The name of the Opensearch Index that logs will go to.
             It will be automatically created if it doesn't already exist.
 
-        es_endpoint (str): The Endpoint of the Opensearch Cluster
+        host_endpoint (str): The Endpoint of the Opensearch Cluster
+
+    Returns:
+        Opensearch Logger
     """
     logging.basicConfig(
         level=logging.INFO,
         format="[%(levelname)s] %(asctime)s %(message)s",
         datefmt="%Y-%m-%d %I:%M:%S %p",
     )
     handler = OpenSearchHandler(
-        index_name=es_index,
-        hosts=[f"{es_host_endpoint}:443"],
+        index_name=index,
+        hosts=[f"{host_endpoint}:443"],
         # http_auth=("admin", "admin"),
         http_compress=True,
         use_ssl=False,
         verify_certs=False,
         ssl_assert_hostname=False,
         ssl_show_warn=False,
     )
```

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/connection.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/sql/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import exc, create_engine
+from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 
 
 def sql_connection(
     database: str,
     schema: str,
     user: str,
@@ -10,28 +10,32 @@
     host: str,
 ) -> Engine:
     """
     SQL Engine function to define the SQL Driver + connection variables needed to connect to the DB.
     This doesn't actually make the connection, use conn.connect() in a context manager to create 1 re-usable connection
 
     Args:
-        rds_schema (str): The Schema in the DB to connect to.
+        database(str): The Database to connect to
+
+        schema (str): The Schema to connect to
+
+        user (str): The User for the connection
+
+        pw (str): The Password for the connection
+
+        host (str): The Host Endpoint of the Database
 
     Returns:
         SQL Engine variable to a specified schema in my PostgreSQL DB
     """
-    try:
-        connection = create_engine(
-            f"postgresql+psycopg2://{user}:{pw}@{host}:5432/{database}",
-            # pool_size=0,
-            # max_overflow=20,
-            connect_args={
-                "options": f"-csearch_path={schema}",
-            },
-            # defining schema to connect to
-            echo=False,
-        )
-        print(f"SQL Engine for schema: {schema} Successful")
-        return connection
-    except exc.SQLAlchemyError as e:
-        print(f"SQL Engine for schema: {schema} Failed, Error: {e}")
-        return e
+    connection = create_engine(
+        f"postgresql+psycopg2://{user}:{pw}@{host}:5432/{database}",
+        # pool_size=0,
+        # max_overflow=20,
+        connect_args={
+            "options": f"-csearch_path={schema}",
+        },
+        # defining schema to connect to
+        echo=False,
+    )
+    print(f"SQL Engine for schema: {schema} Successful")
+    return connection
```

### Comparing `jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/writers.py` & `jyablonski_common_modules-0.0.3/jyablonski_common_modules/sql/writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
                 con=con,
                 name=f"{table}",
                 index=False,
                 if_exists=table_type,
             )
             print(f"Writing {len(df)} {table} rows to {table} to SQL")
     except BaseException as error:
-        print(f"SQL Write Script Failed, {error}")
+        print(f"SQL Write Script Failed while writing to {table}, {error}")
+        raise error
 
 
 def write_to_sql_upsert(
     conn,
     table: str,
     schema: str,
     df: pd.DataFrame,
@@ -69,15 +70,15 @@
 
     Returns:
         Upserts any new data in the Pandas DataFrame to the table in Postgres in the provided schema
 
     """
     sql_table_name = f"{table}"
     if len(df) == 0:
-        print(f"{sql_table_name} is empty, not storing to SQL")
+        print(f"{sql_table_name} is empty, not writing to SQL")
         pass
 
     else:
         # 2 try except blocks bc in event of an error there needs to be different logic to safely exit out and continue script
         try:
             df = df.set_index(pd_index)
             df = df.rename_axis(pd_index)
@@ -136,10 +137,10 @@
                 print(
                     f"SQL Upsert Function Successful, {len(df)} records added or upserted into {table}"
                 )
                 pass
             except BaseException as error:
                 conn.execute(f"DROP TABLE {temp_table_name};")
                 print(
-                    f"SQL Upsert Function Failed for EXISTING {table} ({len(df)} rows), {error}"
+                    f"SQL Upsert Function Failed for EXISTING TABLE {table} ({len(df)} rows), {error}"
                 )
                 pass
```

### Comparing `jyablonski_common_modules-0.0.2/PKG-INFO` & `jyablonski_common_modules-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyablonski-common-modules
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: jyablonski9
 Author-email: jyablonski9@gmail.com
 Maintainer: jyablonski9
 Maintainer-email: jyablonski9@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

