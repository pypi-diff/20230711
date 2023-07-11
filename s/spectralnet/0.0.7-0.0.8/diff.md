# Comparing `tmp/spectralnet-0.0.7.tar.gz` & `tmp/spectralnet-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.7.tar", last modified: Tue Jul  4 19:55:36 2023, max compression
+gzip compressed data, was "spectralnet-0.0.8.tar", last modified: Tue Jul 11 17:44:13 2023, max compression
```

## Comparing `spectralnet-0.0.7.tar` & `spectralnet-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091422 spectralnet-0.0.7/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.7/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-04 19:55:36.091535 spectralnet-0.0.7/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     1768 2023-07-04 19:51:11.000000 spectralnet-0.0.7/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.7/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      615 2023-07-04 19:55:36.091822 spectralnet-0.0.7/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.7/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.085194 spectralnet-0.0.7/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.087241 spectralnet-0.0.7/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.088620 spectralnet-0.0.7/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.089454 spectralnet-0.0.7/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091124 spectralnet-0.0.7/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.088034 spectralnet-0.0.7/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      845 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       18 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/top_level.txt
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091315 spectralnet-0.0.7/src/tests/
--rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 18:58:30.000000 spectralnet-0.0.7/src/tests/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.555530 spectralnet-0.0.8/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-07-10 18:21:28.000000 spectralnet-0.0.8/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-11 17:44:13.555615 spectralnet-0.0.8/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1768 2023-07-10 18:21:28.000000 spectralnet-0.0.8/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-07-10 18:21:28.000000 spectralnet-0.0.8/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      615 2023-07-11 17:44:13.555898 spectralnet-0.0.8/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-07-10 18:21:28.000000 spectralnet-0.0.8/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.549705 spectralnet-0.0.8/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.552071 spectralnet-0.0.8/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      136 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.553452 spectralnet-0.0.8/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.554254 spectralnet-0.0.8/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.555261 spectralnet-0.0.8/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-07-11 17:41:13.000000 spectralnet-0.0.8/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11939 2023-07-10 18:31:21.000000 spectralnet-0.0.8/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.552837 spectralnet-0.0.8/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-11 17:44:13.000000 spectralnet-0.0.8/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      845 2023-07-11 17:44:13.000000 spectralnet-0.0.8/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-07-11 17:44:13.000000 spectralnet-0.0.8/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       18 2023-07-11 17:44:13.000000 spectralnet-0.0.8/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-11 17:44:13.555435 spectralnet-0.0.8/src/tests/
+-rw-r--r--   0 amitai     (501) staff       (20)        0 2023-07-10 18:21:28.000000 spectralnet-0.0.8/src/tests/__init__.py
```

### Comparing `spectralnet-0.0.7/LICENSE.md` & `spectralnet-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/PKG-INFO` & `spectralnet-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spectralnet-0.0.7/README.md` & `spectralnet-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/setup.cfg` & `spectralnet-0.0.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.0.7
+version = 0.0.8
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shaham-lab/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/shaham-lab/SpectralNet/issues
```

### Comparing `spectralnet-0.0.7/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.8/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.8/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_metrics.py` & `spectralnet-0.0.8/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.8/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.8/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.8/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_spectral.py` & `spectralnet-0.0.8/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.8/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.8/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.8/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.7/src/spectralnet/_utils.py` & `spectralnet-0.0.8/src/spectralnet/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -390,14 +390,48 @@
         for i in range(len(Ids)):
             mask[i, Ids[i]] = 1
         W = W * mask
     sym_W = (W + torch.t(W)) / 2.0
     return sym_W
 
 
+def get_t_kernel(
+    D: torch.Tensor, Ids: np.ndarray, device: torch.device, is_local: bool = True
+) -> torch.Tensor:
+    """
+    Computes the t similarity function according to a given distance matrix D and a given scale.
+
+    Parameters
+    ----------
+    D : torch.Tensor
+        Distance matrix.
+    Ids : np.ndarray
+        Indices of the k nearest neighbors of each sample.
+    device : torch.device
+        Defaults to torch.device("cpu").
+    is_local : bool, optional
+        Determines whether the given scale is global or local. Defaults to True.
+
+    Returns
+    -------
+    torch.Tensor
+        Matrix W with t similarities.
+    """
+
+    W = torch.pow(1 + torch.pow(D, 2), -1)
+    if Ids is not None:
+        n, k = Ids.shape
+        mask = torch.zeros([n, n]).to(device=device)
+        for i in range(len(Ids)):
+            mask[i, Ids[i]] = 1
+        W = W * mask
+    sym_W = (W + W.T) / 2.0
+    return sym_W
+
+
 def plot_data_by_assignments(X, assignments: np.ndarray):
     """
     Plots the data with the assignments obtained from SpectralNet. Relevant only for 2D data.
 
     Parameters
     ----------
     X :
```

### Comparing `spectralnet-0.0.7/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.0.8/src/spectralnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spectralnet-0.0.7/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.8/src/spectralnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

