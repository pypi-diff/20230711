# Comparing `tmp/ciderpolarity-0.2.0.tar.gz` & `tmp/ciderpolarity-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.0.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.1.tar", max compression
```

## Comparing `ciderpolarity-0.2.0.tar` & `ciderpolarity-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.0/LICENSE
--rw-r--r--   0        0        0     4582 2023-07-11 11:55:51.733711 ciderpolarity-0.2.0/README.md
--rw-r--r--   0        0        0     8790 2023-07-10 14:03:02.477624 ciderpolarity-0.2.0/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.0/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.0/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2630 2023-07-11 09:15:25.743879 ciderpolarity-0.2.0/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.0/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.0/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.0/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.0/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1119 2023-07-11 09:15:53.459747 ciderpolarity-0.2.0/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      410 2023-07-11 11:56:08.821545 ciderpolarity-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 ciderpolarity-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4582 2023-07-11 11:55:51.733711 ciderpolarity-0.2.1/README.md
+-rw-r--r--   0        0        0     8790 2023-07-10 14:03:02.477624 ciderpolarity-0.2.1/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.1/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.1/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2630 2023-07-11 09:15:25.743879 ciderpolarity-0.2.1/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.1/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.1/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.1/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.1/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.1/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      410 2023-07-11 14:31:33.437562 ciderpolarity-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 ciderpolarity-0.2.1/PKG-INFO
```

### Comparing `ciderpolarity-0.2.0/LICENSE` & `ciderpolarity-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/README.md` & `ciderpolarity-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.1/ciderpolarity/CIDER.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.1/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.1/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.1/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.1/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.1/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.1/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.0/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.1/ciderpolarity/utils_funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 def text_iterate(SS, show=False, full=False):
     'Allows iteration over a list of text or a jsonl/json file'
     if isinstance(SS.FILEINPUT, list):
         for row in tqdm(SS.FILEINPUT, total=SS.LINES,
                         disable=not show):
             yield row
     else:
-        with open(SS.FILEINPUT) as f:
+        with open(SS.FILEINPUT, encoding='utf-8') as f:
             reader = csv.reader(f)
             for row in tqdm(reader, total=SS.LINES, disable=not show):
                 if full:
                     yield row
                 else:
-                    yield ' ,'.join(row)
+                    yield ' ,'.join(row)
```

### Comparing `ciderpolarity-0.2.0/PKG-INFO` & `ciderpolarity-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

