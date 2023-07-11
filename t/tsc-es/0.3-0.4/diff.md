# Comparing `tmp/tsc-es-0.3.tar.gz` & `tmp/tsc-es-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-es-0.3.tar", last modified: Sun Jul  9 14:51:32 2023, max compression
+gzip compressed data, was "tsc-es-0.4.tar", last modified: Tue Jul 11 14:27:52 2023, max compression
```

## Comparing `tsc-es-0.3.tar` & `tsc-es-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:51:32.550081 tsc-es-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:51:32.550081 tsc-es-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-09 14:51:30.000000 tsc-es-0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/tsc_es/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.3/tsc_es/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16553 2023-07-09 14:51:26.000000 tsc-es-0.3/tsc_es/mongo_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/tsc_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.899874 tsc-es-0.4/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 14:27:52.899874 tsc-es-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 14:27:52.899874 tsc-es-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 14:26:32.000000 tsc-es-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.895874 tsc-es-0.4/tsc_es/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.4/tsc_es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17040 2023-07-11 14:27:06.000000 tsc-es-0.4/tsc_es/mongo_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.895874 tsc-es-0.4/tsc_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/top_level.txt
```

### Comparing `tsc-es-0.3/LICENSE` & `tsc-es-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-es-0.3/setup.py` & `tsc-es-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = ''
 
 setup(
     name='tsc-es',
-    version='0.3',
+    version='0.4',
     description="mongo to es",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tsc',
     license='GPLv3',
     url='',
     keywords='tools',
```

### Comparing `tsc-es-0.3/tsc_es/mongo_es.py` & `tsc-es-0.4/tsc_es/mongo_es.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,21 +206,22 @@
         else:
             client.indices.delete(index=name)
             logging.warning(f'index {name} del')
     except NotFoundError:
         ...
 
 
-def es_bulk(client: Elasticsearch, name: str, data: list, op_type='index'):
+def es_bulk(client: Elasticsearch, name: str, data: list, op_type='index', raise_on_error=True):
     """
     批量索引数据
     :param client: es 客户端
     :param name: 索引名称
     :param data: 待索引的数据
     :param op_type: 索引类型
+    :param raise_on_error: 在插入一条出现错误的时候是否报错, False 表示继续插入下一条
     :return: 
     """
     logging.debug('op_type:'+op_type+' ,number is:' + str(len(data)))
     
     def generate_actions():
         for item in data:
             assert '_id' in item
@@ -239,16 +240,18 @@
                 }
             elif op_type == 'delete':
                 yield {
                     '_op_type': op_type,
                     "_index": name,
                     "_id": item['_id'],
                 }
-    deque(parallel_bulk(client=client, actions=generate_actions(),
-                        chunk_size=3000, thread_count=8), maxlen=0)
+    for success, info in parallel_bulk(client=client, actions=generate_actions(),
+                        chunk_size=3000, thread_count=8, raise_on_error=raise_on_error):
+        if not success:
+            logging.info('A document failed: ' + str(info))
     return True
 
 
 def get_docs_from_cursor(cursor: Cursor, map_fields: dict, batch_size=500, get_id=None, doc_skip_f=None):
     """
     从 mongo 的cursor中构建es需要的索引格式
     :param cursor: 游标
@@ -276,48 +279,49 @@
             yield batch
             batch = []
     if batch:
         yield batch
 
 
 def mongo_to_es(client: Elasticsearch, index_name: str, collection: Collection, map_fields: dict,
-          time_field_es: str, time_field_mongo: str,
-          es_is_date=False, mongo_is_date=False, timestamp_tz='Asia/Shanghai',
-          doc_skip_f=None, get_id=None, batch_size=500, is_stream=False):
+          time_field_es: str, time_field_mongo: str, mongo_is_date=False, timestamp_tz='Asia/Shanghai',
+          doc_skip_f=None, get_id=None, batch_size=500, is_stream=False, raise_on_error=True, op_type='index'):
     """
     从 mongo 导入到 es
     :param client: es 客户端
     :param index_name: 索引名称
     :param collection: mongo 的集合
     :param map_fields: 映射字段
     :param time_field_es: es 中的时间字段, 用于增量更新
     :param time_field_mongo: mongo 中的时间字段, 用于增量更新
-    :param es_is_date: time_field_es 是否为 date 类型, 否则代表是精确到微秒的秒级时间戳
     :param mongo_is_date: time_field_mongo 是否为 date 类型, 否则代表是精确到微秒的秒级时间戳
     :param timestamp_tz: time_field_mongo 为时间戳时候的时区
     :param doc_skip_f: 参见 get_docs_from_cursor
     :param get_id: 参见 get_docs_from_cursor
     :param batch_size: 参见 get_docs_from_cursor
     :param is_stream: 是否是 date_stream 索引
+    :param raise_on_error: 在插入一条出现错误的时候是否报错, False 表示不管这个错误继续插入下一条
+    :param op_type: 索引类型, data stream 会自动修改为 create
     :return: 
     """
+    op_type = 'create' if is_stream else op_type
     body = {
         "size": 1,
         "query": {
             "match_all": {},
         },
         "sort": {
             time_field_es: {"order": "desc"},
         },
     }
     es_res = client.search(index=index_name, **body)
     start_time = None
     if es_res['hits']['hits'] and es_res['hits']['hits'][0]['_source'][time_field_es]:
         start_time = es_res['hits']['hits'][0]['_source'][time_field_es]
-        if es_is_date:  # 精确到毫秒的日期
+        if isinstance(start_time, str):  # 精确到毫秒的日期
             start_time = datetime.strptime(start_time, r"%Y-%m-%dT%H:%M:%S.%fZ").replace(tzinfo=pytz.UTC)
             if mongo_is_date:
                 start_time = start_time + timedelta(milliseconds=1)
             else:  # 需要确保 mongo 中的时间戳的时区是当地时区
                 start_time = start_time.timestamp() + 0.001
         else:
             start_time += 1e-6  # 要求是精确到微秒的秒级时间戳
@@ -340,27 +344,27 @@
     
     if info_count:
         pbar = tqdm(total=info_count, desc='更新中', unit='个文档')
         for upsert_data_L in get_docs_from_cursor(info, map_fields=map_fields, doc_skip_f=doc_skip_f,
                                                   get_id=get_id, batch_size=batch_size):
             if not upsert_data_L:
                 continue
-            if is_stream:
+            if is_stream and raise_on_error:
                 for doc in upsert_data_L:
                     _id = doc.pop('_id')
                     try:
                         client.create(index=index_name, id=_id, document=doc)
                     except ConflictError:
                         continue
                     except:
                         print(_id, doc)
                         raise
                     pbar.update(1)
             else:
-                es_bulk(client, index_name, upsert_data_L)
+                es_bulk(client, index_name, upsert_data_L, op_type=op_type, raise_on_error=raise_on_error)
                 pbar.update(len(upsert_data_L))
         pbar.close()
         logging.warning(str(ret))
     else:
         logging.debug('the number of upsert is 0')
     return ret
```

