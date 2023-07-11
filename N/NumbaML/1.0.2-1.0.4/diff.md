# Comparing `tmp/NumbaML-1.0.2.tar.gz` & `tmp/NumbaML-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NumbaML-1.0.2.tar", last modified: Tue Jul 11 06:36:17 2023, max compression
+gzip compressed data, was "NumbaML-1.0.4.tar", last modified: Tue Jul 11 07:41:08 2023, max compression
```

## Comparing `NumbaML-1.0.2.tar` & `NumbaML-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/NumbaML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 06:36:17.000000 NumbaML-1.0.2/NumbaML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-11 06:36:17.285541 NumbaML-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-11 06:36:05.000000 NumbaML-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/numbaml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-11 06:36:05.000000 NumbaML-1.0.2/numbaml/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:36:17.285541 NumbaML-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 06:36:05.000000 NumbaML-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:36:17.285541 NumbaML-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-11 06:36:05.000000 NumbaML-1.0.2/tests/test_linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:41:08.508577 NumbaML-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:41:08.508577 NumbaML-1.0.4/NumbaML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-11 07:41:08.000000 NumbaML-1.0.4/NumbaML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 07:41:08.000000 NumbaML-1.0.4/NumbaML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:41:08.000000 NumbaML-1.0.4/NumbaML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 07:41:08.000000 NumbaML-1.0.4/NumbaML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 07:41:08.000000 NumbaML-1.0.4/NumbaML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-11 07:41:08.508577 NumbaML-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-11 07:40:53.000000 NumbaML-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:41:08.508577 NumbaML-1.0.4/numbaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-11 07:40:53.000000 NumbaML-1.0.4/numbaml/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 07:41:08.508577 NumbaML-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 07:40:53.000000 NumbaML-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:41:08.508577 NumbaML-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-11 07:40:53.000000 NumbaML-1.0.4/tests/test_linear_model.py
```

### Comparing `NumbaML-1.0.2/NumbaML.egg-info/PKG-INFO` & `NumbaML-1.0.4/NumbaML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumbaML
-Version: 1.0.2
+Version: 1.0.4
 Summary: Linear regression with Numba
 Home-page: https://github.com/jcatankard/NumbaML
 Author: Josh Tankard
 Description-Content-Type: text/markdown
 
 # Regression modelling with Numba
 
@@ -159,15 +159,14 @@
     ```
 
 #### conf_int_dict
 Return parameter estimates and confidence intervals as a dictionary that can easily been turned into a Pandas DataFrame.
 If there are feature names seen in the X variables passed to "fit", they will output in the "feature_name" column.
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import pandas as pd
 
 
 X, y = make_regression(random_state=2)
 
@@ -198,41 +197,26 @@
 #### model_outliers
 It is possible to detect which data points in the training data have an out-sized influence on the model
 by using leave-one-out cv. These datapoints may need investigating
 and if necessary removed from the training data before re-fitting. 
 
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import numpy as np
 
 
 X, y = make_regression(random_state=2)
-
-# train
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+
 m = Ridge(alpha=1)
 m.fit(X_train, y_train)
-
-# evaluate
 preds = m.predict(X_test)
-print('original mse:', round(mean_squared_error(y_test, preds), 4))
 
 # flag outliers
 z_scores = m.model_outliers()
 z_threshold = 4
 outliers = np.abs(z_scores) > z_threshold
 print('number of outliers:', z_scores[outliers].size, 'out of:', z_scores.size)
 
-# re-train
-X_train, y_train = X_train[~outliers], y_train[~outliers]
-m = Ridge(alpha=1)
-m.fit(X_train, y_train)
-z_scores = m.model_outliers()
-
-# evaluate
-preds = m.predict(X_test)
-print('new mse:', round(mean_squared_error(y_test, preds), 4))
-
 ```
```

### Comparing `NumbaML-1.0.2/PKG-INFO` & `NumbaML-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumbaML
-Version: 1.0.2
+Version: 1.0.4
 Summary: Linear regression with Numba
 Home-page: https://github.com/jcatankard/NumbaML
 Author: Josh Tankard
 Description-Content-Type: text/markdown
 
 # Regression modelling with Numba
 
@@ -159,15 +159,14 @@
     ```
 
 #### conf_int_dict
 Return parameter estimates and confidence intervals as a dictionary that can easily been turned into a Pandas DataFrame.
 If there are feature names seen in the X variables passed to "fit", they will output in the "feature_name" column.
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import pandas as pd
 
 
 X, y = make_regression(random_state=2)
 
@@ -198,41 +197,26 @@
 #### model_outliers
 It is possible to detect which data points in the training data have an out-sized influence on the model
 by using leave-one-out cv. These datapoints may need investigating
 and if necessary removed from the training data before re-fitting. 
 
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import numpy as np
 
 
 X, y = make_regression(random_state=2)
-
-# train
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+
 m = Ridge(alpha=1)
 m.fit(X_train, y_train)
-
-# evaluate
 preds = m.predict(X_test)
-print('original mse:', round(mean_squared_error(y_test, preds), 4))
 
 # flag outliers
 z_scores = m.model_outliers()
 z_threshold = 4
 outliers = np.abs(z_scores) > z_threshold
 print('number of outliers:', z_scores[outliers].size, 'out of:', z_scores.size)
 
-# re-train
-X_train, y_train = X_train[~outliers], y_train[~outliers]
-m = Ridge(alpha=1)
-m.fit(X_train, y_train)
-z_scores = m.model_outliers()
-
-# evaluate
-preds = m.predict(X_test)
-print('new mse:', round(mean_squared_error(y_test, preds), 4))
-
 ```
```

### Comparing `NumbaML-1.0.2/README.md` & `NumbaML-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -151,15 +151,14 @@
     ```
 
 #### conf_int_dict
 Return parameter estimates and confidence intervals as a dictionary that can easily been turned into a Pandas DataFrame.
 If there are feature names seen in the X variables passed to "fit", they will output in the "feature_name" column.
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import pandas as pd
 
 
 X, y = make_regression(random_state=2)
 
@@ -190,41 +189,26 @@
 #### model_outliers
 It is possible to detect which data points in the training data have an out-sized influence on the model
 by using leave-one-out cv. These datapoints may need investigating
 and if necessary removed from the training data before re-fitting. 
 
 ```
 from numbaml.linear_model import Ridge
-from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_regression
 import numpy as np
 
 
 X, y = make_regression(random_state=2)
-
-# train
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+
 m = Ridge(alpha=1)
 m.fit(X_train, y_train)
-
-# evaluate
 preds = m.predict(X_test)
-print('original mse:', round(mean_squared_error(y_test, preds), 4))
 
 # flag outliers
 z_scores = m.model_outliers()
 z_threshold = 4
 outliers = np.abs(z_scores) > z_threshold
 print('number of outliers:', z_scores[outliers].size, 'out of:', z_scores.size)
 
-# re-train
-X_train, y_train = X_train[~outliers], y_train[~outliers]
-m = Ridge(alpha=1)
-m.fit(X_train, y_train)
-z_scores = m.model_outliers()
-
-# evaluate
-preds = m.predict(X_test)
-print('new mse:', round(mean_squared_error(y_test, preds), 4))
-
 ```
```

### Comparing `NumbaML-1.0.2/numbaml/confidence_intervals.py` & `NumbaML-1.0.4/numbaml/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/numbaml/fit.py` & `NumbaML-1.0.4/numbaml/fit.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/numbaml/linear_model.py` & `NumbaML-1.0.4/numbaml/linear_model.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/numbaml/metrics.py` & `NumbaML-1.0.4/numbaml/metrics.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/numbaml/model_selection.py` & `NumbaML-1.0.4/numbaml/model_selection.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/numbaml/scoring.py` & `NumbaML-1.0.4/numbaml/scoring.py`

 * *Files identical despite different names*

### Comparing `NumbaML-1.0.2/tests/test_linear_model.py` & `NumbaML-1.0.4/tests/test_linear_model.py`

 * *Files identical despite different names*

