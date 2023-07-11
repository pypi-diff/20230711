# Comparing `tmp/aidetector-0.0.1.tar.gz` & `tmp/aidetector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidetector-0.0.1.tar", last modified: Wed Jun 28 15:34:34 2023, max compression
+gzip compressed data, was "aidetector-0.0.2.tar", last modified: Tue Jul 11 19:46:38 2023, max compression
```

## Comparing `aidetector-0.0.1.tar` & `aidetector-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:34:34.610322 aidetector-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 15:34:25.000000 aidetector-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-28 15:34:34.610322 aidetector-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-28 15:34:25.000000 aidetector-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:34:34.610322 aidetector-0.0.1/aidetector/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/aidetectorclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/command_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-28 15:34:25.000000 aidetector-0.0.1/aidetector/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:34:34.610322 aidetector-0.0.1/aidetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 15:34:34.000000 aidetector-0.0.1/aidetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:34:34.610322 aidetector-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-28 15:34:25.000000 aidetector-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:46:38.721948 aidetector-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 19:46:27.000000 aidetector-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-11 19:46:38.721948 aidetector-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-11 19:46:27.000000 aidetector-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:46:38.717947 aidetector-0.0.2/aidetector/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/aidetectorclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/command_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-11 19:46:27.000000 aidetector-0.0.2/aidetector/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:46:38.717947 aidetector-0.0.2/aidetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 19:46:38.000000 aidetector-0.0.2/aidetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:46:38.721948 aidetector-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-11 19:46:27.000000 aidetector-0.0.2/setup.py
```

### Comparing `aidetector-0.0.1/LICENSE` & `aidetector-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aidetector-0.0.1/PKG-INFO` & `aidetector-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aidetector
-Version: 0.0.1
+Version: 0.0.2
 Summary: AiDetector provides a simple interface to train and run models to classify if text was generated by AI or not.
 Home-page: https://github.com/baileytec-labs
 Author: Sean Bailey
 Author-email: seanbailey518@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -50,15 +50,15 @@
 aidetector train --datafile [path_to_data] --modeloutputfile [path_to_model] --vocaboutputfile [path_to_vocab] --tokenmodel [SpaCy model] --percentsplit [percentage_for_test_split] --classificationlabel [classification_label_in_data] --textlabel [text_label_in_data] --download  --lowerbound [lower_bound_for_early_stopping] --upperbound [upper_bound_for_early_stopping] --epochs [number_of_epochs]
 ```
 
 ### Inference
 To make predictions with a trained model, you need to provide the text you want to classify. The script takes the following command-line arguments:
 
 ```
-aidetection infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
+aidetector infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
 ```
 
 
 The prediction will be printed to the console: "This was written by AI" or "This was written by a human."
 
 ___
```

### Comparing `aidetector-0.0.1/README.md` & `aidetector-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 aidetector train --datafile [path_to_data] --modeloutputfile [path_to_model] --vocaboutputfile [path_to_vocab] --tokenmodel [SpaCy model] --percentsplit [percentage_for_test_split] --classificationlabel [classification_label_in_data] --textlabel [text_label_in_data] --download  --lowerbound [lower_bound_for_early_stopping] --upperbound [upper_bound_for_early_stopping] --epochs [number_of_epochs]
 ```
 
 ### Inference
 To make predictions with a trained model, you need to provide the text you want to classify. The script takes the following command-line arguments:
 
 ```
-aidetection infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
+aidetector infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
 ```
 
 
 The prediction will be printed to the console: "This was written by AI" or "This was written by a human."
 
 ___
```

### Comparing `aidetector-0.0.1/aidetector/aidetectorclass.py` & `aidetector-0.0.2/aidetector/aidetectorclass.py`

 * *Files identical despite different names*

### Comparing `aidetector-0.0.1/aidetector/command_interface.py` & `aidetector-0.0.2/aidetector/command_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     parser_infer.add_argument('--threshold',type=float,required=False,default=0.5,help="The threshold to determine if the input is AI or not. Default 0.5")
     parser_infer.add_argument('--download', dest='download', action='store_true', help='Download the model you have specified or the default of xx_ent_wiki_sm')
     
     parser_infer.set_defaults(download=False) 
     args = parser.parse_args()
 
     if args.mode == 'train':
-        tokenizer=get_tokenizer(args.tokenmodel)
+        tokenizer=get_tokenizer(args.tokenmodel,args.download)
         traintxt, test_text, train_labels, test_labels = load_data(args.datafile,percentsplit=args.percentsplit,classificationlabel=args.classificationlabel,textlabel=args.textlabel)
         vocab, trainseqs, testseqs = tokenize_data(
             traintxt,
             test_text,
             tokenizer
             
         )
```

### Comparing `aidetector-0.0.1/aidetector/inference.py` & `aidetector-0.0.2/aidetector/inference.py`

 * *Files identical despite different names*

### Comparing `aidetector-0.0.1/aidetector/tokenization.py` & `aidetector-0.0.2/aidetector/tokenization.py`

 * *Files identical despite different names*

### Comparing `aidetector-0.0.1/aidetector/training.py` & `aidetector-0.0.2/aidetector/training.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,27 @@
 from torch import nn
 from sklearn.model_selection import train_test_split
 import torch
 import torch.optim as optim
 import pickle
 
 
+def detect_delimiter(filename, col1, col2):
+    with open(filename, 'r') as f:
+        first_line = f.readline()
+    parts = first_line.split(col1)
+    if len(parts) < 2:
+        raise ValueError(f"Couldn't find column name {col1} in the first line of the file")
+    second_part = parts[1]
+    parts = second_part.split(col2)
+    if len(parts) < 2:
+        raise ValueError(f"Couldn't find column name {col2} in the first line of the file")
+    delimiter = parts[0]
+    return delimiter
+
 
 #Data loading...
 def load_data(inputfile, percentsplit=0.2,classificationlabel='classification',textlabel='text'):
     """
     Load data from a CSV file and split it into training and testing sets.
 
     Parameters:
@@ -28,17 +41,18 @@
     percentsplit (float, optional): Fraction of the data to be used as a test set. Default is 0.2.
     classificationlabel (str, optional): Column label for classification. Default is 'classification'.
     textlabel (str, optional): Column label for text. Default is 'text'.
 
     Returns:
     tuple: Four pandas Series objects for training text, testing text, training labels, and testing labels.
     """
-
+    delimeter=detect_delimiter(inputfile,classificationlabel,textlabel)
     df = pd.read_csv(
-        inputfile
+        inputfile,
+        sep=delimeter
     )
     traintxt, testtxt, trainlbl, testlbl = train_test_split(
         df[textlabel],
         df[classificationlabel],
         test_size=percentsplit
     )
```

### Comparing `aidetector-0.0.1/aidetector.egg-info/PKG-INFO` & `aidetector-0.0.2/aidetector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aidetector
-Version: 0.0.1
+Version: 0.0.2
 Summary: AiDetector provides a simple interface to train and run models to classify if text was generated by AI or not.
 Home-page: https://github.com/baileytec-labs
 Author: Sean Bailey
 Author-email: seanbailey518@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -50,15 +50,15 @@
 aidetector train --datafile [path_to_data] --modeloutputfile [path_to_model] --vocaboutputfile [path_to_vocab] --tokenmodel [SpaCy model] --percentsplit [percentage_for_test_split] --classificationlabel [classification_label_in_data] --textlabel [text_label_in_data] --download  --lowerbound [lower_bound_for_early_stopping] --upperbound [upper_bound_for_early_stopping] --epochs [number_of_epochs]
 ```
 
 ### Inference
 To make predictions with a trained model, you need to provide the text you want to classify. The script takes the following command-line arguments:
 
 ```
-aidetection infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
+aidetector infer --modelfile [path_to_trained_model] --vocabfile [path_to_vocab] --text [text_to_classify] --tokenmodel [SpaCy_model] --threshold [probability_threshold_for_classification] --download [flag_to_download_SpaCy_model]
 ```
 
 
 The prediction will be printed to the console: "This was written by AI" or "This was written by a human."
 
 ___
```

### Comparing `aidetector-0.0.1/setup.py` & `aidetector-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 print(find_packages())
 
 setup(
     name='aidetector',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": ["aidetector=aidetector.command_interface:main"]
     },
     author="Sean Bailey",
     author_email="seanbailey518@gmail.com",
```

