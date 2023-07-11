# Comparing `tmp/vectordb-0.0.8.tar.gz` & `tmp/vectordb-0.0.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectordb-0.0.8.tar", last modified: Tue Jul 11 15:24:26 2023, max compression
+gzip compressed data, was "vectordb-0.0.8.dev3.tar", last modified: Tue Jul 11 15:23:52 2023, max compression
```

## Comparing `vectordb-0.0.8.tar` & `vectordb-0.0.8.dev3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-11 15:24:26.000000 vectordb-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-11 15:24:14.000000 vectordb-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:24:26.000000 vectordb-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-11 15:24:14.000000 vectordb-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:24:14.000000 vectordb-0.0.8/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-11 15:24:14.000000 vectordb-0.0.8/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:24:26.000000 vectordb-0.0.8/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 15:24:25.000000 vectordb-0.0.8/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.251365 vectordb-0.0.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-11 15:23:47.000000 vectordb-0.0.8.dev3/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:23:52.255365 vectordb-0.0.8.dev3/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 15:23:52.000000 vectordb-0.0.8.dev3/vectordb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectordb-0.0.8/README.md` & `vectordb-0.0.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/setup.py` & `vectordb-0.0.8.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.8.dev3/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.8.dev3/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.8.dev3/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.8.dev3/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/__main__.py` & `vectordb-0.0.8.dev3/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/client/client.py` & `vectordb-0.0.8.dev3/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/db/base.py` & `vectordb-0.0.8.dev3/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.8.dev3/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.8.dev3/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.8.dev3/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/db/service.py` & `vectordb-0.0.8.dev3/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/utils/create_doc_type.py` & `vectordb-0.0.8.dev3/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/utils/pass_parameters.py` & `vectordb-0.0.8.dev3/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.8.dev3/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.8.dev3/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb/utils/unify_input_output.py` & `vectordb-0.0.8.dev3/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.8/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.8.dev3/vectordb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/test_hnswlib_vectordb_serve.py
 tests/integration/test_inmemory_vectordb_serve.py
```

