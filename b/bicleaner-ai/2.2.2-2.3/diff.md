# Comparing `tmp/bicleaner-ai-2.2.2.tar.gz` & `tmp/bicleaner-ai-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicleaner-ai-2.2.2.tar", last modified: Fri Jun  9 08:45:12 2023, max compression
+gzip compressed data, was "bicleaner-ai-2.3.tar", last modified: Tue Jul 11 10:01:41 2023, max compression
```

## Comparing `bicleaner-ai-2.2.2.tar` & `bicleaner-ai-2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24077 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.083460 bicleaner-ai-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/src/bicleaner_ai/
--rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3607 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download_hf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    14123 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/classify.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/datagen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/decomposable_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/models_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/training.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/util.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:01:41.931206 bicleaner-ai-2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    65920 2023-07-11 10:01:41.931206 bicleaner-ai-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24441 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 10:01:41.931206 bicleaner-ai-2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:01:41.923206 bicleaner-ai-2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:01:41.931206 bicleaner-ai-2.3/src/bicleaner_ai/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4132 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_download_hf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14123 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/classify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/decomposable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/models_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_zipf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-07-11 10:01:30.000000 bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_zipf_double_linked.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:01:41.931206 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    65920 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-11 10:01:41.000000 bicleaner-ai-2.3/src/bicleaner_ai.egg-info/top_level.txt
```

### Comparing `bicleaner-ai-2.2.2/LICENSE` & `bicleaner-ai-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/PKG-INFO` & `bicleaner-ai-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.2
+Version: 2.3
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -821,14 +821,19 @@
 
 Or you can download a lite model with:
 ```
 bicleaner-ai-download en fr lite ./bicleaner-models
 ```
 This will download and store the en-fr lite model at `./bicleaner-models/en-fr`.
 
+Since 2.3.0 version, full models also accept a local path to download, instead of the HF cache directory.
+In that case, to use the model, provide the local path instead of the HF identifier.
+
+To read more information about how HF cache works, please read the [official documentation](https://huggingface.co/docs/transformers/v4.30.0/en/installation#cache-setup).
+
 #### Classifying
 To classify a tab separated file containing English sentences in the first column and French sentences in the second column, use
 ```bash
 bicleaner-ai-classify  \
         --scol 1 --tcol 2
         corpus.en-fr.tsv  \
         corpus.en-fr.classifed.tsv  \
```

### Comparing `bicleaner-ai-2.2.2/README.md` & `bicleaner-ai-2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,19 @@
 
 Or you can download a lite model with:
 ```
 bicleaner-ai-download en fr lite ./bicleaner-models
 ```
 This will download and store the en-fr lite model at `./bicleaner-models/en-fr`.
 
+Since 2.3.0 version, full models also accept a local path to download, instead of the HF cache directory.
+In that case, to use the model, provide the local path instead of the HF identifier.
+
+To read more information about how HF cache works, please read the [official documentation](https://huggingface.co/docs/transformers/v4.30.0/en/installation#cache-setup).
+
 #### Classifying
 To classify a tab separated file containing English sentences in the first column and French sentences in the second column, use
 ```bash
 bicleaner-ai-classify  \
         --scol 1 --tcol 2
         corpus.en-fr.tsv  \
         corpus.en-fr.classifed.tsv  \
```

### Comparing `bicleaner-ai-2.2.2/pyproject.toml` & `bicleaner-ai-2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-ai"
-version = "2.2.2"
+version = "2.3"
 license = {file = "LICENSE"}
 authors = [
     { "name" = "Prompsit Language Engineering", "email" = "info@prompsit.com" }
 ]
 maintainers = [
     { "name" = "Jaume Zaragoza", "email" = "jzaragoza@prompsit.com" }
 ]
@@ -21,16 +21,16 @@
     "sacremoses",
     "bicleaner-hardrules==2.8.1",
     "sentencepiece",
     "tensorflow>=2.6.5,<2.12",
     "bicleaner-ai-glove==0.2.1",
     "fuzzywuzzy",
     "python-Levenshtein",
-    "transformers==4.26",
-    "huggingface-hub>=0.13,<0.14",
+    "transformers==4.30.2",
+    "huggingface-hub==0.15.1",
     "psutil",
     "regex",
 ]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.7",
```

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_classifier.py` & `bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_classifier.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download.py` & `bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_download.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,24 @@
         raise Exception("Lite models need a download path")
 
     if args.model_type == 'full':
         #TODO fallback to github if does not exist?
         name = f'bitextor/bicleaner-ai-full-{args.src_lang}-{args.trg_lang}'
         logging.info(f'Downloading {name}')
         try:
-            snapshot_download(name, use_auth_token=args.auth_token, etag_timeout=100)
+            if not args.download_path:
+                snapshot_download(name, use_auth_token=args.auth_token,
+                                  etag_timeout=100, max_workers=1)
+            else:
+                local_dir = f"{args.download_path}/{args.src_lang}-{args.trg_lang}"
+                logging.debug(f"Saving model to local dir: {local_dir}")
+                snapshot_download(name, use_auth_token=args.auth_token,
+                                  local_dir=local_dir,
+                                  local_dir_use_symlinks=False,
+                                  etag_timeout=100, max_workers=1)
             return
         except RepositoryNotFoundError:
             if not args.download_path:
                 logging.error(f"Model repository {name} not found at HuggingFace," \
                               + "please provide a path to download old model from Github")
             logging.warning(f"Model repository {name} not found, trying Github old models...")
```

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download_hf.py` & `bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_download_hf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_train.py` & `bicleaner-ai-2.3/src/bicleaner_ai/bicleaner_ai_train.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/calibrate.py` & `bicleaner-ai-2.3/src/bicleaner_ai/calibrate.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/classify.py` & `bicleaner-ai-2.3/src/bicleaner_ai/classify.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/datagen.py` & `bicleaner-ai-2.3/src/bicleaner_ai/datagen.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/decomposable_attention.py` & `bicleaner-ai-2.3/src/bicleaner_ai/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/layers.py` & `bicleaner-ai-2.3/src/bicleaner_ai/layers.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/losses.py` & `bicleaner-ai-2.3/src/bicleaner_ai/losses.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/metrics.py` & `bicleaner-ai-2.3/src/bicleaner_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/models.py` & `bicleaner-ai-2.3/src/bicleaner_ai/models.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/models_util.py` & `bicleaner-ai-2.3/src/bicleaner_ai/models_util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/tokenizer.py` & `bicleaner-ai-2.3/src/bicleaner_ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/training.py` & `bicleaner-ai-2.3/src/bicleaner_ai/training.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/util.py` & `bicleaner-ai-2.3/src/bicleaner_ai/util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_list.py` & `bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_list.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf.py` & `bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_zipf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py` & `bicleaner-ai-2.3/src/bicleaner_ai/word_freqs_zipf_double_linked.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/PKG-INFO` & `bicleaner-ai-2.3/src/bicleaner_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.2
+Version: 2.3
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -821,14 +821,19 @@
 
 Or you can download a lite model with:
 ```
 bicleaner-ai-download en fr lite ./bicleaner-models
 ```
 This will download and store the en-fr lite model at `./bicleaner-models/en-fr`.
 
+Since 2.3.0 version, full models also accept a local path to download, instead of the HF cache directory.
+In that case, to use the model, provide the local path instead of the HF identifier.
+
+To read more information about how HF cache works, please read the [official documentation](https://huggingface.co/docs/transformers/v4.30.0/en/installation#cache-setup).
+
 #### Classifying
 To classify a tab separated file containing English sentences in the first column and French sentences in the second column, use
 ```bash
 bicleaner-ai-classify  \
         --scol 1 --tcol 2
         corpus.en-fr.tsv  \
         corpus.en-fr.classifed.tsv  \
```

### Comparing `bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/SOURCES.txt` & `bicleaner-ai-2.3/src/bicleaner_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

