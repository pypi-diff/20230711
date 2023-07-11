# Comparing `tmp/tsc-es-0.4.tar.gz` & `tmp/tsc-es-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-es-0.4.tar", last modified: Tue Jul 11 14:27:52 2023, max compression
+gzip compressed data, was "tsc-es-0.5.tar", last modified: Tue Jul 11 15:24:51 2023, max compression
```

## Comparing `tsc-es-0.4.tar` & `tsc-es-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.899874 tsc-es-0.4/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 14:27:52.899874 tsc-es-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 14:27:52.899874 tsc-es-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 14:26:32.000000 tsc-es-0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.895874 tsc-es-0.4/tsc_es/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.4/tsc_es/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17040 2023-07-11 14:27:06.000000 tsc-es-0.4/tsc_es/mongo_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:27:52.895874 tsc-es-0.4/tsc_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 14:27:52.000000 tsc-es-0.4/tsc_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 15:24:51.959329 tsc-es-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:24:51.959329 tsc-es-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 15:20:16.000000 tsc-es-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/tsc_es/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.5/tsc_es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17226 2023-07-11 15:24:34.000000 tsc-es-0.5/tsc_es/mongo_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/tsc_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/top_level.txt
```

### Comparing `tsc-es-0.4/LICENSE` & `tsc-es-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-es-0.4/setup.py` & `tsc-es-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = ''
 
 setup(
     name='tsc-es',
-    version='0.4',
+    version='0.5',
     description="mongo to es",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tsc',
     license='GPLv3',
     url='',
     keywords='tools',
```

### Comparing `tsc-es-0.4/tsc_es/mongo_es.py` & `tsc-es-0.5/tsc_es/mongo_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,19 +240,22 @@
                 }
             elif op_type == 'delete':
                 yield {
                     '_op_type': op_type,
                     "_index": name,
                     "_id": item['_id'],
                 }
+    success_num = 0
     for success, info in parallel_bulk(client=client, actions=generate_actions(),
                         chunk_size=3000, thread_count=8, raise_on_error=raise_on_error):
-        if not success:
+        if not success or info.get('index', {}).get('status') == 409:
             logging.info('A document failed: ' + str(info))
-    return True
+        else:
+            success_num += 1
+    return success_num
 
 
 def get_docs_from_cursor(cursor: Cursor, map_fields: dict, batch_size=500, get_id=None, doc_skip_f=None):
     """
     从 mongo 的cursor中构建es需要的索引格式
     :param cursor: 游标
     :param map_fields: 映射字段
@@ -333,43 +336,45 @@
     if start_time:
         mongo_filter[time_field_mongo] = {'$gte': start_time}
     info = collection.find(mongo_filter).sort(time_field_mongo, ASCENDING)
     info_count = collection.count_documents(mongo_filter)
     ret = {
         'time_field_es': time_field_es,
         'time_field_mongo': time_field_mongo,
-        'num': {
-            'upsert_data': info_count,
-        }
+        'find_num': info_count,
+        'success_num': 0,
     }
     
     if info_count:
         pbar = tqdm(total=info_count, desc='更新中', unit='个文档')
         for upsert_data_L in get_docs_from_cursor(info, map_fields=map_fields, doc_skip_f=doc_skip_f,
                                                   get_id=get_id, batch_size=batch_size):
             if not upsert_data_L:
                 continue
             if is_stream and raise_on_error:
                 for doc in upsert_data_L:
                     _id = doc.pop('_id')
                     try:
                         client.create(index=index_name, id=_id, document=doc)
+                        ret['success_num'] += 1
                     except ConflictError:
                         continue
                     except:
                         print(_id, doc)
                         raise
                     pbar.update(1)
             else:
-                es_bulk(client, index_name, upsert_data_L, op_type=op_type, raise_on_error=raise_on_error)
+                ret['success_num'] += es_bulk(client, index_name, upsert_data_L, op_type=op_type, raise_on_error=raise_on_error)
                 pbar.update(len(upsert_data_L))
         pbar.close()
+
+    if ret['success_num']:
         logging.warning(str(ret))
     else:
-        logging.debug('the number of upsert is 0')
+        logging.info(str(ret))
     return ret
 
 
 def time_to_es_date(t, from_utc=False, current_tz=pytz.timezone('Asia/Shanghai')):
     """
     将时间转换成 es 的 date 类型
     :param t: float or datetime; 时间戳或日期类型
```

