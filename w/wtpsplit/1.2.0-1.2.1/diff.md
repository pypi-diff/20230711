# Comparing `tmp/wtpsplit-1.2.0.tar.gz` & `tmp/wtpsplit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-8ira0x3h/wtpsplit-1.2.0.tar", last modified: Fri Jul  7 09:49:14 2023, max compression
+gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-2pycv7yb/wtpsplit-1.2.1.tar", last modified: Tue Jul 11 18:17:13 2023, max compression
```

## Comparing `wtpsplit-1.2.0.tar` & `wtpsplit-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/LICENSE
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    11432 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/README.md
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-04 15:41:03.000000 wtpsplit-1.2.0/pyproject.toml
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/setup.cfg
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-04 16:15:49.000000 wtpsplit-1.2.0/setup.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.404911 wtpsplit-1.2.0/wtpsplit/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14285 2023-07-04 16:15:58.000000 wtpsplit-1.2.0/wtpsplit/__init__.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-04 15:39:28.000000 wtpsplit-1.2.0/wtpsplit/configs.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/wtpsplit/data/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/language_info.csv
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/punctuation.json
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/punctuation.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5146 2023-07-04 15:54:05.000000 wtpsplit-1.2.0/wtpsplit/extract.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-04 16:15:50.000000 wtpsplit-1.2.0/wtpsplit/models.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6374 2023-07-04 16:15:57.000000 wtpsplit-1.2.0/wtpsplit/utils.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/wtpsplit.egg-info/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/requires.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/LICENSE
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    11432 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/README.md
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/pyproject.toml
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/setup.cfg
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-11 18:16:23.000000 wtpsplit-1.2.1/setup.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14323 2023-07-11 18:13:22.000000 wtpsplit-1.2.1/wtpsplit/__init__.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/configs.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit/data/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/language_info.csv
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/punctuation.json
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/punctuation.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5384 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/extract.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/models.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6374 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/utils.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit.egg-info/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/requires.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.2.0/LICENSE` & `wtpsplit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/README.md` & `wtpsplit-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/setup.py` & `wtpsplit-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="wtpsplit",
-    version="1.2.0",
+    version="1.2.1",
     packages=["wtpsplit"],
     description="Robust, adaptible sentence segmentation for 85 languages",
     author="Benjamin Minixhofer",
     author_email="bminixhofer@gmail.com",
     install_requires=[
         "onnxruntime>=1.13.1",
         "transformers>=4.22.2",
```

### Comparing `wtpsplit-1.2.0/wtpsplit/__init__.py` & `wtpsplit-1.2.1/wtpsplit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import skops.io as sio
 from transformers import AutoConfig, AutoModelForTokenClassification
 from transformers.utils.hub import cached_file
 
 from wtpsplit.extract import ORTWrapper, PyTorchWrapper, extract
 from wtpsplit.utils import Constants, indices_to_sentences, sigmoid
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 class WtP:
     def __init__(
         self,
         model_name_or_model,
         from_pretrained_kwargs=None,
@@ -108,14 +108,15 @@
                 mixture_path,
                 ["numpy.float32", "numpy.float64", "sklearn.linear_model._logistic.LogisticRegression"],
             )
         else:
             self.mixtures = None
 
     def __getattr__(self, name):
+        assert hasattr(self, "model")
         return getattr(self.model, name)
 
     def predict_proba(
         self,
         text_or_texts,
         lang_code: str = None,
         style: str = None,
```

### Comparing `wtpsplit-1.2.0/wtpsplit/configs.py` & `wtpsplit-1.2.1/wtpsplit/configs.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/wtpsplit/data/language_info.csv` & `wtpsplit-1.2.1/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/wtpsplit/data/punctuation.json` & `wtpsplit-1.2.1/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/wtpsplit/extract.py` & `wtpsplit-1.2.1/wtpsplit/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 
 class ORTWrapper:
     def __init__(self, config, ort_session):
         self.config = config
         self.ort_session = ort_session
 
+    def __getattr__(self, name):
+        assert hasattr(self, "ort_session")
+        return getattr(self.ort_session, name)
+
     def __call__(self, hashed_ids, attention_mask):
         logits = self.ort_session.run(
             ["logits"],
             {
                 "attention_mask": attention_mask,
                 "hashed_ids": hashed_ids,
             },
@@ -25,14 +29,18 @@
 
 
 class PyTorchWrapper:
     def __init__(self, model):
         self.model = model
         self.config = model.config
 
+    def __getattr__(self, name):
+        assert hasattr(self, "model")
+        return getattr(self.model, name)
+
     def __call__(self, hashed_ids, attention_mask, language_ids=None):
         try:
             import torch
         except ImportError:
             raise ImportError("`torch` must be installed to use PyTorch models!")
 
         with torch.no_grad():
```

### Comparing `wtpsplit-1.2.0/wtpsplit/models.py` & `wtpsplit-1.2.1/wtpsplit/models.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.0/wtpsplit/utils.py` & `wtpsplit-1.2.1/wtpsplit/utils.py`

 * *Files identical despite different names*

