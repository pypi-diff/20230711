# Comparing `tmp/ohdsi-database-connector-0.2.0.tar.gz` & `tmp/ohdsi-database-connector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-database-connector-0.2.0.tar", last modified: Wed Jun 14 08:26:51 2023, max compression
+gzip compressed data, was "ohdsi-database-connector-0.2.1.tar", last modified: Tue Jul 11 14:30:34 2023, max compression
```

## Comparing `ohdsi-database-connector-0.2.0.tar` & `ohdsi-database-connector-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.501507 ohdsi-database-connector-0.2.0/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi/database_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/ohdsi/database_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/
--rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/postgresql-42.2.18.jar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/database_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/ohdsi/database_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/
+-rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/postgresql-42.2.18.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/setup.py
```

### Comparing `ohdsi-database-connector-0.2.0/PKG-INFO` & `ohdsi-database-connector-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-database-connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `ohdsi-database-connector-0.2.0/ohdsi/database_connector/__init__.py` & `ohdsi-database-connector-0.2.1/ohdsi/database_connector/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -122,8 +122,57 @@
         connection : RS4
             The database connection.
 
         Examples
         --------
         >>> Connect.disconnect(connection)
         """
-        database_connector_r.disconnect(connection)
+        database_connector_r.disconnect(connection)
+
+
+class Sql:
+
+    @staticmethod
+    def query_sql(connection: RS4, sql: str) -> RS4:
+        """
+        Query a database.
+
+        Parameters
+        ----------
+        connection : RS4
+            The database connection.
+        sql : str
+            The SQL query.
+
+        Returns
+        -------
+        RS4
+            The query result.
+
+        Examples
+        --------
+        >>> Sql.query_sql(connection, sql)
+        >>> Sql.query_sql(connection, "SELECT COUNT(*) FROM person")
+        """
+        return database_connector_r.querySql(connection, sql)
+
+    @staticmethod
+    def execute_sql(connection: RS4, sql: str) -> None:
+        """
+        Execute a SQL statement.
+
+        Parameters
+        ----------
+        connection : RS4
+            The database connection.
+        sql : str
+            The SQL statement.
+
+        Examples
+        --------
+        >>> Sql.execute_sql(connection, sql)
+        >>> Sql.execute_sql(connection, "DROP TABLE IF EXISTS person")
+        >>> Sql.execute_sql(
+        ...     conn, "CREATE TABLE x (k INT); CREATE TABLE y (k INT);"
+        ... )
+        """
+        database_connector_r.executeSql(connection, sql)
```

### Comparing `ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/postgresql-42.2.18.jar` & `ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/postgresql-42.2.18.jar`

 * *Files identical despite different names*

### Comparing `ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/PKG-INFO` & `ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-database-connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
```

### Comparing `ohdsi-database-connector-0.2.0/setup.py` & `ohdsi-database-connector-0.2.1/setup.py`

 * *Files identical despite different names*

