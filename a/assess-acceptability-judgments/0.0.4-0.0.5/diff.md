# Comparing `tmp/assess_acceptability_judgments-0.0.4.tar.gz` & `tmp/assess_acceptability_judgments-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assess_acceptability_judgments-0.0.4.tar", last modified: Tue Jul 11 11:56:30 2023, max compression
+gzip compressed data, was "assess_acceptability_judgments-0.0.5.tar", last modified: Tue Jul 11 19:42:52 2023, max compression
```

## Comparing `assess_acceptability_judgments-0.0.4.tar` & `assess_acceptability_judgments-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.464367 assess_acceptability_judgments-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 11:56:30.464367 assess_acceptability_judgments-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.448366 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/fluency_score_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/link_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/nce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/ppl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.444366 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.448366 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.448366 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.464367 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/
--rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/slor.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:30.448366 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 11:56:30.000000 assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 11:56:30.464367 assess_acceptability_judgments-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-11 11:56:19.000000 assess_acceptability_judgments-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.355153 assess_acceptability_judgments-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 19:42:52.355153 assess_acceptability_judgments-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.335153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/fluency_score_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/link_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/nce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/ppl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.335153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.335153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.339153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.351153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/
+-rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/slor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 19:42:51.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:52.335153 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 19:42:52.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-11 19:42:52.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:42:52.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 19:42:52.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 19:42:52.000000 assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 19:42:52.355153 assess_acceptability_judgments-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-11 19:42:36.000000 assess_acceptability_judgments-0.0.5/setup.py
```

### Comparing `assess_acceptability_judgments-0.0.4/LICENSE` & `assess_acceptability_judgments-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/PKG-INFO` & `assess_acceptability_judgments-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess_acceptability_judgments
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.4.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.5.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/fluency_score_interface.py` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/fluency_score_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     @staticmethod
     def _compute_sentences_len(sentences_mask: List[Tensor]) -> List[int]:
         """
         To compute the len of a sequence using the mask.
         """
         # |S| in equation (1) of article https://arxiv.org/pdf/1809.08731v1.pdf
-        sentences_len: List[int] = [sum(sentence_mask).item() for sentence_mask in sentences_mask]
+        sentences_len: List[int] = [sentence_mask.sum().item() for sentence_mask in sentences_mask]
         return sentences_len
 
     @staticmethod
     def _compute_pm(
         padded_sentences_words_idx: List[List[int]],
         sentences_mask: List[Tensor],
         batch_logits: Tensor,
```

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/nce.py` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/nce.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/ppl.py` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/ppl.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/treebank.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/treebank.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments/slor.py` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments/slor.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/PKG-INFO` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess-acceptability-judgments
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.4.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.5.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.4/assess_acceptability_judgments.egg-info/SOURCES.txt` & `assess_acceptability_judgments-0.0.5/assess_acceptability_judgments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.4/setup.py` & `assess_acceptability_judgments-0.0.5/setup.py`

 * *Files identical despite different names*

