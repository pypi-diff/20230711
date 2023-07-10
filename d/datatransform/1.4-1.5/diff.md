# Comparing `tmp/datatransform-1.4.tar.gz` & `tmp/datatransform-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.4.tar", last modified: Mon Jul 10 20:29:34 2023, max compression
+gzip compressed data, was "datatransform-1.5.tar", last modified: Mon Jul 10 23:28:26 2023, max compression
```

## Comparing `datatransform-1.4.tar` & `datatransform-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.540568 datatransform-1.4/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 20:29:34.540440 datatransform-1.4/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.539514 datatransform-1.4/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.4/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1608 2023-07-10 17:17:05.000000 datatransform-1.4/datatransform/datatransform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      793 2023-07-10 17:38:12.000000 datatransform-1.4/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1318 2023-07-10 17:38:07.000000 datatransform-1.4/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      775 2023-07-10 18:16:49.000000 datatransform-1.4/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.540257 datatransform-1.4/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 20:29:34.540603 datatransform-1.4/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 20:23:26.000000 datatransform-1.4/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.119149 datatransform-1.5/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 23:28:26.119041 datatransform-1.5/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.118423 datatransform-1.5/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.5/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1369 2023-07-10 23:25:01.000000 datatransform-1.5/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      769 2023-07-10 23:19:09.000000 datatransform-1.5/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1540 2023-07-10 23:23:47.000000 datatransform-1.5/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      996 2023-07-10 23:25:23.000000 datatransform-1.5/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.118896 datatransform-1.5/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 23:28:26.119182 datatransform-1.5/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 23:27:22.000000 datatransform-1.5/setup.py
```

### Comparing `datatransform-1.4/datatransform/leave_one_out.py` & `datatransform-1.5/datatransform/leave_one_out.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 class LeaveOneOut:
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
-        y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
+        y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
 
         encoder = LeaveOneOutEncoder(cols=X_train.columns)
         X_train = encoder.fit_transform(X_train, y_train)
         X_val = encoder.transform(X_val)
         X_test = encoder.transform(X_test)
         n_components = len(X_train.columns)
 
-        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat, output_size, n_components
+        return X_train, X_test, X_val, y_train, y_test, y_val, output_size, n_components
```

### Comparing `datatransform-1.4/datatransform/mca.py` & `datatransform-1.5/datatransform/mca.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import numpy as np
 import pandas as pd
 import prince
+from keras.utils import to_categorical
 from .datatransform import Data_Transform
 
+
 class MCA():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
-        y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
+        y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
+        num_classes = 3
+        y_train_cat= to_categorical(y_train, num_classes)
+        y_test_cat = to_categorical(y_test, num_classes)
+        y_val_cat = to_categorical(y_val, num_classes)
 
         one_hot = pd.get_dummies(X)
         n_components = self.get_n_components(one_hot)
 
         mca = prince.MCA(n_components, n_iter=20, copy=True, check_input=True, engine='sklearn')
         X_train = mca.fit_transform(X_train)
         X_test = mca.fit_transform(X_test)
```

### Comparing `datatransform-1.4/datatransform/pca.py` & `datatransform-1.5/datatransform/pca.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import pandas as pd
 from sklearn.decomposition import PCA
+from keras.utils import to_categorical
 from .datatransform import Data_Transform
 
 class PCA():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X = pd.get_dummies(X)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
-        y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
+        y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
+        num_classes = 3
+        y_train_cat= to_categorical(y_train, num_classes)
+        y_test_cat = to_categorical(y_test, num_classes)
+        y_val_cat = to_categorical(y_val, num_classes)
 
         pca = PCA(n_components = 0.98)
         X_train = pca.fit_transform(X_train)
         X_test = pca.transform(X_test)
         X_val = pca.transform(X_val)
         n_components = pca.n_components_
```

