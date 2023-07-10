# Comparing `tmp/databricks_sql_connector-2.7.0.tar.gz` & `tmp/databricks_sql_connector-2.7.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.7.0.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.7.1.dev1.tar", max compression
```

## Comparing `databricks_sql_connector-2.7.0.tar` & `databricks_sql_connector-2.7.1.dev1.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     4732 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/README.md
--rw-r--r--   0        0        0     1588 2023-06-26 21:47:10.389497 databricks_sql_connector-2.7.0/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4421 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6192 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     3790 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9499 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     5949 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    37645 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    43174 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9761 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4821 2023-07-10 22:01:30.910556 databricks_sql_connector-2.7.1.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev1/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev1/README.md
+-rw-r--r--   0        0        0     1593 2023-07-10 22:04:02.434540 databricks_sql_connector-2.7.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev1/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-10 22:04:13.555138 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-26 20:08:27.727475 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-06-26 20:08:27.727986 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-06-26 20:08:27.728260 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9499 2023-06-26 20:08:27.728679 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     5949 2023-06-22 16:18:22.936813 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    37992 2023-07-10 15:14:36.220919 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     6547 2023-07-10 15:14:36.221186 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/download_manager.py
+-rw-r--r--   0        0        0     6374 2023-07-10 15:14:36.221386 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/downloader.py
+-rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-06-26 20:08:27.729586 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    40111 2023-07-10 15:14:36.221836 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/types.py
+-rw-r--r--   0        0        0    17993 2023-07-10 15:14:36.222244 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10562 2023-07-10 21:41:38.369013 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev1/PKG-INFO
```

### Comparing `databricks_sql_connector-2.7.0/CHANGELOG.md` & `databricks_sql_connector-2.7.1.dev1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Release History
 
 ## 2.7.x (Unreleased)
 
+- Fix: Revised SQLAlchemy dialect and examples for compatibility with SQLAlchemy==1.3.x
+
 ## 2.7.0 (2023-06-26)
 
 - Fix: connector raised exception when calling close() on a closed Thrift session
 - Improve e2e test development ergonomics
 - Redact logged thrift responses by default
 - Add support for OAuth on Databricks Azure
```

### Comparing `databricks_sql_connector-2.7.0/LICENSE` & `databricks_sql_connector-2.7.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/README.md` & `databricks_sql_connector-2.7.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/pyproject.toml` & `databricks_sql_connector-2.7.1.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.7.0"
+version = "2.7.1.dev1"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.7.0"
+__version__ = "2.7.1.dev1"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/client.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from databricks.sql.utils import ExecuteResponse, ParamEscaper, inject_parameters
 from databricks.sql.types import Row
 from databricks.sql.auth.auth import get_python_sql_connector_auth_provider
 from databricks.sql.experimental.oauth_persistence import OAuthPersistence
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_RESULT_BUFFER_SIZE_BYTES = 10485760
+DEFAULT_RESULT_BUFFER_SIZE_BYTES = 104857600
 DEFAULT_ARRAY_SIZE = 100000
 
 
 class Connection:
     def __init__(
         self,
         server_hostname: str,
@@ -149,14 +149,16 @@
         # (True by default)
         # _use_arrow_native_decimals
         # Databricks runtime will return native Arrow types for decimals instead of Arrow strings
         # (True by default)
         # _use_arrow_native_timestamps
         # Databricks runtime will return native Arrow types for timestamps instead of Arrow strings
         # (True by default)
+        # use_cloud_fetch
+        # Enable use of cloud fetch to extract large query results in parallel via cloud storage
 
         if access_token:
             access_token_kv = {"access_token": access_token}
             kwargs = {**kwargs, **access_token_kv}
 
         self.open = False
         self.host = server_hostname
@@ -185,14 +187,15 @@
             auth_provider,
             **kwargs,
         )
 
         self._session_handle = self.thrift_backend.open_session(
             session_configuration, catalog, schema
         )
+        self.use_cloud_fetch = kwargs.get("use_cloud_fetch", False)
         self.open = True
         logger.info("Successfully opened session " + str(self.get_session_id_hex()))
         self._cursors = []  # type: List[Cursor]
 
     def __enter__(self):
         return self
 
@@ -493,14 +496,15 @@
         execute_response = self.thrift_backend.execute_command(
             operation=operation,
             session_handle=self.connection._session_handle,
             max_rows=self.arraysize,
             max_bytes=self.buffer_size_bytes,
             lz4_compression=self.connection.lz4_compression,
             cursor=self,
+            use_cloud_fetch=self.connection.use_cloud_fetch,
         )
         self.active_result_set = ResultSet(
             self.connection,
             execute_response,
             self.thrift_backend,
             self.buffer_size_bytes,
             self.arraysize,
@@ -818,14 +822,15 @@
             row = self.fetchone()
             if row:
                 yield row
             else:
                 break
 
     def _fill_results_buffer(self):
+        # At initialization or if the server does not have cloud fetch result links available
         results, has_more_rows = self.thrift_backend.fetch_results(
             op_handle=self.command_id,
             max_rows=self.arraysize,
             max_bytes=self.buffer_size_bytes,
             expected_row_start_offset=self._next_row_index,
             lz4_compressed=self.lz4_compressed,
             arrow_schema_bytes=self._arrow_schema_bytes,
```

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/exc.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from decimal import Decimal
 import errno
 import logging
 import math
 import time
 import uuid
 import threading
-import lz4.frame
 from ssl import CERT_NONE, CERT_REQUIRED, create_default_context
 from typing import List, Union
 
 import pyarrow
 import thrift.transport.THttpClient
 import thrift.protocol.TBinaryProtocol
 import thrift.transport.TSocket
@@ -22,19 +21,22 @@
 from databricks.sql.thrift_api.TCLIService import TCLIService, ttypes
 from databricks.sql import *
 from databricks.sql.thrift_api.TCLIService.TCLIService import (
     Client as TCLIServiceClient,
 )
 
 from databricks.sql.utils import (
-    ArrowQueue,
     ExecuteResponse,
     _bound,
     RequestErrorInfo,
     NoRetryReason,
+    ResultSetQueueFactory,
+    convert_arrow_based_set_to_arrow_table,
+    convert_decimals_in_arrow_table,
+    convert_column_based_set_to_arrow_table,
 )
 
 logger = logging.getLogger(__name__)
 
 unsafe_logger = logging.getLogger("databricks.sql.unsafe")
 unsafe_logger.setLevel(logging.DEBUG)
 
@@ -63,15 +65,14 @@
     "_retry_delay_default": (float, 5, 1, 60),
 }
 
 
 class ThriftBackend:
     CLOSED_OP_STATE = ttypes.TOperationState.CLOSED_STATE
     ERROR_OP_STATE = ttypes.TOperationState.ERROR_STATE
-    BIT_MASKS = [1, 2, 4, 8, 16, 32, 64, 128]
 
     def __init__(
         self,
         server_hostname: str,
         port,
         http_path: str,
         http_headers,
@@ -111,14 +112,16 @@
         #   _retry_stop_after_attempts_duration, stop now.)
         #
         # _retry_stop_after_attempts_count
         #  The maximum number of times we should retry retryable requests (defaults to 24)
         # _socket_timeout
         #  The timeout in seconds for socket send, recv and connect operations. Should be a positive float or integer.
         #  (defaults to 900)
+        # max_download_threads
+        #  Number of threads for handling cloud fetch downloads. Defaults to 10
 
         port = port or 443
         if kwargs.get("_connection_uri"):
             uri = kwargs.get("_connection_uri")
         elif server_hostname and http_path:
             uri = "https://{host}:{port}/{path}".format(
                 host=server_hostname, port=port, path=http_path.lstrip("/")
@@ -132,14 +135,17 @@
             "_use_arrow_native_complex_types", True
         )
         self._use_arrow_native_decimals = kwargs.get("_use_arrow_native_decimals", True)
         self._use_arrow_native_timestamps = kwargs.get(
             "_use_arrow_native_timestamps", True
         )
 
+        # Cloud fetch
+        self.max_download_threads = kwargs.get("max_download_threads", 10)
+
         # Configure tls context
         ssl_context = create_default_context(cafile=kwargs.get("_tls_trusted_ca_file"))
         if kwargs.get("_tls_no_verify") is True:
             ssl_context.check_hostname = False
             ssl_context.verify_mode = CERT_NONE
         elif kwargs.get("_tls_verify_hostname") is False:
             ssl_context.check_hostname = False
@@ -554,116 +560,22 @@
         return self.make_request(self._client.GetOperationStatus, req)
 
     def _create_arrow_table(self, t_row_set, lz4_compressed, schema_bytes, description):
         if t_row_set.columns is not None:
             (
                 arrow_table,
                 num_rows,
-            ) = ThriftBackend._convert_column_based_set_to_arrow_table(
-                t_row_set.columns, description
-            )
+            ) = convert_column_based_set_to_arrow_table(t_row_set.columns, description)
         elif t_row_set.arrowBatches is not None:
-            (
-                arrow_table,
-                num_rows,
-            ) = ThriftBackend._convert_arrow_based_set_to_arrow_table(
+            (arrow_table, num_rows,) = convert_arrow_based_set_to_arrow_table(
                 t_row_set.arrowBatches, lz4_compressed, schema_bytes
             )
         else:
             raise OperationalError("Unsupported TRowSet instance {}".format(t_row_set))
-        return self._convert_decimals_in_arrow_table(arrow_table, description), num_rows
-
-    @staticmethod
-    def _convert_decimals_in_arrow_table(table, description):
-        for (i, col) in enumerate(table.itercolumns()):
-            if description[i][1] == "decimal":
-                decimal_col = col.to_pandas().apply(
-                    lambda v: v if v is None else Decimal(v)
-                )
-                precision, scale = description[i][4], description[i][5]
-                assert scale is not None
-                assert precision is not None
-                # Spark limits decimal to a maximum scale of 38,
-                # so 128 is guaranteed to be big enough
-                dtype = pyarrow.decimal128(precision, scale)
-                col_data = pyarrow.array(decimal_col, type=dtype)
-                field = table.field(i).with_type(dtype)
-                table = table.set_column(i, field, col_data)
-        return table
-
-    @staticmethod
-    def _convert_arrow_based_set_to_arrow_table(
-        arrow_batches, lz4_compressed, schema_bytes
-    ):
-        ba = bytearray()
-        ba += schema_bytes
-        n_rows = 0
-        if lz4_compressed:
-            for arrow_batch in arrow_batches:
-                n_rows += arrow_batch.rowCount
-                ba += lz4.frame.decompress(arrow_batch.batch)
-        else:
-            for arrow_batch in arrow_batches:
-                n_rows += arrow_batch.rowCount
-                ba += arrow_batch.batch
-        arrow_table = pyarrow.ipc.open_stream(ba).read_all()
-        return arrow_table, n_rows
-
-    @staticmethod
-    def _convert_column_based_set_to_arrow_table(columns, description):
-        arrow_table = pyarrow.Table.from_arrays(
-            [ThriftBackend._convert_column_to_arrow_array(c) for c in columns],
-            # Only use the column names from the schema, the types are determined by the
-            # physical types used in column based set, as they can differ from the
-            # mapping used in _hive_schema_to_arrow_schema.
-            names=[c[0] for c in description],
-        )
-        return arrow_table, arrow_table.num_rows
-
-    @staticmethod
-    def _convert_column_to_arrow_array(t_col):
-        """
-        Return a pyarrow array from the values in a TColumn instance.
-        Note that ColumnBasedSet has no native support for complex types, so they will be converted
-        to strings server-side.
-        """
-        field_name_to_arrow_type = {
-            "boolVal": pyarrow.bool_(),
-            "byteVal": pyarrow.int8(),
-            "i16Val": pyarrow.int16(),
-            "i32Val": pyarrow.int32(),
-            "i64Val": pyarrow.int64(),
-            "doubleVal": pyarrow.float64(),
-            "stringVal": pyarrow.string(),
-            "binaryVal": pyarrow.binary(),
-        }
-        for field in field_name_to_arrow_type.keys():
-            wrapper = getattr(t_col, field)
-            if wrapper:
-                return ThriftBackend._create_arrow_array(
-                    wrapper, field_name_to_arrow_type[field]
-                )
-
-        raise OperationalError("Empty TColumn instance {}".format(t_col))
-
-    @staticmethod
-    def _create_arrow_array(t_col_value_wrapper, arrow_type):
-        result = t_col_value_wrapper.values
-        nulls = t_col_value_wrapper.nulls  # bitfield describing which values are null
-        assert isinstance(nulls, bytes)
-
-        # The number of bits in nulls can be both larger or smaller than the number of
-        # elements in result, so take the minimum of both to iterate over.
-        length = min(len(result), len(nulls) * 8)
-
-        for i in range(length):
-            if nulls[i >> 3] & ThriftBackend.BIT_MASKS[i & 0x7]:
-                result[i] = None
-
-        return pyarrow.array(result, type=arrow_type)
+        return convert_decimals_in_arrow_table(arrow_table, description), num_rows
 
     def _get_metadata_resp(self, op_handle):
         req = ttypes.TGetResultSetMetadataReq(operationHandle=op_handle)
         return self.make_request(self._client.GetResultSetMetadata, req)
 
     @staticmethod
     def _hive_schema_to_arrow_schema(t_table_schema):
@@ -748,14 +660,15 @@
             t_result_set_metadata_resp = resp.directResults.resultSetMetadata
         else:
             t_result_set_metadata_resp = self._get_metadata_resp(resp.operationHandle)
 
         if t_result_set_metadata_resp.resultFormat not in [
             ttypes.TSparkRowSetType.ARROW_BASED_SET,
             ttypes.TSparkRowSetType.COLUMN_BASED_SET,
+            ttypes.TSparkRowSetType.URL_BASED_SET,
         ]:
             raise OperationalError(
                 "Expected results to be in Arrow or column based format, "
                 "instead they are: {}".format(
                     ttypes.TSparkRowSetType._VALUES_TO_NAMES[
                         t_result_set_metadata_resp.resultFormat
                     ]
@@ -779,21 +692,22 @@
         )
         lz4_compressed = t_result_set_metadata_resp.lz4Compressed
         is_staging_operation = t_result_set_metadata_resp.isStagingOperation
         if direct_results and direct_results.resultSet:
             assert direct_results.resultSet.results.startRowOffset == 0
             assert direct_results.resultSetMetadata
 
-            arrow_results, n_rows = self._create_arrow_table(
-                direct_results.resultSet.results,
-                lz4_compressed,
-                schema_bytes,
-                description,
+            arrow_queue_opt = ResultSetQueueFactory.build_queue(
+                row_set_type=t_result_set_metadata_resp.resultFormat,
+                t_row_set=direct_results.resultSet.results,
+                arrow_schema_bytes=schema_bytes,
+                max_download_threads=self.max_download_threads,
+                lz4_compressed=lz4_compressed,
+                description=description,
             )
-            arrow_queue_opt = ArrowQueue(arrow_results, n_rows, 0)
         else:
             arrow_queue_opt = None
         return ExecuteResponse(
             arrow_queue=arrow_queue_opt,
             status=operation_state,
             has_been_closed_server_side=has_been_closed_server_side,
             has_more_rows=has_more_rows,
@@ -839,15 +753,22 @@
                 )
             if t_spark_direct_results.closeOperation:
                 ThriftBackend._check_response_for_error(
                     t_spark_direct_results.closeOperation
                 )
 
     def execute_command(
-        self, operation, session_handle, max_rows, max_bytes, lz4_compression, cursor
+        self,
+        operation,
+        session_handle,
+        max_rows,
+        max_bytes,
+        lz4_compression,
+        cursor,
+        use_cloud_fetch=False,
     ):
         assert session_handle is not None
 
         spark_arrow_types = ttypes.TSparkArrowTypes(
             timestampAsArrow=self._use_arrow_native_timestamps,
             decimalAsArrow=self._use_arrow_native_decimals,
             complexTypesAsArrow=self._use_arrow_native_complex_types,
@@ -860,15 +781,15 @@
             statement=operation,
             runAsync=True,
             getDirectResults=ttypes.TSparkGetDirectResults(
                 maxRows=max_rows, maxBytes=max_bytes
             ),
             canReadArrowResult=True,
             canDecompressLZ4Result=lz4_compression,
-            canDownloadResult=False,
+            canDownloadResult=use_cloud_fetch,
             confOverlay={
                 # We want to receive proper Timestamp arrow types.
                 "spark.thriftserver.arrowBasedRowSet.timestampAsString": "false"
             },
             useArrowNativeTypes=spark_arrow_types,
         )
         resp = self.make_request(self._client.ExecuteStatement, req)
@@ -989,29 +910,35 @@
                 op_handle.operationType,
                 False,
                 op_handle.modifiedRowCount,
             ),
             maxRows=max_rows,
             maxBytes=max_bytes,
             orientation=ttypes.TFetchOrientation.FETCH_NEXT,
+            includeResultSetMetadata=True,
         )
 
         resp = self.make_request(self._client.FetchResults, req)
         if resp.results.startRowOffset > expected_row_start_offset:
             logger.warning(
                 "Expected results to start from {} but they instead start at {}".format(
                     expected_row_start_offset, resp.results.startRowOffset
                 )
             )
-        arrow_results, n_rows = self._create_arrow_table(
-            resp.results, lz4_compressed, arrow_schema_bytes, description
+
+        queue = ResultSetQueueFactory.build_queue(
+            row_set_type=resp.resultSetMetadata.resultFormat,
+            t_row_set=resp.results,
+            arrow_schema_bytes=arrow_schema_bytes,
+            max_download_threads=self.max_download_threads,
+            lz4_compressed=lz4_compressed,
+            description=description,
         )
-        arrow_queue = ArrowQueue(arrow_results, n_rows)
 
-        return arrow_queue, resp.hasMoreRows
+        return queue, resp.hasMoreRows
 
     def close_command(self, op_handle):
         req = ttypes.TCloseOperationReq(operationHandle=op_handle)
         resp = self.make_request(self._client.CloseOperation, req)
         return resp.status
 
     def cancel_command(self, active_op_handle):
```

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sql/types.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module's layout loosely follows example of SQLAlchemy's postgres dialect
 """
 
 import decimal, re, datetime
 from dateutil.parser import parse
 
+import sqlalchemy
 from sqlalchemy import types, processors, event
 from sqlalchemy.engine import default, Engine
-from sqlalchemy.exc import DatabaseError
+from sqlalchemy.exc import DatabaseError, SQLAlchemyError
 from sqlalchemy.engine import reflection
 
 from databricks import sql
 
 
 from databricks.sqlalchemy.dialect.base import (
     DatabricksDDLCompiler,
@@ -149,17 +150,15 @@
             "struct": types.String,
             "uniontype": types.String,
             "decimal": DatabricksDecimal,
             "timestamp": DatabricksTimestamp,
             "date": DatabricksDate,
         }
 
-        with self.get_driver_connection(
-            connection
-        )._dbapi_connection.dbapi_connection.cursor() as cur:
+        with self.get_connection_cursor(connection) as cur:
             resp = cur.columns(
                 catalog_name=self.catalog,
                 schema_name=schema or self.schema,
                 table_name=table_name,
             ).fetchall()
 
         columns = []
@@ -240,30 +239,26 @@
           boolean
         """
         # TODO: Implement this behaviour
         return []
 
     def get_table_names(self, connection, schema=None, **kwargs):
         TABLE_NAME = 1
-        with self.get_driver_connection(
-            connection
-        )._dbapi_connection.dbapi_connection.cursor() as cur:
+        with self.get_connection_cursor(connection) as cur:
             sql_str = "SHOW TABLES FROM {}".format(
                 ".".join([self.catalog, schema or self.schema])
             )
             data = cur.execute(sql_str).fetchall()
             _tables = [i[TABLE_NAME] for i in data]
 
         return _tables
 
     def get_view_names(self, connection, schema=None, **kwargs):
         VIEW_NAME = 1
-        with self.get_driver_connection(
-            connection
-        )._dbapi_connection.dbapi_connection.cursor() as cur:
+        with self.get_connection_cursor(connection) as cur:
             sql_str = "SHOW VIEWS FROM {}".format(
                 ".".join([self.catalog, schema or self.schema])
             )
             data = cur.execute(sql_str).fetchall()
             _tables = [i[VIEW_NAME] for i in data]
 
         return _tables
@@ -288,14 +283,27 @@
             if DBR_GT_12_NOT_FOUND_STRING in str(
                 e
             ) or DBR_LTE_12_NOT_FOUND_STRING in str(e):
                 return False
             else:
                 raise e
 
+    def get_connection_cursor(self, connection):
+        """Added for backwards compatibility with 1.3.x"""
+        if hasattr(connection, "_dbapi_connection"):
+            return connection._dbapi_connection.dbapi_connection.cursor()
+        elif hasattr(connection, "raw_connection"):
+            return connection.raw_connection().cursor()
+        elif hasattr(connection, "connection"):
+            return connection.connection.cursor()
+
+        raise SQLAlchemyError(
+            "Databricks dialect can't obtain a cursor context manager from the dbapi"
+        )
+
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         # Equivalent to SHOW DATABASES
 
         # TODO: replace with call to cursor.schemas() once its performance matches raw SQL
         return [row[0] for row in connection.execute("SHOW SCHEMAS")]
 
@@ -310,7 +318,17 @@
 
     if "_user_agent_entry" in cparams:
         new_user_agent = f"sqlalchemy + {cparams['_user_agent_entry']}"
     else:
         new_user_agent = "sqlalchemy"
 
     cparams["_user_agent_entry"] = new_user_agent
+
+    if sqlalchemy.__version__.startswith("1.3"):
+        # SQLAlchemy 1.3.x fails to parse the http_path, catalog, and schema from our connection string
+        # These should be passed in as connect_args when building the Engine
+
+        if "schema" in cparams:
+            dialect.schema = cparams["schema"]
+
+        if "catalog" in cparams:
+            dialect.catalog = cparams["catalog"]
```

### Comparing `databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.0/PKG-INFO` & `databricks_sql_connector-2.7.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.7.0
+Version: 2.7.1.dev1
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

