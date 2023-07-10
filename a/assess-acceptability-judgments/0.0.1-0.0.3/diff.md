# Comparing `tmp/assess_acceptability_judgments-0.0.1.tar.gz` & `tmp/assess_acceptability_judgments-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assess_acceptability_judgments-0.0.1.tar", last modified: Sun Jul  9 01:53:12 2023, max compression
+gzip compressed data, was "assess_acceptability_judgments-0.0.3.tar", last modified: Mon Jul 10 22:20:47 2023, max compression
```

## Comparing `assess_acceptability_judgments-0.0.1.tar` & `assess_acceptability_judgments-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:53:12.271894 assess_acceptability_judgments-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-09 01:53:12.271894 assess_acceptability_judgments-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:53:12.271894 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/fluency_score_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/link_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/nce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/ppl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/slor.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:53:12.271894 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-09 01:53:12.000000 assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 01:53:12.271894 assess_acceptability_judgments-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-09 01:53:03.000000 assess_acceptability_judgments-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.582926 assess_acceptability_judgments-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-10 22:20:47.582926 assess_acceptability_judgments-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.562926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/fluency_score_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/link_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/nce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/ppl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.558926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.566926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.566926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.582926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/
+-rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/slor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:20:47.562926 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 22:20:47.000000 assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 22:20:47.582926 assess_acceptability_judgments-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-10 22:20:38.000000 assess_acceptability_judgments-0.0.3/setup.py
```

### Comparing `assess_acceptability_judgments-0.0.1/LICENSE` & `assess_acceptability_judgments-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.1/PKG-INFO` & `assess_acceptability_judgments-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess_acceptability_judgments
-Version: 0.0.1
+Version: 0.0.3
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.1.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.3.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/fluency_score_interface.py` & `assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/fluency_score_interface.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/nce.py` & `assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/nce.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/ppl.py` & `assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/ppl.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.1/assess_acceptability_judgments/slor.py` & `assess_acceptability_judgments-0.0.3/assess_acceptability_judgments/slor.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.1/assess_acceptability_judgments.egg-info/PKG-INFO` & `assess_acceptability_judgments-0.0.3/assess_acceptability_judgments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess-acceptability-judgments
-Version: 0.0.1
+Version: 0.0.3
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.1.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.3.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.1/setup.py` & `assess_acceptability_judgments-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import os
 import subprocess
 
 from setuptools import setup, find_packages
 
 current_file_path = os.path.abspath(os.path.dirname(__file__))
 
@@ -64,14 +65,20 @@
             "Programming Language :: Python :: 3.11",
             "Topic :: Software Development :: Libraries",
             "Topic :: Software Development :: Libraries :: Python Modules",
             "Topic :: Scientific/Engineering",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
         ],
         packages=packages,
+        data_files=[
+            ("resources.nce_scores_distribution", glob.glob('*/*/nce_scores_distribution/*')),
+            ("resources.slor_scores_distribution", glob.glob('*/*/slor_scores_distribution/*')),
+            ("resources.words_probability", glob.glob('*/*/words_probability/*')),
+        ],
+        include_package_data=True,
         install_requires=[
             "transformers",
             "torch",
             "numpy",
             "nltk",
         ],
         python_requires=">=3.8",
```

