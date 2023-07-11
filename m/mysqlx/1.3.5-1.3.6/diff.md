# Comparing `tmp/mysqlx-1.3.5.tar.gz` & `tmp/mysqlx-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.5.tar", last modified: Mon Jul 10 14:24:14 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.6.tar", last modified: Tue Jul 11 03:21:13 2023, max compression
```

## Comparing `mysqlx-1.3.5.tar` & `mysqlx-1.3.6.tar`

### file list

```diff
@@ -1,37 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx/
--rw-rw-rw-   0        0        0     5819 2023-07-09 01:30:37.000000 mysqlx-1.3.5/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1644 2023-07-10 14:22:09.000000 mysqlx-1.3.5/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    19721 2023-07-10 13:35:46.000000 mysqlx-1.3.5/mysqlx/db.py
--rw-rw-rw-   0        0        0    13187 2023-07-09 01:26:49.000000 mysqlx-1.3.5/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    39144 2023-07-10 14:13:27.000000 mysqlx-1.3.5/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.5/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4052 2023-07-10 13:42:49.000000 mysqlx-1.3.5/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     7290 2023-07-10 14:05:30.000000 mysqlx-1.3.5/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.5/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.5/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4248 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      589 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4248 2023-07-10 14:24:14.000000 mysqlx-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3449 2023-07-02 07:59:31.000000 mysqlx-1.3.5/README.md
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-10 14:24:14.000000 mysqlx-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-10 14:23:24.000000 mysqlx-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/test/
--rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.5/test/all_unit_test.py
--rw-rw-rw-   0        0        0      246 2023-07-02 23:03:01.000000 mysqlx-1.3.5/test/coder_test.py
--rw-rw-rw-   0        0        0     2832 2023-07-02 23:03:01.000000 mysqlx-1.3.5/test/dbx_test.py
--rw-rw-rw-   0        0        0     4934 2023-07-10 13:36:04.000000 mysqlx-1.3.5/test/db_test.py
--rw-rw-rw-   0        0        0      642 2023-07-08 17:06:12.000000 mysqlx-1.3.5/test/mapper_test.py
--rw-rw-rw-   0        0        0     1432 2023-07-10 14:22:09.000000 mysqlx-1.3.5/test/models.py
--rw-rw-rw-   0        0        0     5494 2023-07-03 02:33:32.000000 mysqlx-1.3.5/test/orm_test.py
--rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.5/test/snowflake_test.py
--rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.5/test/time_test.py
--rw-rw-rw-   0        0        0      575 2023-07-09 02:11:45.000000 mysqlx-1.3.5/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.5/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:21:13.000000 mysqlx-1.3.6/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx/
+-rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.3.6/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19125 2023-07-10 16:57:52.000000 mysqlx-1.3.6/mysqlx/db.py
+-rw-rw-rw-   0        0        0    12866 2023-07-10 17:10:18.000000 mysqlx-1.3.6/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    38006 2023-07-10 17:34:27.000000 mysqlx-1.3.6/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.6/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4052 2023-07-10 13:42:49.000000 mysqlx-1.3.6/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     9638 2023-07-10 17:21:09.000000 mysqlx-1.3.6/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.6/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4185 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      343 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 03:21:13.000000 mysqlx-1.3.6/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4185 2023-07-11 03:21:13.000000 mysqlx-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3660 2023-07-11 02:06:29.000000 mysqlx-1.3.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 03:21:13.000000 mysqlx-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-11 03:21:10.000000 mysqlx-1.3.6/setup.py
```

### Comparing `mysqlx-1.3.5/LICENSE` & `mysqlx-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.5/mysqlx/db.py` & `mysqlx-1.3.6/mysqlx/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import functools
 from typing import Sequence
-from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, log, get_named_sql, get_named_args, \
-    page_log, LIMIT_1, DBError, DB_LOCK, get_batch_args, logger
+from constant import LIMIT_1, MAPPER_PATH, PK_SQL
+from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
+    DB_LOCK, get_batch_args, logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
 
 _DB_CTX = None
 _SHOW_SQL = False
-_MAPPER_PATH = "mapper_path"
-_PK_SQL = 'SELECT LAST_INSERT_ID()'
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False, **kwargs):
     use_mysql_connector = False
     try:
         from mysql.connector import connect
         use_mysql_connector = True
@@ -27,18 +26,18 @@
         del kwargs['debug']
 
     is_pool = use_mysql_connector and pool_size >= 1
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _SHOW_SQL = show_sql
-        if _MAPPER_PATH in kwargs:
+        if MAPPER_PATH in kwargs:
             from .dbx import load_mapper
-            load_mapper(kwargs[_MAPPER_PATH])
-            del kwargs[_MAPPER_PATH]
+            load_mapper(kwargs[MAPPER_PATH])
+            del kwargs[MAPPER_PATH]
         if is_pool:
             kwargs['pool_size'] = pool_size
             if 'pool_name' not in kwargs:
                 kwargs['pool_name'] = "{}_pool".format(database)
         kwargs['user'] = user
         kwargs['password'] = password
         kwargs['database'] = database
@@ -112,66 +111,66 @@
 
     return _wrapper
 
 
 # ----------------------------------------------------------Update function------------------------------------------------------------------
 def insert(table: str, **kwargs):
     """
-    Execute insert SQL, return effect rowcount.
+    Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: name='张三', age=20}
     return: Effect rowcount
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('insert', table, kwargs))
+    insert_log('insert', table, **kwargs)
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
 def save(table: str, **kwargs):
     """
-    Execute insert SQL, return primary key.
+    Insert data into table, return primary key.
     :param table: table
     :param kwargs: name='张三', age=20
     :return: Primary key
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
+    insert_log('save', table, **kwargs)
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_save(sql, *args)
 
 
 @with_connection
 def do_save(sql: str, *args):
     """
-    Execute insert SQL, return primary key.
+    Insert data into table, return primary key.
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
-        cursor.execute(_PK_SQL)
+        cursor.execute(PK_SQL)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
     finally:
         if cursor:
             cursor.close()
 
 
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.execute', sql, *args, **kwargs)
+    sql_log('db.execute', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 def batch_insert(table: str, *args):
     """
     Batch insert
@@ -205,86 +204,86 @@
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.get', sql, *args, **kwargs)
+    sql_log('get', sql, *args, **kwargs)
     global _DB_CTX
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.query', sql, *args, **kwargs)
+    sql_log('query', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.query_one', sql, *args, **kwargs)
+    sql_log('query_one', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.select', sql, *args, **kwargs)
+    sql_log('select', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    log('db.select_one', sql, *args, **kwargs)
+    sql_log('select_one', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    page_log('db.query_page', sql, page_num, page_size, *args, **kwargs)
+    page_log('query_page', sql, page_num, page_size, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    page_log('db.select_page', sql, page_num, page_size, *args, **kwargs)
+    page_log('select_page', sql, page_num, page_size, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 @with_connection
 def do_execute(sql: str, *args):
@@ -331,26 +330,26 @@
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get', sql, args))
+    do_sql_log('do_get', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
     return do_get_with_limit(sql, *args)
 
 
 def do_get_with_limit(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get_with_limit', sql, args))
+    do_sql_log('do_get_with_limit', sql, *args)
     result = do_select_one_with_limit(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'mysqlx.db.%s' expect only one column but %d." % ('do_get_with_limit', len(result))
         logger.error('%s  \n\t\t sql: %s \n\t\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
@@ -382,15 +381,15 @@
 
 @with_connection
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_query_one', sql, args))
+    do_sql_log('do_query_one', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
     return do_query_one_with_limit(sql, *args)
 
 
 @with_connection
 def do_query_one_with_limit(sql: str, *args):
     """
@@ -432,15 +431,15 @@
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_select_one', sql, args))
+    do_sql_log('do_select_one', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
     return do_select_one_with_limit(sql, *args)
 
 
 @with_connection
 def do_select_one_with_limit(sql: str, *args):
     """
@@ -460,25 +459,25 @@
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    _do_page_log('do_query_page', sql, page_num, page_size, args)
+    do_page_log('do_query_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
     return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    _do_page_log('do_select_page', sql, page_num, page_size, args)
+    do_page_log('do_select_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
     return do_select(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
     if _DB_CTX.is_not_init():
@@ -546,12 +545,7 @@
         return True
 
     idx = lower_sql.rindex('limit')
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
 
     return False
-
-
-def _do_page_log(function: str, sql: str, page_num, page_size, *args):
-    logger.debug(
-        "Exec func 'mysqlx.db.%s', page_num: %d, page_size: %d \n\t\t sql: %s \n\t\t args: %s" % (function, page_num, page_size, sql.strip(), args))
```

### Comparing `mysqlx-1.3.5/mysqlx/dbx.py` & `mysqlx-1.3.6/mysqlx/dbx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 from typing import Mapping
 from jinja2 import Template
-from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction, logger
+from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction, logger, sql_id_log, page_sql_id_log
 from .db import do_get, do_query, do_query_one, do_execute, do_select_page, do_select, do_select_one, do_query_page, init_db as _init_db, \
     get_connection as _get_connection, insert as _insert, save as _save, batch_insert as _batch_insert, batch_execute as _batch_execute
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
@@ -19,39 +19,39 @@
         mapper_path='mapper', **kwargs):
     load_mapper(mapper_path)
     _init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
 
 def insert(table: str, **kwargs):
     """
-    Execute insert SQL, return effect rowcount.
+    Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     return: Effect rowcount
     """
     return _insert(table, **kwargs)
 
 
 def save(table: str, **kwargs):
     """
-    Execute insert SQL, return primary key.
+    Insert data into table, return primary key.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     :return: Primary key
     """
     return _save(table, **kwargs)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.execute', sql_id, *args, **kwargs)
+    sql_id_log('dbx.execute', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 def batch_insert(table: str, *args):
     """
     Batch insert
@@ -65,98 +65,99 @@
 def batch_execute(sql_id: str, *args):
     """
     Batch execute
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
+    logger.debug("Exec func 'mysqlx.dbx.%s' \n\t\t sql_id: '%s' \n\t\t args: %s" % ('batch_execute', sql_id, args))
     args = get_batch_args(*args)
     sql, _ = do_get_sql(get_sql_model(sql_id), True, None, *args)
     return _batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.get', sql_id, *args, **kwargs)
+    sql_id_log('get', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.query', sql_id, *args, **kwargs)
+    sql_id_log('query', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.query_one', sql_id, *args, **kwargs)
+    sql_id_log('query_one', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.select', sql_id, *args, **kwargs)
+    sql_id_log('select', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _sql_id_log('dbx.select_one', sql_id, *args, **kwargs)
+    sql_id_log('select_one', sql_id, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _page_log('dbx.query_page', sql_id, page_num, page_size, *args, **kwargs)
+    page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    _page_log('dbx.select_page', sql_id, page_num, page_size, *args, **kwargs)
+    page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
     sql, args = get_sql(sql_id, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 def get_connection():
     return _get_connection()
 
@@ -290,18 +291,9 @@
     else:
         _valid_sql(sql_id, sql, child.tag)
         _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace)
 
     return _id, includes
 
 
-def _sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func 'mysqlx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
-
-
-def _page_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
-    logger.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (
-        function, page_num, page_size, sql_id.strip(), args, kwargs))
-
-
 def _valid_sql(sql_id, sql, tag):
     assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `mysqlx-1.3.5/mysqlx/orm.py` & `mysqlx-1.3.6/mysqlx/orm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import sys
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
 from typing import Sequence, Union, List, Tuple
-from .support import LIMIT_1, DBError, simple_sql, logger
-from .db import do_get_with_limit, do_query, do_query_one_with_limit, do_execute, insert, save, do_select, do_select_one_with_limit, transaction,\
+from .support import DBError, simple_sql, logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log
+from constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
+    COLUMN_SQL
+from .db import do_get_with_limit, do_query, do_query_one_with_limit, do_execute, insert, save, do_select, do_select_one_with_limit, transaction, \
     batch_insert, do_query_page, do_select_page, do_get
 
-NO_LIMIT = 0
-DEFAULT_PK_FIELD = 'id'
-SYMBOLS = ['=', '>', '<']
-BETWEEN, LIKE, IN = 'between', 'like', 'in'
-PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__', '__pk_strategy__'
-_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
-                 FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? limit ?'''
-
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
 class PkStrategy(Enum):
@@ -80,39 +74,39 @@
 
     def persist(self):
         """
         user = User(name='张三', age=55)
         effect_rowcount = user.persist()
         :return: effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('persist', self.__class__.__name__))
+        orm_inst_log('persist', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         return self.insert(**kv)
 
     def inst_save(self):
         """
         user = User(name='张三', age=55)
         id = user.save()
         :return: Primary key
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('inst_save', self.__class__.__name__))
+        orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         pk = self._get_pk()
         _id = self.save(**kv)
         if pk not in kv:
             self.__dict__.update({pk: _id})
         return _id
 
     def update(self):
         """
         user = User(id=1, name='李四', age=66)
         rowcount = user.update()
         :return: Effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('update', self.__class__.__name__))
+        orm_inst_log('update', self.__class__.__name__)
         pk, table = self._get_pk_and_table()
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         if pk not in kv:
             raise KeyError("Not primary key.")
 
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
@@ -148,71 +142,71 @@
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         user = User(id=1)
         rowcount = user.logical_delete()
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('logical_delete', self.__class__.__name__))
+        orm_inst_log('logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
 
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         user = User(id=1)
         rowcount = user.un_logical_delete()
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('un_logical_delete', self.__class__.__name__))
+        orm_inst_log('un_logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         user = User(id=1)
         rowcount = user.delete()
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('delete', self.__class__.__name__))
+        orm_inst_log('delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = User.insert(name='张三', age=20)
         return: Effect rowcount
         """
-        _insert_log('insert', cls.__name__, **kwargs)
+        orm_insert_log('insert', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
             kwargs[pk] = get_id()
         return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = User.save(name='张三', age=20)
         :return: Primary key
         """
-        _insert_log('save', cls.__name__, **kwargs)
+        orm_insert_log('save', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE:
             if pk in kwargs:
                 _id = kwargs[pk]
             else:
                 _id = get_id()
@@ -224,23 +218,23 @@
 
     @classmethod
     def create(cls, **kwargs):
         """
         user = User.create(name='张三', age=20)
         :return: Instance object
         """
-        _insert_log('create', cls.__name__, **kwargs)
+        orm_insert_log('create', cls.__name__, **kwargs)
         pk = cls._get_pk()
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
         return cls._dict2obj(kwargs)
 
     @classmethod
-    def update_by_id(cls, _id, **kwargs):
+    def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = User.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
         pk = cls._get_pk()
@@ -248,46 +242,46 @@
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
         return do_execute(sql, *args, _id, LIMIT_1)
 
     @classmethod
-    def logical_delete_by_id(cls, _id, update_by=None):
+    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = User.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        _delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
+        orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_id(cls, _id, update_by=None):
+    def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        _delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
+        orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
-    def logical_delete_by_ids(cls, ids: Sequence, update_by=None, batch_size=128):
+    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
             'logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_ids(cls, ids: Sequence, update_by=None, batch_size=128):
+    def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
             'un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
@@ -296,35 +290,35 @@
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = User.delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM `%s` %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_execute(sql, *args)
 
     @classmethod
-    def delete_by_id(cls, _id):
+    def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = User.delete_by_id(id=1)
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
         return do_execute(sql, _id, LIMIT_1)
 
     @classmethod
-    def delete_by_ids(cls, ids: Sequence[int], batch_size=128):
+    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Physical delete
         rowcount = User.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, batch_size: %s" % (
             'delete_by_ids', cls.__name__, ids, batch_size))
@@ -375,29 +369,29 @@
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
         sql = "SELECT count(1) FROM `{}` {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('exists', cls.__name__, kwargs))
         return cls.count(**kwargs) > 0
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return cls.count_by(where, *args, **kwargs) > 0
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find('id', 'name', 'age', name='张三', age=55)
@@ -419,53 +413,53 @@
 
     @classmethod
     def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        _page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls._dict2obj(d) for d in result]
 
     @classmethod
     def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
-    def find_by_id(cls, _id, *fields):
+    def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         user = User.find_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('find_by_id', cls.__name__, _id, fields))
         result = cls.query_by_id(_id, *fields)
         return cls._dict2obj(result) if result else None
 
     @classmethod
-    def find_by_ids(cls, ids: Sequence, *fields):
+    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(class object) or empty list if no result.
         users = User.find_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('find_by_ids', cls.__name__, ids, fields))
@@ -504,61 +498,61 @@
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        _page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.query_by_page(1, 10, 'where name=?', '李四')
         """
-        _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def query_by_id(cls, _id, *fields):
+    def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         user = User.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_query_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
-    def query_by_ids(cls, ids: Sequence[int], *fields):
+    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         users = User.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('query_by_ids', cls.__name__, ids, fields))
@@ -603,61 +597,61 @@
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        _page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.select_by_page(1, 10, 'where name=?', '李四')
         """
-        _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def select_by_id(cls, _id, *fields):
+    def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = User.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_select_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
-    def select_by_ids(cls, ids: Sequence[int], *fields):
+    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('select_by_ids', cls.__name__, ids, fields))
@@ -667,15 +661,15 @@
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_select(sql, *ids, ids_size)
 
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
-    def _logical_delete_by_id_op(cls, _id, update_by=None, del_status=DelFlag.DELETED):
+    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         pk, table = cls._get_pk_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s`=?' % pk
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
@@ -685,30 +679,31 @@
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
             return do_execute(sql, del_status.value, _id, LIMIT_1)
 
     @classmethod
-    def _logical_delete_by_ids_op(cls, ids: Sequence[int], update_by=None, batch_size=128, del_status=DelFlag.DELETED):
+    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
+            del_status=DelFlag.DELETED):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
             return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
         elif ids_size <= batch_size:
             return cls._do_logical_delete_by_ids(ids, update_by, del_status)
         else:
             split_ids = _split_ids(ids, batch_size)
             with transaction():
                 results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
             return sum(results)
 
     @classmethod
-    def _do_logical_delete_by_ids(cls, ids: Sequence, update_by=None, del_status=DelFlag.DELETED):
+    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         pk = cls._get_pk()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
         if update_by is not None and update_by_field is not None:
@@ -719,15 +714,15 @@
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
             return do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
-    def _delete_by_ids(cls, ids: Sequence):
+    def _delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         ids_size = len(ids)
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `{}` WHERE `{}` in ({}) limit ?'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
         return do_execute(sql, *ids, ids_size)
 
     @classmethod
     def _get_pk(cls):
@@ -815,15 +810,15 @@
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
 
 
 @lru_cache(maxsize=128)
 def _get_table_columns(table: str):
-    return do_get_with_limit(_COLUMN_SQL, table, LIMIT_1)
+    return do_get_with_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _delete_by_id_sql(table, pk):
     return 'DELETE FROM `{}` WHERE `{}`=? limit ?'.format(table, pk)
 
 
 def _get_condition_arg(k: str, v: object):
@@ -896,29 +891,7 @@
 
 
 def _get_table_name(class_name):
     for i in range(1, len(class_name) - 1)[::-1]:
         if class_name[i].isupper():
             class_name = class_name[:i] + '_' + class_name[i:]
     return class_name.lower()
-
-
-def _by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
-        function, page_num, page_size, class_name, where, args, kwargs))
-
-
-def _page_log(function, page_num, page_size, class_name, *fields, **kwargs):
-    logger.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', fields: %s, kwargs: %s" % (
-        function, page_num, page_size, class_name, fields, kwargs))
-
-
-def _insert_log(function, class_name, **kwargs):
-    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
-
-
-def _delete_by_id_log(function, class_name, _id, update_by):
-    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
-
-
-def _by_log(function, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
```

### Comparing `mysqlx-1.3.5/mysqlx/snowflake.py` & `mysqlx-1.3.6/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.5/mysqlx/sql_mapper.py` & `mysqlx-1.3.6/mysqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.5/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.6/mysqlx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.5
+Version: 1.3.6
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Install
-'''''''
-
-.. code:: shell
-
-   pip install mysqlx
-
 Mapper file
 '''''''''''
 
 Create a mapper file in ‘mapper’ folder, you can named
 ‘user_mapper.xml’, like follow:
 
 .. code:: xml
@@ -66,15 +59,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from user where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306' user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        users = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `mysqlx-1.3.5/PKG-INFO` & `mysqlx-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.5
+Version: 1.3.6
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Install
-'''''''
-
-.. code:: shell
-
-   pip install mysqlx
-
 Mapper file
 '''''''''''
 
 Create a mapper file in ‘mapper’ folder, you can named
 ‘user_mapper.xml’, like follow:
 
 .. code:: xml
@@ -66,15 +59,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from user where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306' user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        users = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `mysqlx-1.3.5/setup.py` & `mysqlx-1.3.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
-from setuptools import setup, find_packages
+from setuptools import setup
 
 # INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
-long_description = read("README_en.rst")
+long_description = read("README.rst")
 
 setup(
     name='mysqlx',
-    packages=find_packages(),
+    packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.5',
+    version='1.3.6',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

