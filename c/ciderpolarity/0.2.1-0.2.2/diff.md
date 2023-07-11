# Comparing `tmp/ciderpolarity-0.2.1.tar.gz` & `tmp/ciderpolarity-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.1.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.2.tar", max compression
```

## Comparing `ciderpolarity-0.2.1.tar` & `ciderpolarity-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.1/LICENSE
--rw-r--r--   0        0        0     4582 2023-07-11 11:55:51.733711 ciderpolarity-0.2.1/README.md
--rw-r--r--   0        0        0     8790 2023-07-10 14:03:02.477624 ciderpolarity-0.2.1/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.1/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.1/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2630 2023-07-11 09:15:25.743879 ciderpolarity-0.2.1/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.1/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.1/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.1/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.1/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.1/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      410 2023-07-11 14:31:33.437562 ciderpolarity-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 ciderpolarity-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4580 2023-07-11 15:29:00.896330 ciderpolarity-0.2.2/README.md
+-rw-r--r--   0        0        0     8790 2023-07-10 14:03:02.477624 ciderpolarity-0.2.2/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.2/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.2/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2630 2023-07-11 09:15:25.743879 ciderpolarity-0.2.2/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.2/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.2/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.2/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.2/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.2/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-11 15:30:05.547752 ciderpolarity-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 ciderpolarity-0.2.2/PKG-INFO
```

### Comparing `ciderpolarity-0.2.1/LICENSE` & `ciderpolarity-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/README.md` & `ciderpolarity-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 texts = ['Really hate this heat. Just want AC',
          'I love an icecream in this heat!',
          'I’m melting - terrible weather!',
          'Very dehydrated in this heat',
                 ...                    ,
          'this sunny weather is great',
          'Oh my icecream is melting',
-         'My AC is broken! 🥵'],
+         'My AC is broken! 🥵']
 
 
 output_folder = '/path/to/output/folder/'
 
 cdr = CIDER(input_file, output_folder)
 results = cdr.fit_transform()
 ```
@@ -56,15 +56,15 @@
     ['Really hate this heat. Just want AC', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
     ['I love an icecream in this heat!', {"neg":0.0, "neu":0.5, "pos":0.5, "compound":0.6}],
     ['I’m melting - terrible weather!', {"neg":0.7, "neu":0.3, "pos":0.0, "compound":-0.7}],
     ['Very dehydrated in this heat', {"neg":0.5, "neu":0.4, "pos":0.0, "compound":-0.5}],
             ...
     ['this sunny weather is great', {"neg":0.0, "neu":0.2, "pos":0.8, "compound":0.7}],
     ['Oh my icecream is melting', {"neg":0.3, "neu":0.4, "pos":0.3, "compound":0.0}],
-    ['My AC is broken! 🥵', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
+    ['My AC is broken! 🥵', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}]
 ]
 
 ```
 
 ## Examples
 **Some alternative ways to use the library are as follows:**
```

### Comparing `ciderpolarity-0.2.1/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.2/ciderpolarity/CIDER.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.2/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.2/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.2/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.2/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.2/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.2/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.2/ciderpolarity/utils_funcs.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.1/PKG-INFO` & `ciderpolarity-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
+Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +15,15 @@
 Requires-Dist: gensim (>=4.1.0,<5.0.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.0,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: tqdm (>=4.55.0,<5.0.0)
 Requires-Dist: vadersentiment (>=3.3.2,<4.0.0)
+Project-URL: Repository, https://github.com/jcy204/ciderPolarity
 Description-Content-Type: text/markdown
 
 # CIDER Python Package
 
 CIDER (Context Informed Dictionary and sEntiment Reasoner) is a Python library used to improve domain-specific sentiment analysis.
 
 It generates, filters, and substitutes polarities into [VADER](https://github.com/cjhutto/vaderSentiment/). 
@@ -58,15 +60,15 @@
 texts = ['Really hate this heat. Just want AC',
          'I love an icecream in this heat!',
          'I’m melting - terrible weather!',
          'Very dehydrated in this heat',
                 ...                    ,
          'this sunny weather is great',
          'Oh my icecream is melting',
-         'My AC is broken! 🥵'],
+         'My AC is broken! 🥵']
 
 
 output_folder = '/path/to/output/folder/'
 
 cdr = CIDER(input_file, output_folder)
 results = cdr.fit_transform()
 ```
@@ -78,15 +80,15 @@
     ['Really hate this heat. Just want AC', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
     ['I love an icecream in this heat!', {"neg":0.0, "neu":0.5, "pos":0.5, "compound":0.6}],
     ['I’m melting - terrible weather!', {"neg":0.7, "neu":0.3, "pos":0.0, "compound":-0.7}],
     ['Very dehydrated in this heat', {"neg":0.5, "neu":0.4, "pos":0.0, "compound":-0.5}],
             ...
     ['this sunny weather is great', {"neg":0.0, "neu":0.2, "pos":0.8, "compound":0.7}],
     ['Oh my icecream is melting', {"neg":0.3, "neu":0.4, "pos":0.3, "compound":0.0}],
-    ['My AC is broken! 🥵', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
+    ['My AC is broken! 🥵', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}]
 ]
 
 ```
 
 ## Examples
 **Some alternative ways to use the library are as follows:**
```

