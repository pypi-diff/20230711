# Comparing `tmp/datatransform-1.5.tar.gz` & `tmp/datatransform-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.5.tar", last modified: Mon Jul 10 23:28:26 2023, max compression
+gzip compressed data, was "datatransform-1.6.tar", last modified: Tue Jul 11 00:08:42 2023, max compression
```

## Comparing `datatransform-1.5.tar` & `datatransform-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.119149 datatransform-1.5/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 23:28:26.119041 datatransform-1.5/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.118423 datatransform-1.5/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.5/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1369 2023-07-10 23:25:01.000000 datatransform-1.5/datatransform/datatransform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      769 2023-07-10 23:19:09.000000 datatransform-1.5/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1540 2023-07-10 23:23:47.000000 datatransform-1.5/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      996 2023-07-10 23:25:23.000000 datatransform-1.5/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 23:28:26.118896 datatransform-1.5/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 23:28:26.000000 datatransform-1.5/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 23:28:26.119182 datatransform-1.5/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 23:27:22.000000 datatransform-1.5/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.786171 datatransform-1.6/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:08:42.786047 datatransform-1.6/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.785390 datatransform-1.6/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-10 23:37:41.000000 datatransform-1.6/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1369 2023-07-10 23:25:01.000000 datatransform-1.6/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      769 2023-07-10 23:19:09.000000 datatransform-1.6/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1540 2023-07-10 23:37:47.000000 datatransform-1.6/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      996 2023-07-10 23:37:44.000000 datatransform-1.6/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-11 00:08:42.785888 datatransform-1.6/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-11 00:08:42.000000 datatransform-1.6/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-11 00:08:42.786207 datatransform-1.6/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-11 00:08:07.000000 datatransform-1.6/setup.py
```

### Comparing `datatransform-1.5/datatransform/datatransform.py` & `datatransform-1.6/datatransform/datatransform.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.5/datatransform/leave_one_out.py` & `datatransform-1.6/datatransform/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.5/datatransform/mca.py` & `datatransform-1.6/datatransform/mca.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 import prince
 from keras.utils import to_categorical
 from .datatransform import Data_Transform
 
 
-class MCA():
+class mca():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
         y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
         num_classes = 3
```

### Comparing `datatransform-1.5/datatransform/pca.py` & `datatransform-1.6/datatransform/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 from sklearn.decomposition import PCA
 from keras.utils import to_categorical
 from .datatransform import Data_Transform
 
-class PCA():
+class pca():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y, output_size = data_transformer.ready_data(data)
         X = pd.get_dummies(X)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
         y_train, y_test, y_val = data_transformer.label_encode(y_train, y_test, y_val)
```

