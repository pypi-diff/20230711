# Comparing `tmp/mysqlx-1.3.4.tar.gz` & `tmp/mysqlx-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.4.tar", last modified: Mon Jul  3 02:24:04 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.5.tar", last modified: Mon Jul 10 14:24:14 2023, max compression
```

## Comparing `mysqlx-1.3.4.tar` & `mysqlx-1.3.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 02:24:04.000000 mysqlx-1.3.4/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-03 02:24:04.000000 mysqlx-1.3.4/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.4/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1644 2023-06-26 14:04:23.000000 mysqlx-1.3.4/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    20093 2023-07-02 22:53:10.000000 mysqlx-1.3.4/mysqlx/db.py
--rw-rw-rw-   0        0        0    13200 2023-07-02 03:56:40.000000 mysqlx-1.3.4/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    36949 2023-07-03 02:22:31.000000 mysqlx-1.3.4/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.4/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     3773 2023-07-02 22:43:31.000000 mysqlx-1.3.4/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     7811 2023-06-30 06:21:34.000000 mysqlx-1.3.4/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.4/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 02:24:04.000000 mysqlx-1.3.4/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-03 02:24:03.000000 mysqlx-1.3.4/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.4/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4248 2023-07-03 02:24:03.000000 mysqlx-1.3.4/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-03 02:24:03.000000 mysqlx-1.3.4/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      589 2023-07-03 02:24:04.000000 mysqlx-1.3.4/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 02:24:03.000000 mysqlx-1.3.4/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4248 2023-07-03 02:24:04.000000 mysqlx-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3449 2023-07-02 07:59:31.000000 mysqlx-1.3.4/README.md
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-03 02:24:04.000000 mysqlx-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-03 02:23:05.000000 mysqlx-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 02:24:04.000000 mysqlx-1.3.4/test/
--rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.4/test/all_unit_test.py
--rw-rw-rw-   0        0        0      246 2023-07-02 23:03:01.000000 mysqlx-1.3.4/test/coder_test.py
--rw-rw-rw-   0        0        0     2832 2023-07-02 23:03:01.000000 mysqlx-1.3.4/test/dbx_test.py
--rw-rw-rw-   0        0        0     4925 2023-07-02 23:03:01.000000 mysqlx-1.3.4/test/db_test.py
--rw-rw-rw-   0        0        0      637 2023-07-02 23:03:01.000000 mysqlx-1.3.4/test/mapper_test.py
--rw-rw-rw-   0        0        0     5202 2023-07-01 16:10:46.000000 mysqlx-1.3.4/test/models.py
--rw-rw-rw-   0        0        0     5494 2023-07-03 02:18:22.000000 mysqlx-1.3.4/test/orm_test.py
--rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.4/test/snowflake_test.py
--rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.4/test/time_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.4/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.4/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx/
+-rw-rw-rw-   0        0        0     5819 2023-07-09 01:30:37.000000 mysqlx-1.3.5/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1644 2023-07-10 14:22:09.000000 mysqlx-1.3.5/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    19721 2023-07-10 13:35:46.000000 mysqlx-1.3.5/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13187 2023-07-09 01:26:49.000000 mysqlx-1.3.5/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    39144 2023-07-10 14:13:27.000000 mysqlx-1.3.5/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.5/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4052 2023-07-10 13:42:49.000000 mysqlx-1.3.5/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     7290 2023-07-10 14:05:30.000000 mysqlx-1.3.5/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.5/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4248 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      589 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 14:24:14.000000 mysqlx-1.3.5/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4248 2023-07-10 14:24:14.000000 mysqlx-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3449 2023-07-02 07:59:31.000000 mysqlx-1.3.5/README.md
+-rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:24:14.000000 mysqlx-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-10 14:23:24.000000 mysqlx-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:24:14.000000 mysqlx-1.3.5/test/
+-rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.5/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      246 2023-07-02 23:03:01.000000 mysqlx-1.3.5/test/coder_test.py
+-rw-rw-rw-   0        0        0     2832 2023-07-02 23:03:01.000000 mysqlx-1.3.5/test/dbx_test.py
+-rw-rw-rw-   0        0        0     4934 2023-07-10 13:36:04.000000 mysqlx-1.3.5/test/db_test.py
+-rw-rw-rw-   0        0        0      642 2023-07-08 17:06:12.000000 mysqlx-1.3.5/test/mapper_test.py
+-rw-rw-rw-   0        0        0     1432 2023-07-10 14:22:09.000000 mysqlx-1.3.5/test/models.py
+-rw-rw-rw-   0        0        0     5494 2023-07-03 02:33:32.000000 mysqlx-1.3.5/test/orm_test.py
+-rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.5/test/snowflake_test.py
+-rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.5/test/time_test.py
+-rw-rw-rw-   0        0        0      575 2023-07-09 02:11:45.000000 mysqlx-1.3.5/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.5/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.5/test/__init__.py
```

### Comparing `mysqlx-1.3.4/LICENSE` & `mysqlx-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/mysqlx/coder.py` & `mysqlx-1.3.5/mysqlx/coder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 
 class Coder:
     comma1 = ','
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
-     WHERE table_schema = (SELECT DATABASE())
-       AND table_name = ? 
+     WHERE table_schema = (SELECT DATABASE()) AND table_name = ? 
     '''
 
     def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, use_unicode=True, pool_size=1, show_sql=False,
             **kwargs):
         db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
```

### Comparing `mysqlx-1.3.4/mysqlx/coder.tpl` & `mysqlx-1.3.5/mysqlx/coder.tpl`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from decimal import Decimal
 from datetime import date, datetime
 from mysqlx.orm import Model, PkStrategy
 
 
 class BaseModel(Model):
     __pk__ = '{{__pk__}}'
+    __del_flag__ = '{{__del_flag__}}'
     __update_by__ = '{{__update_by__}}'
     __update_time__ = '{{__update_time__}}'
-    __del_flag__ = '{{__del_flag__}}'
     __pk_strategy__ = PkStrategy.DB.value
 
     def __init__(self,{% for item in base_columns %}{% if loop.last %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %}{% else %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %},{% endif %}{% endfor %}): {% for item in base_columns %}
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% for meta in metas %}
 class {{meta.class_name}}(BaseModel):{% if meta.pk != __pk__ %}
```

### Comparing `mysqlx-1.3.4/mysqlx/db.py` & `mysqlx-1.3.5/mysqlx/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import logging
 import functools
 from typing import Sequence
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, log, get_named_sql, get_named_args, \
-    page_log, LIMIT_1, DBError, DB_LOCK, get_batch_args
+    page_log, LIMIT_1, DBError, DB_LOCK, get_batch_args, logger
 
 _DB_CTX = None
 _SHOW_SQL = False
 _MAPPER_PATH = "mapper_path"
 _PK_SQL = 'SELECT LAST_INSERT_ID()'
 
 
@@ -19,20 +18,17 @@
         from pymysql import connect
 
     global _DB_CTX
     global _SHOW_SQL
 
     if 'debug' in kwargs:
         if kwargs['debug']:
-            logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-        else:
-            logging.basicConfig(level=logging.INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+            from logging import DEBUG
+            logger.setLevel(DEBUG)
         del kwargs['debug']
-    else:
-        logging.basicConfig(level=logging.INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
     is_pool = use_mysql_connector and pool_size >= 1
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _SHOW_SQL = show_sql
         if _MAPPER_PATH in kwargs:
@@ -47,17 +43,17 @@
         kwargs['password'] = password
         kwargs['database'] = database
         kwargs['host'] = host
         kwargs['port'] = port
         kwargs['use_unicode'] = use_unicode
         _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
     if is_pool:
-        logging.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
+        logger.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
-        logging.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
+        logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
@@ -121,27 +117,27 @@
 def insert(table: str, **kwargs):
     """
     Execute insert SQL, return effect rowcount.
     :param table: table name
     :param kwargs: name='张三', age=20}
     return: Effect rowcount
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('insert', table, kwargs))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('insert', table, kwargs))
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
 def save(table: str, **kwargs):
     """
     Execute insert SQL, return primary key.
     :param table: table
     :param kwargs: name='张三', age=20
     :return: Primary key
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_save(sql, *args)
 
 
 @with_connection
 def do_save(sql: str, *args):
     """
@@ -179,29 +175,29 @@
 def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', args: %s" % ('batch_insert', table, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', args: %s" % ('batch_insert', table, args))
     assert len(args) > 0, 'args must not be empty.'
     sql, args = _batch_insert_sql_args(table, *args)
     return batch_execute(sql, *args)
 
 
 def batch_execute(sql: str, *args):
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
         sql, args = _batch_named_sql_args(sql, *args)
 
     return do_batch_execute(sql, *args)
 
 
@@ -335,32 +331,32 @@
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get', sql, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get', sql, args))
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_get_limit(sql, *args)
+    return do_get_with_limit(sql, *args)
 
 
-def do_get_limit(sql: str, *args):
+def do_get_with_limit(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get_limit', sql, args))
-    result = do_select_one_limit(sql, *args)
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get_with_limit', sql, args))
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
@@ -369,54 +365,53 @@
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_query', sql.strip(), *args)
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
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_query_one', sql, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_query_one', sql, args))
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_query_one_limit(sql, *args)
+    return do_query_one_with_limit(sql, *args)
 
 
 @with_connection
-def do_query_one_limit(sql: str, *args):
+def do_query_one_with_limit(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql, args = _limit_one_sql_args(sql, *args)
-    sql = _before_execute('do_query_one_limit', sql.strip(), *args)
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
@@ -437,28 +432,28 @@
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_select_one', sql, args))
+    logger.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_select_one', sql, args))
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_select_one_limit(sql, *args)
+    return do_select_one_with_limit(sql, *args)
 
 
 @with_connection
-def do_select_one_limit(sql: str, *args):
+def do_select_one_with_limit(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_select_one_limit', sql.strip(), *args)
+    sql = _before_execute('do_select_one_with_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
@@ -495,15 +490,15 @@
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
@@ -554,9 +549,9 @@
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
 
     return False
 
 
 def _do_page_log(function: str, sql: str, page_num, page_size, *args):
-    logging.debug(
+    logger.debug(
         "Exec func 'mysqlx.db.%s', page_num: %d, page_size: %d \n\t\t sql: %s \n\t\t args: %s" % (function, page_num, page_size, sql.strip(), args))
```

### Comparing `mysqlx-1.3.4/mysqlx/dbx.py` & `mysqlx-1.3.5/mysqlx/dbx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import re
-import logging
-from jinja2 import Template
 from typing import Mapping
-from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction
+from jinja2 import Template
+from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction, logger
 from .db import do_get, do_query, do_query_one, do_execute, do_select_page, do_select, do_select_one, do_query_page, init_db as _init_db, \
     get_connection as _get_connection, insert as _insert, save as _save, batch_insert as _batch_insert, batch_execute as _batch_execute
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
@@ -175,22 +174,22 @@
     :param param_names: original function parameter names
     :param args:
     :param kwargs:
     :return:
     """
     if sql_model.dynamic:
         sql = sql_model.sql.render(**kwargs)
-        logging.debug("Original sql: {}".format(sql))
+        logger.debug("Original sql: {}".format(sql))
         return get_named_sql_args(sql, **kwargs)
     else:
-        logging.debug("Original sql: {}".format(sql_model.sql))
+        logger.debug("Original sql: {}".format(sql_model.sql))
         if sql_model.mapping and kwargs:
             return get_named_sql_args(sql_model.sql, **kwargs)
         elif sql_model.placeholder and kwargs:
-            logging.warning("Better use 'func(arg1, arg2...)' then 'func(arg1=arg1, arg2=arg2...)' if sql contain '?' placeholder.")
+            logger.warning("Better use 'func(arg1, arg2...)' then 'func(arg1=arg1, arg2=arg2...)' if sql contain '?' placeholder.")
             args = [kwargs[name] for name in param_names if name in kwargs] if param_names else list(kwargs.values())
         elif sql_model.mapping and not kwargs and (not batch or
                                                    (batch and (not args or not isinstance(args[0], Mapping)))):  # batch_execute时args可能为List[Mapping]
             raise MapperError("Parameter 'kwargs' must not be empty when named mapping sql.")
         return sql_model.sql, args
 
 
@@ -292,17 +291,17 @@
         _valid_sql(sql_id, sql, child.tag)
         _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace)
 
     return _id, includes
 
 
 def _sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
+    logger.debug("Exec func 'mysqlx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
 
 
 def _page_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (
+    logger.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (
         function, page_num, page_size, sql_id.strip(), args, kwargs))
 
 
 def _valid_sql(sql_id, sql, tag):
     assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `mysqlx-1.3.4/mysqlx/orm.py` & `mysqlx-1.3.5/mysqlx/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import sys
-import logging
-from enum import IntEnum
-from typing import Sequence, Union, List, Tuple
-from .snowflake import get_id
 from datetime import datetime
+from .snowflake import get_id
+from enum import Enum, IntEnum
 from functools import lru_cache
-from .support import LIMIT_1, DBError, PkStrategy, simple_sql
-from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
-    do_query_page, do_select_page, do_get
+from typing import Sequence, Union, List, Tuple
+from .support import LIMIT_1, DBError, simple_sql, logger
+from .db import do_get_with_limit, do_query, do_query_one_with_limit, do_execute, insert, save, do_select, do_select_one_with_limit, transaction,\
+    batch_insert, do_query_page, do_select_page, do_get
 
 NO_LIMIT = 0
 DEFAULT_PK_FIELD = 'id'
 SYMBOLS = ['=', '>', '<']
 BETWEEN, LIKE, IN = 'between', 'like', 'in'
 PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__', '__pk_strategy__'
 _COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
@@ -19,14 +18,29 @@
 
 
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
     Create a class extends Model:
 
     class User(Model):
         __pk__ = 'id'
         __table__ = 'user'
@@ -66,112 +80,112 @@
 
     def persist(self):
         """
         user = User(name='张三', age=55)
         effect_rowcount = user.persist()
         :return: effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('persist', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('persist', self.__class__.__name__))
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         return self.insert(**kv)
 
     def inst_save(self):
         """
         user = User(name='张三', age=55)
         id = user.save()
         :return: Primary key
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('inst_save', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('inst_save', self.__class__.__name__))
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
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('update', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('update', self.__class__.__name__))
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
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         user = User(id=1)
         rowcount = user.logical_delete()
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('logical_delete', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('logical_delete', self.__class__.__name__))
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
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('un_logical_delete', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('un_logical_delete', self.__class__.__name__))
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
-        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('delete', self.__class__.__name__))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('delete', self.__class__.__name__))
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
@@ -180,28 +194,28 @@
         """
         rowcount = User.insert(name='张三', age=20)
         return: Effect rowcount
         """
         _insert_log('insert', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE.value and pk not in kwargs:
+        if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
             kwargs[pk] = get_id()
         return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = User.save(name='张三', age=20)
         :return: Primary key
         """
         _insert_log('save', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE.value:
+        if pk_strategy == PkStrategy.SNOWFLAKE:
             if pk in kwargs:
                 _id = kwargs[pk]
             else:
                 _id = get_id()
                 kwargs[pk] = _id
             insert(table, **kwargs)
         else:
@@ -218,68 +232,68 @@
         pk = cls._get_pk()
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
         return cls._dict2obj(kwargs)
 
     @classmethod
-    def update_by_id(cls, _id: int, **kwargs):
+    def update_by_id(cls, _id, **kwargs):
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
         return do_execute(sql, *args, _id, LIMIT_1)
 
     @classmethod
-    def logical_delete_by_id(cls, _id: int, update_by: int = None):
+    def logical_delete_by_id(cls, _id, update_by=None):
         """
         Logic delete only update the del flag
         rowcount = User.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         _delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_id(cls, _id: int, update_by: int = None):
+    def un_logical_delete_by_id(cls, _id, update_by=None):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         _delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
-    def logical_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, batch_size=128):
+    def logical_delete_by_ids(cls, ids: Sequence, update_by=None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
             'logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, batch_size=128):
+    def un_logical_delete_by_ids(cls, ids: Sequence, update_by=None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
             'un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size))
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
@@ -290,33 +304,33 @@
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM `%s` %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_execute(sql, *args)
 
     @classmethod
-    def delete_by_id(cls, _id: int):
+    def delete_by_id(cls, _id):
         """
         Physical delete
         rowcount = User.delete_by_id(id=1)
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
         return do_execute(sql, _id, LIMIT_1)
 
     @classmethod
     def delete_by_ids(cls, ids: Sequence[int], batch_size=128):
         """
         Physical delete
         rowcount = User.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, batch_size: %s" % (
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, batch_size: %s" % (
             'delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
             return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
@@ -331,37 +345,37 @@
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = User.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE.value:
+        if pk_strategy == PkStrategy.SNOWFLAKE:
             for arg in args:
                 if pk not in arg:
                     arg[pk] = get_id()
 
         return batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = User.count(name='张三', age=55)
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('count', cls.__name__, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('count', cls.__name__, kwargs))
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
         sql = _select_sql(table, where, LIMIT_1, fields)
-        return do_get_limit(sql, *args, LIMIT_1)
+        return do_get_with_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
@@ -370,33 +384,44 @@
         table = cls._get_table()
         sql = "SELECT count(1) FROM `{}` {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('exists', cls.__name__, kwargs))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('exists', cls.__name__, kwargs))
         return cls.count(**kwargs) > 0
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
         _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return cls.count_by(where, *args, **kwargs) > 0
 
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
     def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
         _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
@@ -404,15 +429,15 @@
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
         _page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls._dict2obj(d) for d in result]
 
     @classmethod
     def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
@@ -420,55 +445,68 @@
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
         _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
-    def find_by_id(cls, _id: int, *fields):
+    def find_by_id(cls, _id, *fields):
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
+    def find_by_ids(cls, ids: Sequence, *fields):
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
         table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_query(sql, *args)
 
     @classmethod
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
+
+    @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
         _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
@@ -478,15 +516,15 @@
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
         _page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_query_page(sql, page_num, page_size, *args)
 
@@ -498,63 +536,76 @@
         """
         _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def query_by_id(cls, _id: int, *fields):
+    def query_by_id(cls, _id, *fields):
         """
         Return one row(dict) or None if no result.
         user = User.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_query_one_limit(sql, _id, LIMIT_1)
+        return do_query_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Sequence[int], *fields):
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
 
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_query(sql, *ids, ids_size)
 
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
         table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_select(sql, *args)
 
     @classmethod
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
+
+    @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
         _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
@@ -564,15 +615,15 @@
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
         _page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_select_page(sql, page_num, page_size, *args)
 
@@ -584,47 +635,47 @@
         """
         _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def select_by_id(cls, _id: int, *fields):
+    def select_by_id(cls, _id, *fields):
         """
         Return one row(dict) or None if no result.
         row = User.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
-        :param fields: Default select all fields with 'select *' if not set
+        :param fields: Default select all fields if not set
         """
-        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
+        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_select_one_limit(sql, _id, LIMIT_1)
+        return do_select_one_with_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Sequence[int], *fields):
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
 
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_select(sql, *ids, ids_size)
 
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
-    def _logical_delete_by_id_op(cls, _id: int, update_by: int = None, del_status=DelFlag.DELETED):
+    def _logical_delete_by_id_op(cls, _id, update_by=None, del_status=DelFlag.DELETED):
         pk, table = cls._get_pk_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s`=?' % pk
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
@@ -634,30 +685,30 @@
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
             return do_execute(sql, del_status.value, _id, LIMIT_1)
 
     @classmethod
-    def _logical_delete_by_ids_op(cls, ids: Sequence[int], update_by: int = None, batch_size=128, del_status=DelFlag.DELETED):
+    def _logical_delete_by_ids_op(cls, ids: Sequence[int], update_by=None, batch_size=128, del_status=DelFlag.DELETED):
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
-    def _do_logical_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, del_status=DelFlag.DELETED):
+    def _do_logical_delete_by_ids(cls, ids: Sequence, update_by=None, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         pk = cls._get_pk()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
         if update_by is not None and update_by_field is not None:
@@ -668,32 +719,32 @@
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
             return do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
-    def _delete_by_ids(cls, ids: Sequence[int]):
+    def _delete_by_ids(cls, ids: Sequence):
         ids_size = len(ids)
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `{}` WHERE `{}` in ({}) limit ?'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
         return do_execute(sql, *ids, ids_size)
 
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
@@ -764,15 +815,15 @@
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
 
 
 @lru_cache(maxsize=128)
 def _get_table_columns(table: str):
-    return do_get_limit(_COLUMN_SQL, table, LIMIT_1)
+    return do_get_with_limit(_COLUMN_SQL, table, LIMIT_1)
 
 
 def _delete_by_id_sql(table, pk):
     return 'DELETE FROM `{}` WHERE `{}`=? limit ?'.format(table, pk)
 
 
 def _get_condition_arg(k: str, v: object):
@@ -848,26 +899,26 @@
     for i in range(1, len(class_name) - 1)[::-1]:
         if class_name[i].isupper():
             class_name = class_name[:i] + '_' + class_name[i:]
     return class_name.lower()
 
 
 def _by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
+    logger.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
         function, page_num, page_size, class_name, where, args, kwargs))
 
 
 def _page_log(function, page_num, page_size, class_name, *fields, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', fields: %s, kwargs: %s" % (
+    logger.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', fields: %s, kwargs: %s" % (
         function, page_num, page_size, class_name, fields, kwargs))
 
 
 def _insert_log(function, class_name, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
+    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def _delete_by_id_log(function, class_name, _id, update_by):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
+    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
 
 
 def _by_log(function, class_name, where, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
+    logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
```

### Comparing `mysqlx-1.3.4/mysqlx/snowflake.py` & `mysqlx-1.3.5/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/mysqlx/sql_mapper.py` & `mysqlx-1.3.5/mysqlx/sql_mapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
-import logging
 import functools
-from .support import SqlAction, get_named_sql_args, simple_sql
 from .dbx import get_sql_model, do_get_sql, build_sql_id
+from .support import SqlAction, get_named_sql_args, simple_sql, logger, MapperError
 from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute, do_save
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
@@ -14,17 +13,19 @@
         def _wrapper(*args, **kwargs):
             param_names = func.__code__.co_varnames
             full_sql_id, func_name = _before(func, namespace, sql_id, *args, **kwargs)
             sql_model = get_sql_model(full_sql_id)
             exec_func = _get_exec_func(func, sql_model.action, batch, return_pk)
             if not batch:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
+                if return_pk and SqlAction.INSERT.value not in use_sql.lower():
+                    raise MapperError("Only insert sql can return primary key.")
             else:
                 if kwargs:
-                    logging.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
+                    logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             return exec_func(use_sql, *args)
 
         return _wrapper
     return _decorator
 
@@ -39,14 +40,15 @@
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return batch_execute(use_sql, *args)
                 if kwargs:
                     use_sql, args = get_named_sql_args(**kwargs)
                 if return_pk:
+                    assert SqlAction.INSERT.value in use_sql.lower(), 'Only insert sql can return primary key.'
                     return do_save(use_sql, *args)
                 return do_execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = _get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
@@ -86,9 +88,9 @@
 
 def _before(func, namespace, _id, *args, **kwargs):
     file_name = os.path.basename(func.__code__.co_filename)[:-3]
     _namespace = namespace if namespace else file_name
     _id = _id if _id else func.__name__
     sql_id = build_sql_id(_namespace, _id)
     func_name = file_name + '.' + func.__name__
-    logging.debug("Exec mapper func: '%s', sql_id: '%s', args: %s, kwargs: %s" % (func_name, sql_id, args, kwargs))
+    logger.debug("Exec mapper func: '%s', sql_id: '%s', args: %s, kwargs: %s" % (func_name, sql_id, args, kwargs))
     return sql_id, func_name
```

### Comparing `mysqlx-1.3.4/mysqlx/support.py` & `mysqlx-1.3.5/mysqlx/support.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import re
-import logging
 import threading
 from enum import Enum
 from typing import Sequence
 from jinja2 import Template
 from functools import lru_cache
+from logging import basicConfig, INFO, getLogger
 
 LIMIT_1 = 1
 _REGEX = r':[\w|\d]*'
 DYNAMIC_REGEX = '{%|{{|}}|%}'
 DB_LOCK = threading.RLock()
+logger = getLogger(__name__)
+basicConfig(level=INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def try_commit(db_ctx):
     if db_ctx.transactions == 0:
-        logging.debug('Commit transaction...')
+        logger.debug('Commit transaction...')
         try:
             db_ctx.connection.commit()
-            logging.debug('Commit ok.')
+            logger.debug('Commit ok.')
         except Exception:
-            logging.warning('Commit failed, try rollback...')
+            logger.warning('Commit failed, try rollback...')
             db_ctx.connection.rollback()
-            logging.warning('Rollback ok.')
+            logger.warning('Rollback ok.')
             raise
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
@@ -62,19 +64,19 @@
 
 
 def get_named_args(sql: str, **kwargs):
     return [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
 
 
 def log(function: str, sql: str, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s' \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+    logger.debug("Exec func 'mysqlx.%s' \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (function, sql.strip(), args, kwargs))
 
 
 def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (
+    logger.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (
         function, page_num, page_size, sql.strip(), args, kwargs))
 
 
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
@@ -82,18 +84,18 @@
     def __init__(self, connect, use_mysql_connector):
         self.connect = connect
         self.connection = None
         self.transactions = 0
         self.prepared = True
         if use_mysql_connector:
             self.get_cursor = lambda: self.connection.cursor(prepared=self.prepared)
-            self.log = lambda action: logging.debug('%s connection <%s>...' % (action, hex(id(self.connection._cnx))))
+            self.log = lambda action: logger.debug('%s connection <%s>...' % (action, hex(id(self.connection._cnx))))
         else:
             self.get_cursor = lambda: self.connection.cursor()
-            self.log = lambda action: logging.debug('%s connection <%s>...' % (action, hex(id(self.connection))))
+            self.log = lambda action: logger.debug('%s connection <%s>...' % (action, hex(id(self.connection))))
 
     def is_not_init(self):
         return self.connection is None
 
     def init(self):
         self.transactions = 0
         self.connection = self.connect()
@@ -105,15 +107,15 @@
             self.connection.close()
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
-        # logging.debug('Cursor prepared: %s' % self.prepared)
+        # logger.debug('Cursor prepared: %s' % self.prepared)
         return self.get_cursor()
 
     def statement(self, sql: str):
         """
         Return statement
         """
         return self.connection.statement(sql)
@@ -157,15 +159,15 @@
     def __enter__(self):
         self.should_close_conn = False
         if self.db_ctx.is_not_init():
             # needs open a connection first:
             self.db_ctx.init()
             self.should_close_conn = True
         self.db_ctx.transactions += 1
-        logging.debug('Begin transaction...' if self.db_ctx.transactions == 1 else 'Join current transaction...')
+        logger.debug('Begin transaction...' if self.db_ctx.transactions == 1 else 'Join current transaction...')
         return self
 
     def __exit__(self, exctype, excvalue, traceback):
         self.db_ctx.transactions -= 1
         try:
             if self.db_ctx.transactions == 0:
                 if exctype is None:
@@ -176,17 +178,17 @@
             if self.should_close_conn:
                 self.db_ctx.release()
 
     def commit(self):
         try_commit(self.db_ctx)
 
     def rollback(self):
-        logging.warning('Rollback transaction...')
+        logger.warning('Rollback transaction...')
         self.db_ctx.connection.rollback()
-        logging.debug('Rollback ok.')
+        logger.debug('Rollback ok.')
 
 
 class DBError(Exception):
     pass
 
 
 class MapperError(DBError):
@@ -256,22 +258,7 @@
 
 class SqlAction(Enum):
     CALL = 'call'
     INSERT = 'insert'
     UPDATE = 'update'
     DELETE = 'delete'
     SELECT = 'select'
-
-
-class PkStrategy(Enum):
-    """
-    DB: 由数据库的AUTO_INCREMENT自动生成主键
-    SNOWFLAKE: 由Snowflake算法生成主键
-
-    在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
-    OverflowError: Python int too large to convert to C long
-
-    如果用的是mysql.connector，且在Windows上开发测试，可以就在初始化数据库的时候加上参数'use_pure'为True用纯python的connect; 在linux是部署生成环境时去掉'use_pure'用
-    C语言写的connect, 以提高性能.
-    """
-    DB = 'db'
-    SNOWFLAKE = 'snowflake'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysqlx-1.3.4/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.5/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.4
+Version: 1.3.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.3.4/mysqlx.egg-info/SOURCES.txt` & `mysqlx-1.3.5/mysqlx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/PKG-INFO` & `mysqlx-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.4
+Version: 1.3.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.3.4/README.md` & `mysqlx-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/README.rst` & `mysqlx-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/setup.py` & `mysqlx-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.4',
+    version='1.3.5',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `mysqlx-1.3.4/test/dbx_test.py` & `mysqlx-1.3.5/test/dbx_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.4/test/db_test.py` & `mysqlx-1.3.5/test/db_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,18 @@
     test_transaction2(rollback=False)
     assert db.get('select count(1) from user') == 7, 'transaction2'
 
 
 if __name__ == '__main__':
     db.init_db(**DB_CONF, pool_size=2)
     # drop_table()
-    full_test()
+    # full_test()
 
 
-    # for u in db.select('select * from user'):
-    #     print(u)
+    users = db.query_one('select * from user where 1=0')
+    print(users)
     #
     # for u in db.select_page('select * from user', 2, 3):
     #     print(u)
```

### Comparing `mysqlx-1.3.4/test/mapper_test.py` & `mysqlx-1.3.5/test/mapper_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if __name__ == '__main__':
     from config import DB_CONF
     db.init_db(**DB_CONF, debug=False)
     args = [
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
     ]
-    user.batch_insert(args)
+    user.batch_insert(args=args)
 
     print(user.select_name(4))
 
     user.user_update('王五', 5)
 
     user.user_update2(id=6, name='赵六')
```

### Comparing `mysqlx-1.3.4/test/orm_test.py` & `mysqlx-1.3.5/test/orm_test.py`

 * *Files identical despite different names*

