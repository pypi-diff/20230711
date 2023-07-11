# Comparing `tmp/datatransform-1.6.tar.gz` & `tmp/datatransform-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.6.tar", last modified: Tue Jul 11 00:08:42 2023, max compression
+gzip compressed data, was "datatransform-1.7.tar", last modified: Tue Jul 11 00:23:53 2023, max compression
```

## Comparing `datatransform-1.6.tar` & `datatransform-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.786171 datatransform-1.6/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:08:42.786047 datatransform-1.6/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.785390 datatransform-1.6/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-10 23:37:41.000000 datatransform-1.6/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1369 2023-07-10 23:25:01.000000 datatransform-1.6/datatransform/datatransform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      769 2023-07-10 23:19:09.000000 datatransform-1.6/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1540 2023-07-10 23:37:47.000000 datatransform-1.6/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      996 2023-07-10 23:37:44.000000 datatransform-1.6/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.785888 datatransform-1.6/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-11 00:08:42.786207 datatransform-1.6/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-11 00:08:07.000000 datatransform-1.6/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:23:53.418778 datatransform-1.7/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:23:53.418651 datatransform-1.7/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:23:53.417993 datatransform-1.7/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-10 23:37:41.000000 datatransform-1.7/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1369 2023-07-10 23:25:01.000000 datatransform-1.7/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1024 2023-07-11 00:17:12.000000 datatransform-1.7/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1539 2023-07-11 00:17:23.000000 datatransform-1.7/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      996 2023-07-10 23:37:44.000000 datatransform-1.7/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:23:53.418485 datatransform-1.7/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:23:53.000000 datatransform-1.7/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-11 00:23:53.000000 datatransform-1.7/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-11 00:23:53.000000 datatransform-1.7/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-11 00:23:53.000000 datatransform-1.7/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-11 00:23:53.418847 datatransform-1.7/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-11 00:17:34.000000 datatransform-1.7/setup.py
```

### Comparing `datatransform-1.6/datatransform/datatransform.py` & `datatransform-1.7/datatransform/datatransform.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.6/datatransform/leave_one_out.py` & `datatransform-1.7/datatransform/leave_one_out.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from category_encoders import LeaveOneOutEncoder
+from keras.utils import to_categorical
 from .datatransform import Data_Transform
 
 class LeaveOneOut:
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
         y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
 
         encoder = LeaveOneOutEncoder(cols=X_train.columns)
         X_train = encoder.fit_transform(X_train, y_train)
         X_val = encoder.transform(X_val)
         X_test = encoder.transform(X_test)
+
+        num_classes = 3
+        y_train_cat= to_categorical(y_train, num_classes)
+        y_test_cat = to_categorical(y_test, num_classes)
+        y_val_cat = to_categorical(y_val, num_classes)
+        
         n_components = len(X_train.columns)
 
-        return X_train, X_test, X_val, y_train, y_test, y_val, output_size, n_components
+        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat, output_size, n_components
```

### Comparing `datatransform-1.6/datatransform/mca.py` & `datatransform-1.7/datatransform/mca.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         X_train = mca.fit_transform(X_train)
         X_test = mca.fit_transform(X_test)
         X_val = mca.fit_transform(X_val)
         return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat, output_size, n_components
 
     def get_n_components(self, data, threshold=0.9):
         covariance_matrix = np.cov(data.values.T)
-        eigenvalues, _ = np.linalg.eigv(covariance_matrix)
+        eigenvalues, _ = np.linalg.eig(covariance_matrix)
         total_variance = np.sum(eigenvalues)
         explained_variance_ratio = eigenvalues / total_variance
         cumulative_explained_variance = np.cumsum(explained_variance_ratio)
         n_components = np.argmax(cumulative_explained_variance >= threshold) + 1
         return n_components
```

### Comparing `datatransform-1.6/datatransform/pca.py` & `datatransform-1.7/datatransform/pca.py`

 * *Files identical despite different names*

