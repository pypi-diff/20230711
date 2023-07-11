# Comparing `tmp/tsc-es-0.5.tar.gz` & `tmp/tsc-es-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-es-0.5.tar", last modified: Tue Jul 11 15:24:51 2023, max compression
+gzip compressed data, was "tsc-es-0.6.tar", last modified: Tue Jul 11 16:18:30 2023, max compression
```

## Comparing `tsc-es-0.5.tar` & `tsc-es-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 15:24:51.959329 tsc-es-0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:24:51.959329 tsc-es-0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 15:20:16.000000 tsc-es-0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/tsc_es/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.5/tsc_es/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17226 2023-07-11 15:24:34.000000 tsc-es-0.5/tsc_es/mongo_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:24:51.959329 tsc-es-0.5/tsc_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 15:24:51.000000 tsc-es-0.5/tsc_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.857484 tsc-es-0.6/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 16:18:30.857484 tsc-es-0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:18:30.857484 tsc-es-0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 16:06:27.000000 tsc-es-0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.841484 tsc-es-0.6/tsc_es/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.6/tsc_es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17239 2023-07-11 16:06:46.000000 tsc-es-0.6/tsc_es/mongo_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.857484 tsc-es-0.6/tsc_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/top_level.txt
```

### Comparing `tsc-es-0.5/LICENSE` & `tsc-es-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-es-0.5/setup.py` & `tsc-es-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = ''
 
 setup(
     name='tsc-es',
-    version='0.5',
+    version='0.6',
     description="mongo to es",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tsc',
     license='GPLv3',
     url='',
     keywords='tools',
```

### Comparing `tsc-es-0.5/tsc_es/mongo_es.py` & `tsc-es-0.6/tsc_es/mongo_es.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
         'time_field_es': time_field_es,
         'time_field_mongo': time_field_mongo,
         'find_num': info_count,
         'success_num': 0,
     }
     
     if info_count:
-        pbar = tqdm(total=info_count, desc='更新中', unit='个文档')
+        pbar = tqdm(total=info_count, desc='更新中', unit='个文档', leave=False)
         for upsert_data_L in get_docs_from_cursor(info, map_fields=map_fields, doc_skip_f=doc_skip_f,
                                                   get_id=get_id, batch_size=batch_size):
             if not upsert_data_L:
                 continue
             if is_stream and raise_on_error:
                 for doc in upsert_data_L:
                     _id = doc.pop('_id')
```

