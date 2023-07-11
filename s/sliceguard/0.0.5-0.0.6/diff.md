# Comparing `tmp/sliceguard-0.0.5.tar.gz` & `tmp/sliceguard-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.5.tar", last modified: Fri Jul  7 08:35:45 2023, max compression
+gzip compressed data, was "sliceguard-0.0.6.tar", last modified: Tue Jul 11 15:32:51 2023, max compression
```

## Comparing `sliceguard-0.0.5.tar` & `sliceguard-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.5/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2907 2023-07-07 08:35:45.453053 sliceguard-0.0.5/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2251 2023-07-07 08:31:58.000000 sliceguard-0.0.5/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-07 08:33:44.000000 sliceguard-0.0.5/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 08:35:45.453053 sliceguard-0.0.5/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.5/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9222 2023-07-07 08:09:57.000000 sliceguard-0.0.5/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2907 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4644 2023-07-07 08:09:57.000000 sliceguard-0.0.5/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.6/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3862 2023-07-11 15:32:51.659112 sliceguard-0.0.6/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2023-07-11 15:29:58.000000 sliceguard-0.0.6/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1086 2023-07-11 15:30:09.000000 sliceguard-0.0.6/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 15:32:51.659112 sliceguard-0.0.6/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.6/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.6/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2843 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10187 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8224 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3862 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.6/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.5/LICENSE` & `sliceguard-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.5/PKG-INFO` & `sliceguard-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sliceguard
-Version: 0.0.5
-Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
-Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
-Project-URL: Homepage, https://github.com/Renumics/sliceguard
-Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center"><a href="https://github.com/Renumics/sliceguard"><img src="static/img/spotlight.svg" alt="Gray shape shifter" height="60"/></a></p>
 <h1 align="center">sliceguard</h1>
 <p align="center">Detect problematic data slices in unstructured and structured data fast.</p>
 
 <p align="center">
  	<a href="https://pypi.org/project/sliceguard/"><img src="https://img.shields.io/pypi/pyversions/sliceguard" height="20"/></a>
  	<a href="https://pypi.org/project/sliceguard/"><img src="https://img.shields.io/pypi/wheel/sliceguard" height="20"/></a>
@@ -59,10 +45,27 @@
     "prediction",
     wer_metric,
     metric_mode="min"
 )
 sg.report()
 ```
 
-For a more comprehensive tutorial check the following blog post on Medium:
+## 🔧 Use case-specific examples
+* [Detecting issues in automatic speech recognition (ASR) models](examples/audio_issues_commonvoice_whisper.ipynb)
+* [Detecting issues in audio datasets (condition monitoring)](examples/audio_issues_condition_monitoring_dcase.ipynb)
+
+
+Also check this post on Medium:
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
+
+## 🗺️ Public Roadmap
+- [x] Detection of problematic data slices
+- [x] Basic explanation of found issues via feature importances
+- [x] Limited embedding computation for images, audio, text
+- [ ] Extensive documentation and examples for common cases
+- [ ] Data connectors for faster application on common data formats
+- [ ] Improved explanations for found issues, e.g., via SHAP
+- [ ] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
+- [ ] Generation of a summary report doing predefined checks
+- [ ] Allow for control features in order to account for expected variations when running checks
+- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems
```

### Comparing `sliceguard-0.0.5/pyproject.toml` & `sliceguard-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -22,15 +22,16 @@
   "umap-learn >= 0.5.3",
   "transformers >= 4.30.2",
   "torch >= 2.0.1",
   "torchaudio >= 2.0.2",
   "sentence-transformers >= 2.2.1",
   "tqdm >= 4.65.0",
   "Pillow >= 9.5.0",
-  "renumics-spotlight >= 1.3.0rc2",
+  "renumics-spotlight >= 1.3.0rc3",
+  "pydantic < 2.0.0",
   "plotly >= 5.15.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Renumics/sliceguard"
 "Bug Tracker" = "https://github.com/Renumics/sliceguard/issues"
```

### Comparing `sliceguard-0.0.5/sliceguard/detection.py` & `sliceguard-0.0.6/sliceguard/detection.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.5/sliceguard/embedding_utils.py` & `sliceguard-0.0.6/sliceguard/embedding_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,81 @@
 # Embedding support for text, images, audio
 import pandas as pd
 from sentence_transformers import SentenceTransformer
-from transformers import AutoFeatureExtractor, ViTModel, ASTModel
+from transformers import AutoFeatureExtractor, AutoModel
 from tqdm import tqdm
 from PIL import Image
 import numpy as np
 import torch
 import torchaudio
 
-def generate_text_embeddings(texts):
-    model = SentenceTransformer("all-MiniLM-L6-v2")
+
+def generate_text_embeddings(texts, model_name="all-MiniLM-L6-v2", hf_auth_token=None):
+    model = SentenceTransformer(model_name, use_auth_token=hf_auth_token)
     embeddings = model.encode(texts)
     return embeddings
 
 
-
-def generate_image_embeddings(image_paths, model_name="google/vit-base-patch16-224"):
-    feature_extractor = AutoFeatureExtractor.from_pretrained(model_name)
+def generate_image_embeddings(
+    image_paths, model_name="google/vit-base-patch16-224", hf_auth_token=None
+):
+    feature_extractor = AutoFeatureExtractor.from_pretrained(
+        model_name, use_auth_token=hf_auth_token
+    )
     device = "cuda" if torch.cuda.is_available() else "cpu"
-    model = ViTModel.from_pretrained(
-        model_name, output_hidden_states=True
+    model = AutoModel.from_pretrained(
+        model_name, output_hidden_states=True, use_auth_token=hf_auth_token
     ).to(device)
     embeddings = []
     for i, image_path in enumerate(tqdm(image_paths)):
         try:
             with open(image_path, "rb") as f:
                 image = Image.open(f)
-                inputs = feature_extractor(images=image.convert("RGB"), return_tensors="pt").to(device)
+                inputs = feature_extractor(
+                    images=image.convert("RGB"), return_tensors="pt"
+                ).to(device)
                 with torch.no_grad():
                     outputs = model(**inputs)
-                emb = outputs.last_hidden_state[0,0].cpu().detach().numpy()
+                emb = outputs.last_hidden_state[0, 0].cpu().detach().numpy()
                 embeddings.append(emb)
                 image.close()
         except:
             embeddings.append(None)
             print(f"Could not generate embedding for {image_path}.")
-    embeddings = np.array([emb.tolist() if emb is not None else None for emb in embeddings])
+    embeddings = np.array(
+        [emb.tolist() if emb is not None else None for emb in embeddings]
+    )
     return embeddings
 
 
-
-def generate_audio_embeddings(audio_paths, model_name="MIT/ast-finetuned-audioset-10-10-0.4593"):
-    feature_extractor = AutoFeatureExtractor.from_pretrained(model_name)
+def generate_audio_embeddings(
+    audio_paths,
+    model_name="MIT/ast-finetuned-audioset-10-10-0.4593",
+    hf_auth_token=None,
+):
+    feature_extractor = AutoFeatureExtractor.from_pretrained(
+        model_name, use_auth_token=hf_auth_token
+    )
     device = "cuda" if torch.cuda.is_available() else "cpu"
-    model = ASTModel.from_pretrained(
-        model_name, output_hidden_states=True
+    model = AutoModel.from_pretrained(
+        model_name, output_hidden_states=True, use_auth_token=hf_auth_token
     ).to(device)
-    
-    
+
     embeddings = []
     for i, audio_path in enumerate(tqdm(audio_paths)):
-        # try: 
+        # try:
         y, sr = torchaudio.load(audio_path)
-        y = y.mean(0) # convert to mono
+        y = y.mean(0)  # convert to mono
 
         inputs = feature_extractor(y, sampling_rate=sr, return_tensors="pt").to(device)
         with torch.no_grad():
             outputs = model(**inputs)
-        emb = outputs.last_hidden_state[0,0].cpu().detach().numpy()
-        
+        emb = outputs.last_hidden_state[0, 0].cpu().detach().numpy()
+
         embeddings.append(emb)
         # except:
         #     embeddings.append(None)
         #     print(f"Could not generate embedding for {audio_path}.")
-    embeddings = np.array([emb.tolist() if emb is not None else None for emb in embeddings])
-    return embeddings
+    embeddings = np.array(
+        [emb.tolist() if emb is not None else None for emb in embeddings]
+    )
+    return embeddings
```

### Comparing `sliceguard-0.0.5/sliceguard/explanation.py` & `sliceguard-0.0.6/sliceguard/explanation.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,24 @@
             classification_data = np.concatenate(
                 (classification_data, df[col].values.reshape(-1, 1)), axis=1
             )
             feature_groups.append([current_feature_index])
             current_feature_index += 1
         elif feature_type == "nominal" or feature_type == "ordinal":
             label_encoder = LabelEncoder()
-            integer_encoded_data = label_encoder.fit_transform(
-                df[col].values
-            ).reshape(-1, 1)
+            integer_encoded_data = label_encoder.fit_transform(df[col].values).reshape(
+                -1, 1
+            )
             label_encoders[col] = label_encoder
             classification_data = np.concatenate(
                 (classification_data, integer_encoded_data), axis=1
             )
             feature_groups.append([current_feature_index])
             current_feature_index += 1
-        elif feature_type == "raw":
+        elif feature_type == "raw" or feature_type == "embedding":
             reduced_embeddings = prereduced_embeddings[col]
             classification_data = np.concatenate(
                 (classification_data, reduced_embeddings), axis=1
             )
 
             feature_groups.append(
                 list(
@@ -97,8 +97,8 @@
         # if f1 > 0.7: # only add explanation if it is succicient to classify cluster?
         importance_strings = []
         for f, i in zip(ordered_features[:3], ordered_importances[:3]):
             importance_strings.append(f"{f}, ({i:.2f})")
         issue_df.loc[issue_indices_pandas, "issue_explanation"] = ", ".join(
             importance_strings
         )
-    return issue_df
+    return issue_df
```

### Comparing `sliceguard-0.0.5/sliceguard/sliceguard.py` & `sliceguard-0.0.6/sliceguard/sliceguard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Supress numba deprecation warnings until umap fixes this
+import warnings
+from numba.core.errors import NumbaDeprecationWarning, NumbaPendingDeprecationWarning
+
+warnings.simplefilter("ignore", category=NumbaDeprecationWarning)
+warnings.simplefilter("ignore", category=NumbaPendingDeprecationWarning)
+
+# Real imports
 from typing import List, Literal, Dict, Callable
 
 import pandas as pd
 import numpy as np
 import plotly.express as px
 
 from renumics import spotlight
@@ -22,55 +30,74 @@
     def find_issues(
         self,
         data: pd.DataFrame,
         features: List[str],
         y: str,
         y_pred: str,
         metric: Callable,
+        min_support: int = None,
+        min_drop: float = None,
         metric_mode: Literal["min", "max"] = "max",
         feature_types: Dict[
-            str, Literal["raw", "nominal", "ordinal", "numerical"]
+            str, Literal["raw", "nominal", "ordinal", "numerical", "embedding"]
         ] = {},
         feature_orders: Dict[str, list] = {},
         precomputed_embeddings: Dict[str, np.array] = {},
-        min_support: int = None,
-        min_drop: float = None,
+        embedding_models: Dict[str, str] = {},
+        hf_auth_token=None,
     ):
         """
         Find slices that are classified badly by your model.
 
         :param data: A pandas dataframe containing your data.
         :param features: A list of columns that contains features to feed into your model but also metadata.
         :param y: The column containing the ground-truth label.
         :param y_pred: The column containing your models prediction.
         :param metric: A callable metric function that must correspond to the form metric(y_true, y_pred) -> scikit-learn style.
+        :min_support: Minimum support for clusters that are listed as issues. If you are more looking towards outliers choose small values, if you target biases choose higher values.
+        :min_drop: Minimum metric drop a cluster has to have to be counted as issue compared to the result on the whole dataset.
         :param metric_mode: What do you optimize your metric for? max is the right choice for accuracy while e.g. min is good for regression error.
         :param feature_types: Specify how your feature should be treated in encoding and normalizing.
         :param feature_orders: If your feature is ordinal, specify the order of that should be used for encoding. This is required for EVERY ordinal feature.
         :param precomputed_embeddings: Supply precomputed embeddings for raw columns. E.g. if repeatedly running checks on your data.
-        :min_support: Minimum support for clusters that are listed as issues. If you are more looking towards outliers choose small values, if you target biases choose higher values.
-        :min_drop: Minimum metric drop a cluster has to have to be counted as issue compared to the result on the whole dataset.
+        :param embedding_model: Supply embedding models that should be used to compute embedding vectors from raw data.
+        :param hf_auth_token: The authentification token used to download embedding models from the huggingface hub.
         """
 
         assert (
-            (all([f in data.columns for f in features]))
+            (
+                all(
+                    [
+                        (f in data.columns or f in precomputed_embeddings)
+                        for f in features
+                    ]
+                )
+            )
             and (y in data.columns)
             and (y_pred in data.columns)
         )  # check presence of all columns
         df = data  # just rename the variable for shorter naming
 
         # Try to infer the column dtypes
-        feature_types = infer_feature_types(features, feature_types, df)
+        feature_types = infer_feature_types(
+            features, feature_types, precomputed_embeddings, df
+        )
 
         # TODO: Potentially also explicitely check for univariate and bivariate fairness issues, however start with the more generic variant
         # See also connection with full report functionality. It makes sense to habe a feature and a samples based view!
 
         # Encode the features for clustering according to inferred types
         encoded_data, prereduced_embeddings, raw_embeddings = encode_normalize_features(
-            features, feature_types, feature_orders, precomputed_embeddings, df
+            features,
+            feature_types,
+            feature_orders,
+            precomputed_embeddings,
+            embedding_models,
+            hf_auth_token,
+            df,
         )
 
         # Perform detection of problematic clusters based on the given features
         # 1. A hierarchical clustering is performed and metrics are calculated for all hierarchies
         # 2. hierarchy level that is most indicative of a real problem is then determined
         # 3. the reason for the problem e.g. feature combination or rule that is characteristic for the cluster is determined.
```

### Comparing `sliceguard-0.0.5/sliceguard/utils.py` & `sliceguard-0.0.6/sliceguard/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,26 +10,34 @@
     generate_audio_embeddings,
     generate_text_embeddings,
 )
 
 
 def infer_feature_types(
     features,
-    given_feature_types: Dict[str, Literal["raw", "nominal", "ordinal", "numerical"]],
+    given_feature_types: Dict[
+        str, Literal["raw", "nominal", "ordinal", "numerical", "embedding"]
+    ],
+    precomputed_embeddings: Dict[str, np.array],
     df: pd.DataFrame,
 ):
     """
     Infer the datatypes of certain features based on their column data.
     :param features: The features that have to be inferred.
     :param given_feature_types: Feature types that are already defined by the user.
     :param df: The dataframe containing all the data.
     """
 
     feature_types = {}
     for col in features:
+        # check if the column is supplied in precomputed embeddings, then always use embedding feature type
+        if col in precomputed_embeddings:
+            feature_types[col] = "embedding"
+            continue
+
         col_dtype = df[col].dtype
 
         if col_dtype == "object" and col not in given_feature_types:
             num_unique_values = len(df[col].unique())
             if num_unique_values / len(df) > 0.5:
                 print(
                     f"Feature {col} was inferred as referring to raw data. If this is not the case, please specify in feature_types!"
@@ -47,24 +55,27 @@
             feature_types[col] = "numerical"
         else:
             assert given_feature_types[col] in (
                 "raw",
                 "nominal",
                 "ordinal",
                 "numerical",
+                "embedding",
             )
             feature_types[col] = given_feature_types[col]
     return feature_types
 
 
 def encode_normalize_features(
     features: List[str],
     feature_types: Dict[str, Literal["raw", "nominal", "ordinal", "numerical"]],
     feature_orders: Dict[str, list],
     precomputed_embeddings: Dict[str, np.array],
+    embedding_models: Dict[str, str],
+    hf_auth_token: str,
     df: pd.DataFrame,
 ):
     """
     :param features: Names of features that should be encoded and normalized for later processing.
     :param feature_types: The previously inferred or given types of the respective features.
     :param feature_orders: If ordinal features are present you have to supply an order for each of them.
     :param precomputed_embeddings: Precomputed embeddings that the user might supply.
@@ -103,33 +114,56 @@
             ordinal_data = OrdinalEncoder(categories=[feature_order]).fit_transform(
                 df[col].values.reshape(-1, 1)
             )
             ordinal_data = ordinal_data / (
                 len(feature_order) - 1
             )  # normalize with unique category count to make compatible with range of one hot encoding
             encoded_data = np.concatenate((encoded_data, ordinal_data), axis=1)
-        elif feature_type == "raw":
-            first_entry = df[col].iloc[0]
+        elif feature_type == "raw" or feature_type == "embedding":
+            # Print model that will be used for computing embeddings
+            if col in df.columns and col not in precomputed_embeddings:
+                model_name_param = (
+                    {"model_name": embedding_models[col]}
+                    if col in embedding_models
+                    else {}
+                )
+                if "model_name" in model_name_param:
+                    print(
+                        f"Using {model_name_param['model_name']} for computing embeddings for feature {col}."
+                    )
+                else:
+                    print(
+                        f"Using default model for computing embeddings for feature {col}."
+                    )
+            # Set first entry as for checking type of raw data.
+            if col in df.columns:
+                first_entry = df[col].iloc[0]
             if col in precomputed_embeddings:  # use precomputed embeddings when given
                 embeddings = precomputed_embeddings[col]
                 assert len(embeddings) == len(df)
             elif first_entry.lower().endswith(
                 ".wav"
             ):  # TODO: Improve data type inference for raw data
-                embeddings = generate_audio_embeddings(df[col].values)
+                embeddings = generate_audio_embeddings(
+                    df[col].values, **model_name_param
+                )
                 raw_embeddings[col] = embeddings
             elif (
                 first_entry.lower().endswith(".jpg")
                 or first_entry.lower().endswith(".jpeg")
                 or first_entry.lower().endswith(".png")
             ):
-                embeddings = generate_image_embeddings(df[col].values)
+                embeddings = generate_image_embeddings(
+                    df[col].values, **model_name_param
+                )
                 raw_embeddings[col] = embeddings
             else:  # Treat as text if nothing known
-                embeddings = generate_text_embeddings(df[col].values)
+                embeddings = generate_text_embeddings(
+                    df[col].values, **model_name_param
+                )
                 raw_embeddings[col] = embeddings
 
             # TODO: Potentially filter out entries without valid embedding or replace with mean?
             reduced_embeddings = umap.UMAP(
                 # n_neighbors=min(len(df) - 1, 30),
                 # min_dist=0.0,
                 n_components=2,
```

### Comparing `sliceguard-0.0.5/tests/test_sliceguard.py` & `sliceguard-0.0.6/tests/test_sliceguard.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,34 +129,35 @@
         ["path"],
         "label",
         "class",
         accuracy_score,
         metric_mode="max",
         # feature_types={"age": "ordinal"},
         # feature_orders={"age": ["", "teens", "twenties", "thirties", "fourties", "fifties", "sixties", "seventies", "eighties", "nineties"]},
+        embedding_models={"path": "superb/wav2vec2-base-superb-sid"},
         min_support=5,
         min_drop=0.1,
     )
 
-    computed_embeddings = sg.embeddings
+    # computed_embeddings = sg.embeddings
 
-    issue_df = sg.find_issues(
-        df,
-        ["path"],
-        "label",
-        "class",
-        accuracy_score,
-        metric_mode="max",
-        # feature_types={"age": "ordinal"},
-        # feature_orders={"age": ["", "teens", "twenties", "thirties", "fourties", "fifties", "sixties", "seventies", "eighties", "nineties"]},
-        precomputed_embeddings=computed_embeddings,
-        min_support=5,
-        min_drop=0.1,
-    )
+    # issue_df = sg.find_issues(
+    #     df,
+    #     ["path"],
+    #     "label",
+    #     "class",
+    #     accuracy_score,
+    #     metric_mode="max",
+    #     # feature_types={"age": "ordinal"},
+    #     # feature_orders={"age": ["", "teens", "twenties", "thirties", "fourties", "fifties", "sixties", "seventies", "eighties", "nineties"]},
+    #     precomputed_embeddings=computed_embeddings,
+    #     min_support=5,
+    #     min_drop=0.1,
+    # )
 
     sg.report(spotlight_dtype={"path": Audio})
 
 
 if __name__ == "__main__":
-    test_sliceguard_text()
+    # test_sliceguard_text()
     # test_sliceguard_images()
-    # test_sliceguard_audio()
+    test_sliceguard_audio()
```

