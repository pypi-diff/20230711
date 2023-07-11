# Comparing `tmp/mysqlx-1.3.1.tar.gz` & `tmp/mysqlx-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.1.tar", last modified: Tue Jun 20 09:06:19 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.8.tar", last modified: Tue Jul 11 05:58:04 2023, max compression
```

## Comparing `mysqlx-1.3.1.tar` & `mysqlx-1.3.8.tar`

### file list

```diff
@@ -1,32 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.1/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.3.1/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.3.1/mysqlx/db.py
--rw-rw-rw-   0        0        0    10001 2023-06-20 01:39:01.000000 mysqlx-1.3.1/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.3.1/mysqlx/orm.py
--rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.3.1/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.1/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      487 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-06-20 08:57:34.000000 mysqlx-1.3.1/README.md
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-20 09:06:19.000000 mysqlx-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-06-20 09:01:58.000000 mysqlx-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/test/
--rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.3.1/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.1/test/coder_test.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.3.1/test/dbx_test.py
--rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.3.1/test/db_test.py
--rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.3.1/test/models.py
--rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.3.1/test/orm_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.1/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.1/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:58:04.000000 mysqlx-1.3.8/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.8/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx/
+-rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.3.8/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19126 2023-07-11 03:25:48.000000 mysqlx-1.3.8/mysqlx/db.py
+-rw-rw-rw-   0        0        0    12866 2023-07-10 17:10:18.000000 mysqlx-1.3.8/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    38007 2023-07-11 03:25:48.000000 mysqlx-1.3.8/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.8/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4052 2023-07-10 13:42:49.000000 mysqlx-1.3.8/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     9639 2023-07-11 03:25:48.000000 mysqlx-1.3.8/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.8/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 05:57:36.000000 mysqlx-1.3.8/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4185 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      343 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 05:58:04.000000 mysqlx-1.3.8/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4185 2023-07-11 05:58:04.000000 mysqlx-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3660 2023-07-11 02:06:29.000000 mysqlx-1.3.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 05:58:04.000000 mysqlx-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2023-07-11 05:58:00.000000 mysqlx-1.3.8/setup.py
```

### Comparing `mysqlx-1.3.1/LICENSE` & `mysqlx-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.1/mysqlx/db.py` & `mysqlx-1.3.8/mysqlx/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,58 @@
-import logging
 import functools
-from typing import Any, Union, Mapping, Sequence
-from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, log, get_named_sql, get_named_args, page_log, LIMIT_1, DBError
+from typing import Sequence
+from .constant import LIMIT_1, MAPPER_PATH, PK_SQL
+from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
+    DB_LOCK, get_batch_args, logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
 
 _DB_CTX = None
 _SHOW_SQL = False
-_PK_SQL = 'SELECT LAST_INSERT_ID()'
 
 
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False, **kwargs):
-    from mysql.connector import connect
-    from mysql.connector.pooling import CONNECTION_POOL_LOCK
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False, **kwargs):
+    use_mysql_connector = False
+    try:
+        from mysql.connector import connect
+        use_mysql_connector = True
+    except ImportError:
+        from pymysql import connect
+
     global _DB_CTX
     global _SHOW_SQL
 
-    with CONNECTION_POOL_LOCK:
+    if 'debug' in kwargs:
+        if kwargs['debug']:
+            from logging import DEBUG
+            logger.setLevel(DEBUG)
+        del kwargs['debug']
+
+    is_pool = use_mysql_connector and pool_size >= 1
+    with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-
         _SHOW_SQL = show_sql
-        if 'mapper_dir' in kwargs:
-            del kwargs['mapper_dir']
-
-        if pool_size >= 1:
+        if MAPPER_PATH in kwargs:
+            from .dbx import load_mapper
+            load_mapper(kwargs[MAPPER_PATH])
+            del kwargs[MAPPER_PATH]
+        if is_pool:
             kwargs['pool_size'] = pool_size
             if 'pool_name' not in kwargs:
-                kwargs['pool_name'] = "%s_pool" % database
-
+                kwargs['pool_name'] = "{}_pool".format(database)
         kwargs['user'] = user
         kwargs['password'] = password
         kwargs['database'] = database
         kwargs['host'] = host
         kwargs['port'] = port
         kwargs['use_unicode'] = use_unicode
-        _DB_CTX = DBCtx(lambda: connect(**kwargs))
-
-    if pool_size >= 1:
-        logging.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
+        _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
+    if is_pool:
+        logger.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
-        logging.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
+        logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
@@ -94,175 +104,186 @@
     """
     global _DB_CTX
 
     @functools.wraps(func)
     def _wrapper(*args, **kw):
         with TransactionCtx(_DB_CTX):
             return func(*args, **kw)
+
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
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('insert', table, kwargs))
+    insert_log('insert', table, **kwargs)
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
-@with_connection
 def save(table: str, **kwargs):
     """
-    Execute insert SQL, return primary key.
-    :param table: table name
-    :param kwargs: name='张三', age=20}
+    Insert data into table, return primary key.
+    :param table: table
+    :param kwargs: name='张三', age=20
+    :return: Primary key
+    """
+    insert_log('save', table, **kwargs)
+    sql, args = _insert_sql_args(table.strip(), **kwargs)
+    return do_save(sql, *args)
+
+
+@with_connection
+def do_save(sql: str, *args):
+    """
+    Insert data into table, return primary key.
+    :param sql: table
+    :param args:
     :return: Primary key
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
     global _DB_CTX
     cursor = None
-    sql, args = _insert_sql_args(table.strip(), ** kwargs)
-    sql = _before_execute('save', sql, *args)
+    sql = _before_execute('do_save', sql, *args)
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
 
 
-def batch_insert(table: str, args: Sequence[Mapping[str, Any]]):
+def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', args: %s" % ('batch_insert', table, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', args: %s" % ('batch_insert', table, args))
     assert len(args) > 0, 'args must not be empty.'
-    sql, args = _batch_insert_sql_args(table, args)
-    return batch_execute(sql, args)
+    sql, args = _batch_insert_sql_args(table, *args)
+    return batch_execute(sql, *args)
 
 
-def batch_execute(sql: str, args: Union[Sequence[Sequence[Any]], Sequence[Mapping[str, Any]]]):
+def batch_execute(sql: str, *args):
     """
     Batch execute
     :param sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
                 INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :param args: All number must have same size.
     :return: Effect row count
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: '%s' \n\t\t args: %s" % ('batch_execute', sql, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: '%s' \n\t\t args: %s" % ('batch_execute', sql, args))
     assert len(args) > 0, 'args must not be empty.'
     if isinstance(args[0], dict):
-        sql, args = _batch_named_sql_args(sql, args)
+        sql, args = _batch_named_sql_args(sql, *args)
 
-    return do_batch_execute(sql, args)
+    return do_batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
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
@@ -281,93 +302,115 @@
         return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def do_batch_execute(sql: str, args: Sequence[Sequence[Any]]):
+def do_batch_execute(sql: str, *args):
     """
     Batch execute sql return effect rowcount
     :param sql: insert into user(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_batch_execute', sql.strip(), *args)
+    args = get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
 def do_get(sql: str, *args):
     """
-    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
+    MultiColumnsError: Expect only one column.
+    sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    do_sql_log('do_get', sql, *args)
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_get_with_limit(sql, *args)
+
+
+def do_get_with_limit(sql: str, *args):
+    """
+    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t  args: %s" % ('do_get', sql, args))
-    result = do_select_one(sql, *args)
+    do_sql_log('do_get_with_limit', sql, *args)
+    result = do_select_one_with_limit(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
-        msg = "Exec func 'mysqlx.db.%s' expect only one column but %d." % ('do_get', len(result))
-        logging.error('%s  \n\t\t sql: %s \n\t\t args: %s' % (msg, sql, args))
+        msg = "Exec func 'mysqlx.db.%s' expect only one column but %d." % ('do_get_with_limit', len(result))
+        logger.error('%s  \n\t\t sql: %s \n\t\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
 
 
 @with_connection
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_select', sql.strip(), *args)
+    sql = _before_execute('do_query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
-        if cursor.description:
+        results = cursor.fetchall()
+        if results and cursor.description:
             names = [x[0] for x in cursor.description]
-            return [Dict(names, x) for x in cursor.fetchall()]
+            return [Dict(names, x) for x in results]
         else:
-            return cursor.fetchall()
+            return results
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
 def do_query_one(sql: str, *args):
     """
-    execute select SQL and return unique result(dict). Automatically add 'limit ?' after sql statement if not.
+    execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    do_sql_log('do_query_one', sql, *args)
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_query_one_with_limit(sql, *args)
+
+
+@with_connection
+def do_query_one_with_limit(sql: str, *args):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql, args = _limit_one_sql_args(sql, *args)
-    sql = _before_execute('do_query_one', sql.strip(), *args)
+    sql = _before_execute('do_query_one_with_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
-        if cursor.description:
+        result = cursor.fetchone()
+        if result and cursor.description:
             names = [x[0] for x in cursor.description]
-            result = cursor.fetchone()
-            return Dict(names, result) if result else result
-        else:
-            return cursor.fetchone()
+            return Dict(names, result)
+        return result
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
 def do_select(sql: str, *args):
@@ -383,50 +426,59 @@
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
 
 
-@with_connection
 def do_select_one(sql: str, *args):
     """
-    Execute select SQL and return unique result(tuple). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    do_sql_log('do_select_one', sql, *args)
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_select_one_with_limit(sql, *args)
+
+
+@with_connection
+def do_select_one_with_limit(sql: str, *args):
+    """
+    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql, args = _limit_one_sql_args(sql, *args)
-    sql = _before_execute('do_select_one', sql.strip(), *args)
+    sql = _before_execute('do_select_one_with_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
+    do_page_log('do_query_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
-    sql = _before_execute('do_query_page', sql.strip(), *args)
     return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
+    do_page_log('do_select_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
-    sql = _before_execute('do_select_page', sql.strip(), *args)
     return do_select(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
     if _DB_CTX.is_not_init():
         _DB_CTX.init()
@@ -437,52 +489,56 @@
     global _DB_CTX
     _DB_CTX.prepared = prepared
 
 
 def _before_execute(function: str, sql: str, *args):
     global _SHOW_SQL
     if _SHOW_SQL:
-        logging.info("Exec func 'mysqlx.db.%s' \n\t\tSQL: %s \n\t\tARGS: %s" % (function, sql, args))
+        logger.info("Exec func 'mysqlx.db.%s' \n\t\tSQL: %s \n\t\tARGS: %s" % (function, sql, args))
     return sql.replace('?', '%s')
 
 
 def _insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = _create_insert_sql(table, cols)
     return sql, args
 
 
-def _batch_insert_sql_args(table: str, args: Sequence[Mapping[str, Any]]):
+def _batch_insert_sql_args(table: str, *args):
+    args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
-    cols, args = zip(*args)
+    cols, args = zip(*args)  # (cols), (args)
     sql = _create_insert_sql(table, cols[0])
     return sql, args
 
 
-def _batch_named_sql_args(sql: str, args: Sequence[Mapping[str, Any]]):
+def _batch_named_sql_args(sql: str, *args):
+    args = get_batch_args(*args)
     args = [get_named_args(sql, **arg) for arg in args]
     sql = get_named_sql(sql)
     return sql, args
 
 
+@functools.lru_cache(maxsize=128)
 def _create_insert_sql(table: str, cols: Sequence[str]):
-    return 'INSERT INTO `%s` (%s) VALUES (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for _ in range(len(cols))]))
+    columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
+    return 'INSERT INTO `{}` ({}) VALUES ({})'.format(table, ','.join(columns), ','.join(placeholders))
 
 
 def _page_sql_args(sql: str, page_num=1, page_size=10, *args):
+    start = (page_num - 1) * page_size
+    args = [*args, start, page_size]
     if _require_limit(sql):
-        sql = '%s limit ?,?' % sql
-        start = (page_num - 1) * page_size
-        args = [*args, start, page_size]
+        sql = '{} limit ?,?'.format(sql)
     return sql, args
 
 
 def _limit_one_sql_args(sql: str, *args):
     if _require_limit(sql):
-        return '%s limit ?' % sql, [*args, LIMIT_1]
+        return '{} limit ?'.format(sql), [*args, LIMIT_1]
 
     return sql, args
 
 
 def _require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
```

### Comparing `mysqlx-1.3.1/mysqlx/dbx.py` & `mysqlx-1.3.8/mysqlx/dbx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,299 @@
 import os
-from . import db
+import re
+from typing import Mapping
 from jinja2 import Template
-from typing import Any, Union, Sequence, Mapping
-from .support import simple_sql, SqlModel, log, page_log, MapperError, is_dynamic_sql
+from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction, logger, sql_id_log, page_sql_id_log
+from .db import do_get, do_query, do_query_one, do_execute, do_select_page, do_select, do_select_one, do_query_page, init_db as _init_db, \
+    get_connection as _get_connection, insert as _insert, save as _save, batch_insert as _batch_insert, batch_execute as _batch_execute
+
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
+_valid_sql_actions = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.SELECT.value)
 
 
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False,
-            mapper_dir='mapper', **kwargs):
-    _load_mapper(mapper_dir)
-    db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False,
+        mapper_path='mapper', **kwargs):
+    load_mapper(mapper_path)
+    _init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
 
 def insert(table: str, **kwargs):
     """
-    Execute insert SQL, return effect rowcount.
+    Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     return: Effect rowcount
     """
-    return db.insert(table, **kwargs)
+    return _insert(table, **kwargs)
 
 
 def save(table: str, **kwargs):
     """
-    Execute insert SQL, return primary key.
+    Insert data into table, return primary key.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     :return: Primary key
     """
-    return db.save(table, **kwargs)
+    return _save(table, **kwargs)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.execute', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_execute(sql, *args)
+    sql_id_log('dbx.execute', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_execute(sql, *args)
 
 
-def batch_insert(table: str, args: Sequence[Mapping[str, Any]]):
+def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    return db.batch_insert(table, args)
+    return _batch_insert(table, *args)
 
 
-def batch_execute(sql_id: str, args: Union[Sequence[Sequence[Any]], Sequence[Mapping[str, Any]]]):
+def batch_execute(sql_id: str, *args):
     """
     Batch execute
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    sql = get_sql(sql_id)
-    return db.batch_execute(sql, args)
+    logger.debug("Exec func 'mysqlx.dbx.%s' \n\t\t sql_id: '%s' \n\t\t args: %s" % ('batch_execute', sql_id, args))
+    args = get_batch_args(*args)
+    sql, _ = do_get_sql(get_sql_model(sql_id), True, None, *args)
+    return _batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.get', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_get(sql, *args)
+    sql_id_log('get', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_get(sql, *args)
 
 
 def query(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.query', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query(sql, *args)
+    sql_id_log('query', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query(sql, *args)
 
 
 def query_one(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one row result(dict). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.query_one', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query_one(sql, *args)
+    sql_id_log('query_one', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query_one(sql, *args)
 
 
 def select(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.select', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select(sql, *args)
+    sql_id_log('select', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select(sql, *args)
 
 
 def select_one(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.select_one', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select_one(sql, *args)
+    sql_id_log('select_one', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select_one(sql, *args)
 
 
 def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    page_log('dbx.query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query_page(sql, page_num, page_size, *args)
+    page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    page_log('dbx.select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select_page(sql, page_num, page_size, *args)
+    page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select_page(sql, page_num, page_size, *args)
 
 
 def get_connection():
-    return db.get_connection()
+    return _get_connection()
+
+
+def get_sql(sql_id: str, *args, **kwargs):
+    sql_model = get_sql_model(sql_id)
+    return do_get_sql(sql_model, False, None, *args, **kwargs)
+
+
+def do_get_sql(sql_model, batch, param_names, *args, **kwargs):
+    """
+    Get sql from SqlModel.
+    :param sql_model: SqlModel
+    :param batch: bool, is batch or not
+    :param param_names: original function parameter names
+    :param args:
+    :param kwargs:
+    :return:
+    """
+    if sql_model.dynamic:
+        sql = sql_model.sql.render(**kwargs)
+        logger.debug("Original sql: {}".format(sql))
+        return get_named_sql_args(sql, **kwargs)
+    else:
+        logger.debug("Original sql: {}".format(sql_model.sql))
+        if sql_model.mapping and kwargs:
+            return get_named_sql_args(sql_model.sql, **kwargs)
+        elif sql_model.placeholder and kwargs:
+            logger.warning("Better use 'func(arg1, arg2...)' then 'func(arg1=arg1, arg2=arg2...)' if sql contain '?' placeholder.")
+            args = [kwargs[name] for name in param_names if name in kwargs] if param_names else list(kwargs.values())
+        elif sql_model.mapping and not kwargs and (not batch or
+                                                   (batch and (not args or not isinstance(args[0], Mapping)))):  # batch_execute时args可能为List[Mapping]
+            raise MapperError("Parameter 'kwargs' must not be empty when named mapping sql.")
+        return sql_model.sql, args
+
+
+def build_sql_id(namespace, _id):
+    return namespace + "." + _id
+
+
+def get_sql_model(sql_id: str):
+    global _SQL_CONTAINER
+    return _SQL_CONTAINER[sql_id]
 
 
 # ----------------------------------------------------------Load mapper--------------------------------------------------------------------
-# def _get_abs_path(path: str):
-#     parent_flg = '../'
-#     current_flg = './'
-#     if path.startswith(parent_flg):
-#         idx = path.rindex(parent_flg) + 3
-#         parent_path = path[:idx]
-#         os.chdir(parent_path)
-#         path = path[idx:]
-#     elif path.startswith(current_flg):
-#         path = path[2:]
-#     return os.path.join(os.getcwd(), path)
-
-
-def _load_mapper(path: str):
-    # if not os.path.isabs(path):
-    #     path = _get_abs_path(path)
+def load_mapper(path: str):
     if os.path.isfile(path) and path.endswith(".xml"):
         _parse_mapper_file(path)
     elif os.path.isdir(path):
         for f in os.listdir(path):
             file = os.path.join(path, f)
             if os.path.isfile(file) and f.endswith(".xml"):
                 _parse_mapper_file(file)
             elif os.path.isdir(file):
-                _load_mapper(file)
+                load_mapper(file)
 
 
 def _parse_mapper_file(file: str):
+    global _SQL_CONTAINER
     tree = ET.parse(file)
     root = tree.getroot()
     namespace = root.attrib.get('namespace', '')
     results = list(map(lambda child: _load_sql(namespace, child, file), root))
-    sql_ids, file_includes = zip(*results)
-    invalid_includes = [include for includes in file_includes if includes for include in includes if include not in sql_ids]
-    if invalid_includes:
-        raise MapperError("Includes %s are not exist in mapper file: %s" % (set(invalid_includes), file))
-
-
-def get_sql(sql_id: str, **kwargs):
-    sql_model = _get_sql_model(sql_id)
-    if sql_model.includes:
-        for include in sql_model.includes:
-            assert include not in kwargs, "include: '%s' in kwargs: %s" % (include, kwargs)
-            kwargs[include] = get_sql(_build_sql_id(sql_model.namespace, include), **kwargs)
-    return sql_model.sql.render(**kwargs) if sql_model.dynamic else sql_model.sql
-
-
-def _get_sql_model(sql_id: str):
-    global _SQL_CONTAINER
-    return _SQL_CONTAINER[sql_id]
-
-
-def _build_sql_id(namespace, _id):
-    return namespace + "." + _id
+    sql_ids, file_all_includes = zip(*results)
+    for i, includes in enumerate(file_all_includes):
+        if includes:
+            for include in includes:
+                if include not in sql_ids:
+                    raise MapperError("Include '%s' are not exist in mapper file: %s" % (include, file))
+
+                include_sql_id = build_sql_id(namespace, include)
+                include_sql_model = _SQL_CONTAINER[include_sql_id]
+                if include_sql_model.includes:
+                    raise MapperError("Nested include: '%s' include '%s' and it include %s in mapper file: %s" % (
+                        sql_ids[i], include, include_sql_model.includes, file))
+
+    # include sql
+    include_results = filter(lambda x: x[1] is not None, results)
+    for sql_id, includes in include_results:
+        _handle_includes(build_sql_id(namespace, sql_id), includes)
+
+    # dynamic sql change to Template
+    for sql_id in sql_ids:
+        sql_model = _SQL_CONTAINER[build_sql_id(namespace, sql_id)]
+        if sql_model.dynamic:
+            sql_model.sql = Template(sql_model.sql)
+
+
+def _handle_includes(sql_id, includes):
+    is_dynamic = False
+    sql_model = _SQL_CONTAINER[sql_id]
+    for include in includes:
+        include_sql_id = build_sql_id(sql_model.namespace, include)
+        include_sql_model = _SQL_CONTAINER[include_sql_id]
+        if include_sql_model.dynamic:
+            is_dynamic = True
+        if include_sql_model.includes:
+            _handle_includes(include_sql_id, include_sql_model.includes)
+        sql = re.sub(r'{{\s*%s\s*}}' % include, include_sql_model.sql, sql_model.sql)
+
+    _valid_sql(sql_id, sql, sql_model.action)
+    if is_dynamic or is_dynamic_sql(sql):
+        sql_model.dynamic = True
+        sql_model.mapping = True
+        sql_model.placeholder = False
+    else:
+        sql_model.mapping = ':' in sql
+        sql_model.placeholder = False if sql_model.mapping else '?' in sql
+    sql_model.sql = sql
+    sql_model.includes = None
 
 
 def _load_sql(namespace, child, file):
     global _SQL_CONTAINER
-    # child.tag = select
     includes = None
     _id = child.attrib.get('id')
     assert _id, "Mapper 'id' must be set in mapper file: %s." % file
-    sql_id = _build_sql_id(namespace, _id)
+    sql_id = build_sql_id(namespace, _id)
     assert sql_id not in _SQL_CONTAINER, "Sql id '%s' repeat." % sql_id
     include = child.attrib.get('include')
     sql = child.text.strip()
     if include:
         includes = include.split(",")
         for include in set(includes):
             assert include != _id, "Include must not be it self, id: '%s' = include: '%s' " % (_id, include)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), namespace=namespace, dynamic=True, includes=includes)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, includes=includes)
     elif is_dynamic_sql(sql):
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), namespace=namespace, dynamic=True)
+        _valid_sql(sql_id, sql, child.tag)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, dynamic=True)
     else:
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, namespace=namespace)
+        _valid_sql(sql_id, sql, child.tag)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace)
 
     return _id, includes
 
+
+def _valid_sql(sql_id, sql, tag):
+    assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `mysqlx-1.3.1/mysqlx/orm.py` & `mysqlx-1.3.8/mysqlx/orm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 import sys
-import logging
-from . import db
-from enum import IntEnum
-from typing import Any, Mapping, Sequence
 from datetime import datetime
-from .support import LIMIT_1, DBError
-
-NO_LIMIT = 0
-DEFAULT_PK_FIELD = 'id'
-SYMBOLS = ['=', '>', '<']
-BETWEEN, LIKE, IN = 'between', 'like', 'in'
-PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__'
+from .snowflake import get_id
+from enum import Enum, IntEnum
+from functools import lru_cache
+from typing import Sequence, Union, List, Tuple
+from .support import DBError, simple_sql, logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
+    COLUMN_SQL
+from .db import do_get_with_limit, do_query, do_query_one_with_limit, do_execute, insert, save, do_select, do_select_one_with_limit, transaction, \
+    batch_insert, do_query_page, do_select_page, do_get
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
+class PkStrategy(Enum):
+    """
+    SNOWFLAKE: 由Snowflake算法生成主键
+    DB_AUTO_INCREMENT: 由数据库的AUTO_INCREMENT自动生成主键
+
+    在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
+    OverflowError: Python int too large to convert to C long
+
+    如果用的是mysql.connector，且在Windows上开发测试，可以就在初始化数据库的时候加上参数'use_pure'为True用纯python的connect; 在linux是部署生成环境时去掉'use_pure'用
+    C语言写的connect, 以提高性能.
+    """
+    SNOWFLAKE = 'snowflake'
+    DB_AUTO_INCREMENT = 'db_auto_increment'
+
+
 class Model:
     """
-    Use db.init_db(...) or dbx.init_db(...) init db first, then create a class extends Model:
+    Create a class extends Model:
 
     class User(Model):
         __pk__ = 'id'
         __table__ = 'user'
         __update_by__ = 'update_by'
         __update_time__ = 'update_time'
         __del_flag__ = 'del_flag'
@@ -32,19 +45,24 @@
         def __init__(self, id: int = None, name: str = None, age: int = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
             self.id = id
             self.update_by = update_by
             self.update_time = update_time
             self.del_flag = del_flag
             self.name = name
             self.age = age
+
+    then you can use like follow:
+        db.init_db(user='xxx', password='xxx', database='xxx', host='xxx', ...)  # or dbx.init_db(...) init db first,
+        user = User(name='张三', age=55)
+        effect_rowcount = user.persist()
+        id = user.inst_save()
     """
 
     def __str__(self):
-        kv = {k: v for k, v in self.__dict__.items() if not k.startswith("__")}
-        return str(kv)
+        return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
 
     def __getattr__(self, name):
         if PK == name:
             return self._get_pk()
         elif TABLE == name:
             return self._get_table()
         elif UPDATE_BY == name:
@@ -53,580 +71,691 @@
             return self._get_update_time_field()
         else:
             return None
 
     def persist(self):
         """
         user = User(name='张三', age=55)
-        id = user.persist()
+        effect_rowcount = user.persist()
+        :return: effect rowcount
+        """
+        orm_inst_log('persist', self.__class__.__name__)
+        kv = {k: v for k, v in self.__dict__.items() if v is not None}
+        return self.insert(**kv)
+
+    def inst_save(self):
+        """
+        user = User(name='张三', age=55)
+        id = user.save()
         :return: Primary key
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('persist', self.__class__.__name__))
+        orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        self.id = db.save(self._get_table(), **kv)
-        return self.id
+        pk = self._get_pk()
+        _id = self.save(**kv)
+        if pk not in kv:
+            self.__dict__.update({pk: _id})
+        return _id
 
     def update(self):
         """
         user = User(id=1, name='李四', age=66)
         rowcount = user.update()
         :return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('update', self.__class__.__name__))
+        orm_inst_log('update', self.__class__.__name__)
         pk, table = self._get_pk_and_table()
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         if pk not in kv:
             raise KeyError("Not primary key.")
 
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
             return self.update_by_id(kv[pk], **update_kv)
         else:
-            logging.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t\t   %s" % ('update', self.__class__.__name__, self))
+            logger.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
-        :param fields: Default select all fields with 'select *' if not set. like: ('id', 'name', 'age')
+        :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         user = User(id=1)
         user2 = user.load()
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
         pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
         if _id is not None:
             if not fields:
                 fields, _ = zip(*kv.items())
             m = self.query_by_id(_id, *fields)
             if m:
                 self.__dict__.update(m)
                 return self
             else:
                 msg = "Exec func 'mysqlx.orm.Model.%s' load none, Class: '%s', %s=%d." % ('load', self.__class__.__name__, self._get_pk(), _id)
-                logging.error(msg)
+                logger.error(msg)
                 raise DBError(msg)
         else:
             raise KeyError("Not primary key.")
 
-    def delete(self):
+    def logical_delete(self):
         """
         Logic delete only update the del flag
         user = User(id=1)
-        rowcount = user.delete()
+        rowcount = user.logical_delete()
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('delete', self.__class__.__name__))
+        orm_inst_log('logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
 
-        return self.delete_by_id(_id, update_by)
+        return self.logical_delete_by_id(_id, update_by)
 
-    def un_delete(self):
+    def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         user = User(id=1)
-        rowcount = user.un_delete()
+        rowcount = user.un_logical_delete()
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('un_delete', self.__class__.__name__))
+        orm_inst_log('un_logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
+        return self.un_logical_delete_by_id(_id, update_by)
 
-        return self.un_delete_by_id(_id, update_by)
-
-    def physical_delete(self):
+    def delete(self):
         """
         Physical delete
         user = User(id=1)
-        rowcount = user.physical_delete()
+        rowcount = user.delete()
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('physical_delete', self.__class__.__name__))
+        orm_inst_log('delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
-
-        return self.physical_delete_by_id(_id)
+        return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = User.insert(name='张三', age=20)
         return: Effect rowcount
         """
-        _insert_log('insert', cls.__name__, **kwargs)
-        table = cls._get_table()
-        return db.insert(table, **kwargs)
+        orm_insert_log('insert', cls.__name__, **kwargs)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
+            kwargs[pk] = get_id()
+        return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = User.save(name='张三', age=20)
         :return: Primary key
         """
-        _insert_log('save', cls.__name__, **kwargs)
-        table = cls._get_table()
-        return db.save(table, **kwargs)
+        orm_insert_log('save', cls.__name__, **kwargs)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE:
+            if pk in kwargs:
+                _id = kwargs[pk]
+            else:
+                _id = get_id()
+                kwargs[pk] = _id
+            insert(table, **kwargs)
+        else:
+            _id = save(table, **kwargs)
+        return _id
 
     @classmethod
-    def update_by_id(cls, _id: int, **kwargs):
+    def create(cls, **kwargs):
+        """
+        user = User.create(name='张三', age=20)
+        :return: Instance object
+        """
+        orm_insert_log('create', cls.__name__, **kwargs)
+        pk = cls._get_pk()
+        _id = cls.save(**kwargs)
+        if pk not in kwargs:
+            kwargs[pk] = _id
+        return cls._dict2obj(kwargs)
+
+    @classmethod
+    def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = User.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
         pk = cls._get_pk()
         where = '`%s`=?' % pk
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
-        return db.do_execute(sql, *args, _id, LIMIT_1)
+        return do_execute(sql, *args, _id, LIMIT_1)
 
     @classmethod
-    def delete_by_id(cls, _id: int, update_by: int = None):
+    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = User.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        _delete_by_id_log('delete_by_id', cls.__name__, _id, update_by)
-        return cls._delete_by_id_op(_id, update_by, DelFlag.DELETED)
+        orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
-    def un_delete_by_id(cls, _id: int, update_by: int = None):
+    def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
-        rowcount = User.un_delete_by_id(id=1, update_by=100)
+        rowcount = User.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        _delete_by_id_log('un_delete_by_id', cls.__name__, _id, update_by)
-        return cls._delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
+        orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
-    def delete_by_ids(cls, ids: Sequence[int], update_by: int = None, batch_size=128):
+    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
-        rowcount = User.delete_by_ids(id=[1,2], update_by=100)
+        rowcount = User.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
-            'delete_by_ids', cls.__name__, ids, update_by, batch_size))
-        return cls._delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+            'logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
-    def un_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, batch_size=128):
+    def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
-        rowcount = User.un_delete_by_ids(id=[1,2], update_by=100)
+        rowcount = User.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
-            'un_delete_by_ids', cls.__name__, ids, update_by, batch_size))
-        return cls._delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+            'un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
-    def physical_delete_by(cls, where: str, *args):
+    def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
-        rowcount = User.physical_delete_by('where name=? and age=?', '张三', 55)
+        rowcount = User.delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM `%s` %s' % (table, where)
-        return db.do_execute(sql, *args)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_execute(sql, *args)
 
     @classmethod
-    def physical_delete_by_id(cls, _id: int):
+    def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
-        rowcount = User.physical_delete_by_id(id=1)
+        rowcount = User.delete_by_id(id=1)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('physical_delete_by_id', cls.__name__, _id))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
-        return db.do_execute(sql, _id, LIMIT_1)
+        return do_execute(sql, _id, LIMIT_1)
 
     @classmethod
-    def physical_delete_by_ids(cls, ids: Sequence[int], batch_size=128):
+    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Physical delete
-        rowcount = User.physical_delete_by_ids(id=[1,2])
+        rowcount = User.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, batch_size: %s" % (
-            'physical_delete_by_ids', cls.__name__, ids, batch_size))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, batch_size: %s" % (
+            'delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
-            return cls.physical_delete_by_id(ids[0])
+            return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
-            return cls._physical_delete_by_ids(ids)
+            return cls._delete_by_ids(ids)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with db.transaction():
-                results = list(map(cls._physical_delete_by_ids, split_ids))
+            with transaction():
+                results = list(map(cls._delete_by_ids, split_ids))
             return sum(results)
 
     @classmethod
-    def batch_insert(cls, args: Sequence[Mapping[str, Any]]):
+    def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = User.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
-        table = cls._get_table()
-        return db.batch_insert(table, args)
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
+        assert len(args) > 0, 'args must not be empty.'
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE:
+            for arg in args:
+                if pk not in arg:
+                    arg[pk] = get_id()
+
+        return batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = User.count(name='张三', age=55)
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('count', cls.__name__, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('count', cls.__name__, kwargs))
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
-        sql = cls._select_sql(where, LIMIT_1, fields)
-        return db.do_get(sql, *args, LIMIT_1)
+        sql = _select_sql(table, where, LIMIT_1, fields)
+        return do_get_with_limit(sql, *args, LIMIT_1)
 
     @classmethod
-    def count_by(cls, where: str, *args):
+    def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
-        sql = "SELECT count(1) FROM `%s` %s" % (table, where)
-        return db.do_get(sql, *args)
+        sql = "SELECT count(1) FROM `{}` {}".format(table, where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_get(sql, *args)
+
+    @classmethod
+    def exists(cls, **kwargs):
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('exists', cls.__name__, kwargs))
+        return cls.count(**kwargs) > 0
+
+    @classmethod
+    def exists_by(cls, where: str, *args, **kwargs):
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        return cls.count_by(where, *args, **kwargs) > 0
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('find', cls.__name__, fields, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('find', cls.__name__, fields, kwargs))
         return [cls._dict2obj(d) for d in cls.query(*fields, **kwargs)]
 
     @classmethod
-    def find_by(cls, where: str, *args):
+    def find_one(cls, *fields, **kwargs):
+        """
+        Return unique result(object) or None if no result.
+        user = User.find_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('find_one', cls.__name__, fields, kwargs))
+        result = cls.query_one(*fields, **kwargs)
+        return cls._dict2obj(result) if result else None
+
+    @classmethod
+    def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        return [cls._dict2obj(d) for d in cls.query_by(where, *args)]
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        _page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls._dict2obj(d) for d in result]
 
     @classmethod
-    def find_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        return [cls._dict2obj(d) for d in cls.query_by_page(page_num, page_size, where, *args)]
+        orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
-    def find_by_id(cls, _id: int, *fields):
+    def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         user = User.find_by_id(1, 'id', 'name', 'age')
         :param _id: pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('find_by_id', cls.__name__, _id, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('find_by_id', cls.__name__, _id, fields))
         result = cls.query_by_id(_id, *fields)
         return cls._dict2obj(result) if result else None
 
     @classmethod
-    def find_by_ids(cls, ids: Sequence[int], *fields):
+    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(class object) or empty list if no result.
         users = User.find_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('find_by_ids', cls.__name__, ids, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('find_by_ids', cls.__name__, ids, fields))
         return [cls._dict2obj(d) for d in cls.query_by_ids(ids, *fields)]
 
     @classmethod
     def query(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('query', cls.__name__, fields, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('query', cls.__name__, fields, kwargs))
         where, args, limit = _get_where_arg_limit(**kwargs)
-        if not limit:
-            limit = 1000
+        table = cls._get_table()
+        sql = _select_sql(table, where, limit, *fields)
+        if limit:
+            if isinstance(limit, int):
+                args = [*args, limit]
+            else:
+                args = [*args, *limit]
+        return do_query(sql, *args)
 
-        sql = cls._select_sql(where, limit, *fields)
-        return db.do_query(sql, *args, limit) if limit else db.do_query(sql, *args)
+    @classmethod
+    def query_one(cls, *fields, **kwargs):
+        """
+        Return unique result(dict) or None if no result.
+        users = User.query_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('query_one', cls.__name__, fields, kwargs))
+        where, args, _ = _get_where_arg_limit(**kwargs)
+        table = cls._get_table()
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_query_one_with_limit(sql, *args, LIMIT_1)
 
     @classmethod
-    def query_by(cls, where: str, *args):
+    def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_query(sql, *args)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        _page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = cls._select_sql(where, NO_LIMIT, *fields)
-        return db.do_query_page(sql, page_num, page_size, *args)
+        sql = _select_sql(table, where, NO_LIMIT, *fields)
+        return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def query_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.query_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_query_page(sql, page_num, page_size, *args)
+        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def query_by_id(cls, _id: int, *fields):
+    def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         user = User.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
-        pk = cls._get_pk()
-        where = 'WHERE `%s`=?' % pk
-        sql = cls._select_sql(where, LIMIT_1, *fields)
-        return db.do_query_one(sql, _id, LIMIT_1)
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}`=?'.format(pk)
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_query_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
-    def query_by_ids(cls, ids: Sequence[int], *fields):
+    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         users = User.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('query_by_ids', cls.__name__, ids, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('query_by_ids', cls.__name__, ids, fields))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk = cls._get_pk()
-        where = 'WHERE `%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-        sql = cls._select_sql(where, ids_size, *fields)
-        return db.do_query(sql, *ids, ids_size)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        sql = _select_sql(table, where, ids_size, *fields)
+        return do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('select', cls.__name__, fields, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('select', cls.__name__, fields, kwargs))
         where, args, limit = _get_where_arg_limit(**kwargs)
-        if not limit:
-            limit = 1000
+        table = cls._get_table()
+        sql = _select_sql(table, where, limit, *fields)
+        if limit:
+            if isinstance(limit, int):
+                args = [*args, limit]
+            else:
+                args = [*args, *limit]
+        return do_select(sql, *args)
 
-        sql = cls._select_sql(where, limit, *fields)
-        return db.do_select(sql, *args, limit) if limit else db.do_select(sql, *args)
+    @classmethod
+    def select_one(cls, *fields, **kwargs):
+        """
+        Return unique result(tuple) or None if no result.
+        row = User.select_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('select_one', cls.__name__, fields, kwargs))
+        where, args, _ = _get_where_arg_limit(**kwargs)
+        table = cls._get_table()
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_select_one_with_limit(sql, *args, LIMIT_1)
 
     @classmethod
-    def select_by(cls, where: str, *args):
+    def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_select(sql, *args)
+        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        _page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = cls._select_sql(where, NO_LIMIT, *fields)
-        return db.do_select_page(sql, page_num, page_size, *args)
+        sql = _select_sql(table, where, NO_LIMIT, *fields)
+        return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def select_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.select_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_select_page(sql, page_num, page_size, *args)
+        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def select_by_id(cls, _id: int, *fields):
+    def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = User.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
-        pk = cls._get_pk()
-        where = 'WHERE `%s`=?' % pk
-        sql = cls._select_sql(where, LIMIT_1, *fields)
-        return db.do_select_one(sql, _id, LIMIT_1)
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}`=?'.format(pk)
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_select_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
-    def select_by_ids(cls, ids: Sequence[int], *fields):
+    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('select_by_ids', cls.__name__, ids, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('select_by_ids', cls.__name__, ids, fields))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk = cls._get_pk()
-        where = 'WHERE `%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-        sql = cls._select_sql(where, ids_size, *fields)
-        return db.do_select(sql, *ids, ids_size)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        sql = _select_sql(table, where, ids_size, *fields)
+        return do_select(sql, *ids, ids_size)
 
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
-    def _delete_by_id_op(cls, _id: int, update_by: int = None, del_status=DelFlag.DELETED):
+    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         pk, table = cls._get_pk_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s`=?' % pk
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
-            return db.do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
+                return do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
+            return do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
-            return db.do_execute(sql, del_status.value, _id, LIMIT_1)
+                return do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
+            return do_execute(sql, del_status.value, _id, LIMIT_1)
 
     @classmethod
-    def _delete_by_ids_op(cls, ids: Sequence[int], update_by: int = None, batch_size=128, del_status=DelFlag.DELETED):
+    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
+            del_status=DelFlag.DELETED):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
-            return cls._delete_by_id_op(ids[0], update_by, del_status)
+            return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
         elif ids_size <= batch_size:
-            return cls._do_delete_by_ids(ids, update_by, del_status)
+            return cls._do_logical_delete_by_ids(ids, update_by, del_status)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with db.transaction():
-                results = [cls._do_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
+            with transaction():
+                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
             return sum(results)
 
     @classmethod
-    def _do_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, del_status=DelFlag.DELETED):
+    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         pk = cls._get_pk()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
-            return db.do_execute(sql, del_status.value, update_by, *ids, ids_size)
+                return do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
+            return do_execute(sql, del_status.value, update_by, *ids, ids_size)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
-            return db.do_execute(sql, del_status.value, *ids, ids_size)
+                return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
+            return do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
-    def _physical_delete_by_ids(cls, ids: Sequence[int]):
+    def _delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         ids_size = len(ids)
         pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit ?' % (table, pk, ','.join(['?' for _ in range(ids_size)]))
-        return db.do_execute(sql, *ids, ids_size)
+        sql = 'DELETE FROM `{}` WHERE `{}` in ({}) limit ?'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
+        return do_execute(sql, *ids, ids_size)
 
     @classmethod
     def _get_pk(cls):
         if hasattr(cls, PK):
             return cls.__pk__
-        logging.warning("%s not set attribute '%s'" % (cls.__name__, PK))
+        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
         return DEFAULT_PK_FIELD
 
     @classmethod
     def _get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
-        logging.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
+        logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
         return _get_table_name(cls.__name__)
 
     @classmethod
     def _get_pk_and_table(cls):
         return cls._get_pk(), cls._get_table()
 
     @classmethod
+    def _get_pk_strategy(cls):
+        if hasattr(cls, PK_STRATEGY):
+            return cls.__pk_strategy__
+        return None
+
+    @classmethod
     def _dict2obj(cls, dictionary):
         m = cls.__new__(cls)
-        m.__init__(**dictionary)
+        m.__dict__.update(dictionary)
         return m
 
     @classmethod
     def _get_update_by_field(cls):
         if hasattr(cls, UPDATE_BY):
             return cls.__update_by__
         return None
@@ -639,97 +768,130 @@
 
     @classmethod
     def _get_del_flag_field(cls):
         assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
         return cls.__del_flag__
 
     @classmethod
-    def _select_sql(cls, where, limit, *fields):
-        table = cls._get_table()
-        if not fields:
-            fields = '*'
-        else:
-            fields = ','.join(['%s' % col if '(' in col else '`%s`' % col for col in fields])
-
-        if limit:
-            return 'SELECT %s FROM `%s` %s limit ?' % (fields, table, where)
-        else:
-            return 'SELECT %s FROM `%s` %s' % (fields, table, where)
-
-    @classmethod
     def _update_sql(cls, where, *update_fields):
         update_time_arg = None
         table = cls._get_table()
         update_time_field = cls._get_update_time_field()
         if update_time_field is not None and update_time_field not in update_fields:
             update_fields = [*update_fields, update_time_field]
             update_time_arg = datetime.now()
 
-        update_fields = ','.join(['`%s`=?' % col for col in update_fields])
-        return 'UPDATE `%s` SET %s WHERE %s limit ?' % (table, update_fields, where), update_time_arg
+        update_fields = ','.join(['`{}`=?'.format(col) for col in update_fields])
+        return 'UPDATE `{}` SET {} WHERE {} limit ?'.format(table, update_fields, where), update_time_arg
+
+    @classmethod
+    def _where_sql(cls, where: str):
+        low_where = where.lower()
+        if low_where.startswith('where'):
+            table = cls._get_table()
+            return _select_sql(table, where, NO_LIMIT)
+        elif low_where.startswith('select'):
+            return where
+        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
 
 
 # ----------------------------------------------------------Private function------------------------------------------------------------------
-def _get_condition_arg(k, v):
-    if not isinstance(v, str):
-        return "`%s`=?" % k, v
+def _select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
+    if fields:
+        fields = ','.join([col if '(' in col else '`{}`'.format(col) for col in fields])
+    else:
+        fields = _get_table_columns(table)
 
-    v_lower = v.lower()
-    if any([symbol in SYMBOLS for symbol in v_lower]):
-        return "`%s`%s" % (k, v), None
-    elif BETWEEN in v_lower or LIKE in v_lower or IN in v_lower:
-        return "`%s` %s" % (k, v), None
+    if limit:
+        if isinstance(limit, int):
+            return 'SELECT {} FROM `{}` {} limit ?'.format(fields, table, where)
+        elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
+            return 'SELECT {} FROM `{}` {} limit ?,?'.format(fields, table, where)
+        else:
+            raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
-        return "`%s`=?" % k, v
+        return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
+
+
+@lru_cache(maxsize=128)
+def _get_table_columns(table: str):
+    return do_get_with_limit(COLUMN_SQL, table, LIMIT_1)
+
+
+def _delete_by_id_sql(table, pk):
+    return 'DELETE FROM `{}` WHERE `{}`=? limit ?'.format(table, pk)
+
+
+def _get_condition_arg(k: str, v: object):
+    if k.endswith("__eq"):
+        return "`{}`=?".format(k[:-4]), v
+    if k.endswith("__gt"):
+        return "`{}`>?".format(k[:-4]), v
+    if k.endswith("__lt"):
+        return "`{}`<?".format(k[:-4]), v
+    if k.endswith("__ge"):
+        return "`{}`>=?".format(k[:-4]), v
+    if k.endswith("__gte"):
+        return "`{}`>=?".format(k[:-5]), v
+    if k.endswith("__le"):
+        return "`{}`<=?".format(k[:-4]), v
+    if k.endswith("__lte"):
+        return "`{}`<=?".format(k[:-5]), v
+    if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
+        return "`{}` in ({})".format(k[:-4], ','.join(['?' for _ in v])), v
+    if k.endswith("__in"):
+        return "`{}` in ({})".format(k[:-4], '?'), v
+    if k.endswith("__startswith"):
+        return "`{}` like ?".format(k[:-12]), '{}%'.format(v)
+    if k.endswith("__endswith"):
+        return "`{}` like ?".format(k[:-10]), '%{}'.format(v)
+    if k.endswith("__contains"):
+        return "`{}` like ?".format(k[:-10]), '%{}%'.format(v)
+    if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
+        return "`{}` between ? and ?".format(k[:-9]), v
+    if k.endswith("__between"):
+        return ValueError("Must is instance of Sequence with length 2 when use between statement")
+
+    if not isinstance(v, str):
+        return "`{}`=?".format(k), v
+    lower_v = v.lower()
+    if any([symbol in SYMBOLS for symbol in lower_v]):
+        return "`{}`{}".format(k, v), None
+    elif BETWEEN in lower_v or LIKE in lower_v or IN in lower_v:
+        return "`{}` {}".format(k, v), None
+    else:
+        return "`{}`=?".format(k), v
 
 
 def _get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.get('limit')
         del kwargs['limit']
 
     if kwargs:
-        conditions, args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
-        args = [arg for arg in args if arg is not None]
-        where = 'WHERE %s' % ' and '.join(conditions)
+        conditions, tmp_args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
+        tmp_args = [arg for arg in tmp_args if arg is not None]
+
+        for arg in tmp_args:
+            if arg:
+                if isinstance(arg, Sequence) and not isinstance(arg, str):
+                    args.extend(arg)
+                else:
+                    args.append(arg)
+        where = 'WHERE {}'.format(' and '.join(conditions))
 
     return where, args, limit
 
 
 def _split_ids(ids: Sequence[int], batch_size):
     ids_size = len(ids)
-    mod = ids_size % batch_size
     n = ids_size // batch_size
-    if mod != 0:
-        n += 1
-
+    n += 0 if ids_size % batch_size == 0 else 1
     return [ids[i:i + batch_size] for i in range(0, ids_size, batch_size)]
 
 
 def _get_table_name(class_name):
     for i in range(1, len(class_name) - 1)[::-1]:
         if class_name[i].isupper():
             class_name = class_name[:i] + '_' + class_name[i:]
     return class_name.lower()
-
-
-def _page_log(function, page_num, page_size, class_name, where, *args):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s" % (
-        function, page_num, page_size, class_name, where, args))
-
-
-def _by_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', fields: %s, kwargs: %s" % (
-        function, page_num, page_size, class_name, fields, kwargs))
-
-
-def _insert_log(function, class_name, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
-
-
-def _delete_by_id_log(function, class_name, _id, update_by):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
-
-
-def _by_log(function, class_name, where, *args):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s" % (function, class_name, where, args))
```

### Comparing `mysqlx-1.3.1/setup.py` & `mysqlx-1.3.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import os
-from setuptools import setup, find_packages
+from setuptools import setup
 
 # INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
-    with open(os.path.join(here, rel_path)) as fp:
+    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='mysqlx',
-    packages=find_packages(),
-    description="MySqlx is a simple python sql executor for MySQL like iBatis.",
+    packages=['mysqlx'],
+    description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'Jinja2>=3.0.3',
-        'mysql-connector-python>=8.0.20',
+        'Jinja2>=3.0.0',
+        # 'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.1',
+    version='1.3.8',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
-    keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
+    keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.6.0',
+    python_requires='>=3.7.0',
     zip_safe=False
 )
```

