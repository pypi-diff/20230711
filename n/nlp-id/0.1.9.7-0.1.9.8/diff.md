# Comparing `tmp/nlp_id-0.1.9.7.tar.gz` & `tmp/nlp_id-0.1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nlp_id-0.1.9.7.tar", last modified: Tue Jul  7 03:51:14 2020, max compression
+gzip compressed data, was "dist/nlp_id-0.1.9.8.tar", last modified: Thu Jul 16 06:46:23 2020, max compression
```

## Comparing `nlp_id-0.1.9.7.tar` & `nlp_id-0.1.9.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     1040 2020-07-07 03:48:10.000000 nlp_id-0.1.9.7/setup.py
-drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/
--rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)        7 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/top_level.txt
--rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)       41 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/requires.txt
--rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)        1 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/dependency_links.txt
--rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)      383 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/SOURCES.txt
--rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)     6867 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id.egg-info/PKG-INFO
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)       79 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/setup.cfg
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     5397 2020-07-07 03:24:16.000000 nlp_id-0.1.9.7/README.md
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     6867 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/PKG-INFO
-drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id/
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     7750 2020-04-07 10:59:39.000000 nlp_id-0.1.9.7/nlp_id/lemmatizer.py
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     7806 2020-04-21 06:55:02.000000 nlp_id-0.1.9.7/nlp_id/postag.py
-drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-07 03:51:14.000000 nlp_id-0.1.9.7/nlp_id/data/
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)   236287 2019-11-18 08:09:00.000000 nlp_id-0.1.9.7/nlp_id/data/root-word.txt
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000) 19937523 2020-01-08 09:20:10.000000 nlp_id-0.1.9.7/nlp_id/data/lemma_dict.json
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)  5178661 2020-04-21 06:13:39.000000 nlp_id-0.1.9.7/nlp_id/data/dataset_postag.txt
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)    10520 2020-04-21 06:59:46.000000 nlp_id-0.1.9.7/nlp_id/data/stopword.txt
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     5559 2020-07-07 03:45:37.000000 nlp_id-0.1.9.7/nlp_id/tokenizer.py
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)      432 2020-04-21 07:01:17.000000 nlp_id-0.1.9.7/nlp_id/stopword.py
--rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)      221 2020-04-21 07:03:02.000000 nlp_id-0.1.9.7/nlp_id/__init__.py
+drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     1040 2020-07-16 06:38:57.000000 nlp_id-0.1.9.8/setup.py
+drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/
+-rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)        7 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/top_level.txt
+-rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)       41 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/requires.txt
+-rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)        1 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/dependency_links.txt
+-rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)      383 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/SOURCES.txt
+-rw-r--r--   0 frandyeddy  (1000) frandyeddy  (1000)     7880 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id.egg-info/PKG-INFO
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)       79 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/setup.cfg
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     6242 2020-07-16 06:38:32.000000 nlp_id-0.1.9.8/README.md
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     7880 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/PKG-INFO
+drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id/
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     7750 2020-04-07 10:59:39.000000 nlp_id-0.1.9.8/nlp_id/lemmatizer.py
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     7806 2020-04-21 06:55:02.000000 nlp_id-0.1.9.8/nlp_id/postag.py
+drwxrwxr-x   0 frandyeddy  (1000) frandyeddy  (1000)        0 2020-07-16 06:46:22.000000 nlp_id-0.1.9.8/nlp_id/data/
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)   236287 2019-11-18 08:09:00.000000 nlp_id-0.1.9.8/nlp_id/data/root-word.txt
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000) 19937523 2020-01-08 09:20:10.000000 nlp_id-0.1.9.8/nlp_id/data/lemma_dict.json
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)  5178661 2020-04-21 06:13:39.000000 nlp_id-0.1.9.8/nlp_id/data/dataset_postag.txt
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)    10520 2020-04-21 06:59:46.000000 nlp_id-0.1.9.8/nlp_id/data/stopword.txt
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)     5559 2020-07-07 03:45:37.000000 nlp_id-0.1.9.8/nlp_id/tokenizer.py
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)      916 2020-07-16 06:38:32.000000 nlp_id-0.1.9.8/nlp_id/stopword.py
+-rw-rw-r--   0 frandyeddy  (1000) frandyeddy  (1000)      221 2020-04-21 07:03:02.000000 nlp_id-0.1.9.8/nlp_id/__init__.py
```

### Comparing `nlp_id-0.1.9.7/setup.py` & `nlp_id-0.1.9.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # Package details
 setup(
   name='nlp_id',
   packages=['nlp_id'],
-  version='0.1.9.7',
+  version='0.1.9.8',
   license='MIT',
   description="Kumparan's NLP Services",
   long_description=open("README.md", "r").read(),
   long_description_content_type="text/markdown",
   author='Frandy Eddy',
   author_email='eddy.frandy@gmail.com',
   url='https://github.com/kumparan/nlp-id',
```

### Comparing `nlp_id-0.1.9.7/nlp_id.egg-info/PKG-INFO` & `nlp_id-0.1.9.8/nlp_id.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-id
-Version: 0.1.9.7
+Version: 0.1.9.8
 Summary: Kumparan's NLP Services
 Home-page: https://github.com/kumparan/nlp-id
 Author: Frandy Eddy
 Author-email: eddy.frandy@gmail.com
 License: MIT
 Description: # Kumparan's NLP Services
         
@@ -87,14 +87,35 @@
         | 16 | VB | Verb. Includes transitive verbs, intransitive verbs, active verbs, passive verbs, and copulas. | tertidur, bekerja, membaca |
         | 17 | WH | Question words | siapa, apa, kapan, bagaimana |
         | 18 | ADJP | Adjective Phrase. A group of words headed by an adjective that describes a noun or a pronoun | sangat tinggi |
         | 19 | DP | Date Phrase. Date written with whitespaces | 1 Januari 2020 |
         | 20 | NP | Noun Phrase. A phrase that has a noun (or indefinite pronoun) as its head | Jakarta Pusat, Lionel Messi |
         | 21 | NUMP | Number Phrase.  | 10 juta |
         | 22 | VP | Verb Phrase. A syntactic unit composed of at least one verb and its dependents | tidak makan |
+        
+        ### Stopword
+        
+        `nlp-id` also provide list of Indonesian stopword.
+        
+            from nlp_id.stopword import StopWord 
+            stopword = StopWord() 
+            stopword.get_stopword() 
+            # [{list_of_nlp_id_stopword}]    
+        
+        Stopword Removal is used to remove every Indonesian stopword from the given text.
+        
+            from nlp_id.stopword import StopWord 
+            text = "Lionel Messi pergi Ke pasar di area Jakarta Pusat" # single sentence
+            stopword = StopWord() 
+            stopword.remove_stopword(text)
+            # Lionel Messi pergi pasar area Jakarta Pusat  
+            
+            paragraph = "Lionel Messi pergi Ke pasar di area Jakarta Pusat itu. Sedangkan Cristiano Ronaldo ke pasar Di area Jakarta Selatan. Dan mereka tidak bertemu begini-begitu."
+            stopword.remove_stopword(text)
+            # Lionel Messi pergi pasar area Jakarta Pusat. Cristiano Ronaldo pasar area Jakarta Selatan. bertemu.
 Keywords: Indonesian,Bahasa,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nlp_id-0.1.9.7/README.md` & `nlp_id-0.1.9.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -78,8 +78,29 @@
 | 15 | UH | Interjection. Interjection expresses feeling or state of mind and has no relation with other words syntactically. | ayo, mari, aduh|
 | 16 | VB | Verb. Includes transitive verbs, intransitive verbs, active verbs, passive verbs, and copulas. | tertidur, bekerja, membaca |
 | 17 | WH | Question words | siapa, apa, kapan, bagaimana |
 | 18 | ADJP | Adjective Phrase. A group of words headed by an adjective that describes a noun or a pronoun | sangat tinggi |
 | 19 | DP | Date Phrase. Date written with whitespaces | 1 Januari 2020 |
 | 20 | NP | Noun Phrase. A phrase that has a noun (or indefinite pronoun) as its head | Jakarta Pusat, Lionel Messi |
 | 21 | NUMP | Number Phrase.  | 10 juta |
-| 22 | VP | Verb Phrase. A syntactic unit composed of at least one verb and its dependents | tidak makan |
+| 22 | VP | Verb Phrase. A syntactic unit composed of at least one verb and its dependents | tidak makan |
+
+### Stopword
+
+`nlp-id` also provide list of Indonesian stopword.
+
+    from nlp_id.stopword import StopWord 
+    stopword = StopWord() 
+    stopword.get_stopword() 
+    # [{list_of_nlp_id_stopword}]    
+
+Stopword Removal is used to remove every Indonesian stopword from the given text.
+
+    from nlp_id.stopword import StopWord 
+    text = "Lionel Messi pergi Ke pasar di area Jakarta Pusat" # single sentence
+    stopword = StopWord() 
+    stopword.remove_stopword(text)
+    # Lionel Messi pergi pasar area Jakarta Pusat  
+    
+    paragraph = "Lionel Messi pergi Ke pasar di area Jakarta Pusat itu. Sedangkan Cristiano Ronaldo ke pasar Di area Jakarta Selatan. Dan mereka tidak bertemu begini-begitu."
+    stopword.remove_stopword(text)
+    # Lionel Messi pergi pasar area Jakarta Pusat. Cristiano Ronaldo pasar area Jakarta Selatan. bertemu.
```

### Comparing `nlp_id-0.1.9.7/PKG-INFO` & `nlp_id-0.1.9.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp_id
-Version: 0.1.9.7
+Version: 0.1.9.8
 Summary: Kumparan's NLP Services
 Home-page: https://github.com/kumparan/nlp-id
 Author: Frandy Eddy
 Author-email: eddy.frandy@gmail.com
 License: MIT
 Description: # Kumparan's NLP Services
         
@@ -87,14 +87,35 @@
         | 16 | VB | Verb. Includes transitive verbs, intransitive verbs, active verbs, passive verbs, and copulas. | tertidur, bekerja, membaca |
         | 17 | WH | Question words | siapa, apa, kapan, bagaimana |
         | 18 | ADJP | Adjective Phrase. A group of words headed by an adjective that describes a noun or a pronoun | sangat tinggi |
         | 19 | DP | Date Phrase. Date written with whitespaces | 1 Januari 2020 |
         | 20 | NP | Noun Phrase. A phrase that has a noun (or indefinite pronoun) as its head | Jakarta Pusat, Lionel Messi |
         | 21 | NUMP | Number Phrase.  | 10 juta |
         | 22 | VP | Verb Phrase. A syntactic unit composed of at least one verb and its dependents | tidak makan |
+        
+        ### Stopword
+        
+        `nlp-id` also provide list of Indonesian stopword.
+        
+            from nlp_id.stopword import StopWord 
+            stopword = StopWord() 
+            stopword.get_stopword() 
+            # [{list_of_nlp_id_stopword}]    
+        
+        Stopword Removal is used to remove every Indonesian stopword from the given text.
+        
+            from nlp_id.stopword import StopWord 
+            text = "Lionel Messi pergi Ke pasar di area Jakarta Pusat" # single sentence
+            stopword = StopWord() 
+            stopword.remove_stopword(text)
+            # Lionel Messi pergi pasar area Jakarta Pusat  
+            
+            paragraph = "Lionel Messi pergi Ke pasar di area Jakarta Pusat itu. Sedangkan Cristiano Ronaldo ke pasar Di area Jakarta Selatan. Dan mereka tidak bertemu begini-begitu."
+            stopword.remove_stopword(text)
+            # Lionel Messi pergi pasar area Jakarta Pusat. Cristiano Ronaldo pasar area Jakarta Selatan. bertemu.
 Keywords: Indonesian,Bahasa,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nlp_id-0.1.9.7/nlp_id/lemmatizer.py` & `nlp_id-0.1.9.8/nlp_id/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/postag.py` & `nlp_id-0.1.9.8/nlp_id/postag.py`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/data/root-word.txt` & `nlp_id-0.1.9.8/nlp_id/data/root-word.txt`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/data/lemma_dict.json` & `nlp_id-0.1.9.8/nlp_id/data/lemma_dict.json`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/data/dataset_postag.txt` & `nlp_id-0.1.9.8/nlp_id/data/dataset_postag.txt`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/data/stopword.txt` & `nlp_id-0.1.9.8/nlp_id/data/stopword.txt`

 * *Files identical despite different names*

### Comparing `nlp_id-0.1.9.7/nlp_id/tokenizer.py` & `nlp_id-0.1.9.8/nlp_id/tokenizer.py`

 * *Files identical despite different names*

