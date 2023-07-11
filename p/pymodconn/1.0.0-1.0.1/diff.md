# Comparing `tmp/pymodconn-1.0.0.tar.gz` & `tmp/pymodconn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodconn-1.0.0.tar", last modified: Tue Jul 11 10:33:17 2023, max compression
+gzip compressed data, was "pymodconn-1.0.1.tar", last modified: Tue Jul 11 11:11:08 2023, max compression
```

## Comparing `pymodconn-1.0.0.tar` & `pymodconn-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 10:33:06.000000 pymodconn-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-11 10:33:17.463890 pymodconn-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-11 10:33:06.000000 pymodconn-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.459890 pymodconn-1.0.0/pymodconn/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/Decoder_class_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/Encoder_class_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/MHA_block_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/RNN_block_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/TCN_addnorm_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/cit_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/pymodconn/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/configs/configs_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/keras_tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/model_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/model_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/utils_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/pymodconn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 10:33:17.463890 pymodconn-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 10:33:07.000000 pymodconn-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 11:10:56.000000 pymodconn-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-11 11:11:08.200735 pymodconn-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-11 11:10:56.000000 pymodconn-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/Decoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/Encoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/MHA_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/RNN_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/TCN_addnorm_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/cit_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/configs/configs_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/keras_tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/model_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/model_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/utils_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 11:11:08.200735 pymodconn-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 11:10:56.000000 pymodconn-1.0.1/setup.py
```

### Comparing `pymodconn-1.0.0/LICENSE` & `pymodconn-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/PKG-INFO` & `pymodconn-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,105 @@
-Metadata-Version: 2.1
-Name: pymodconn
-Version: 1.0.0
-Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
-Home-page: https://github.com/gaurav306/pymodconn
-Author: Gaurav Chaudhary
-Author-email: gaurav.chaudhary@ntnu.no
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pymodconn
-
-## _pymodconn_ : A Python package for developing modular sequence to sequence control oriented neural networks
-
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture1.jpg)
+# _pymodconn_ : A Python package for developing modular sequence to sequence control-oriented deep neural networks
+*To prevent plagarism, more details will be added here after the paper is published.*
 
-A Control-Oriented Neural Network (CONN) is an artificial neural network designed to predict the future behavior and response of highly complex dynamic systems, taking into account past known data and future known data.
+![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/FIG1.png)
 
-1. Past known data includes historical information such as weather data, system dynamics, and control inputs, which is used to train the neural network to understand the relationships between these variables and their effects on the system.
-2. Future known data encompasses forecasted weather data and targeted control inputs, representing the expected conditions and desired actions that the system will be subject to in the future.
+A control-oriented deep neural network (CONN) is a deep neural network designed to predict the future behaviour and response of complex dynamic systems, taking into account *Known past data* and *Known future data*. 
+- *Known past data* includes historical information such as weather data, time information, system dynamics, and control inputs, which are used to train the CONN to understand the relationships between these variables and their effects on the system. 
+- *Known future data* encompasses forecasted weather data, time information, schedules, and most importantly targeted control inputs, representing the expected conditions and desired actions that the system will be subject to in the future. 
 
-The neural network leverages this information to predict future unknown data, referring to the system dynamics or states that are not yet known. This prediction enables the control system to anticipate changes in the environment and adapt its actions accordingly, ensuring optimal performance and robustness in the face of uncertainties.
-
-CONN is particularly useful in applications where systems are affected by external factors (such as weather) and require precise control over their dynamics, such as energy management systems, water resource management, and other infrastructure systems that must be optimized to ensure reliability and efficiency.
+The CONN leverages this information to predict future, i.e., *Unknown future data*, referring to the system dynamics or states that are not yet known. This prediction enables the control system to anticipate changes in the environment and adapt its actions, accordingly, ensuring optimal performance and robustness in spite of uncertainties.
 
 ## Instructions
 
 ### 1. Install:
 ```
 pip install pymodconn
 ```
 ### 2. Usage:
 Download congifuration file from [pymodconn\configs\default_config.yaml]
 
 ```python
+import multiprocessing
 import numpy as np
-from pymodconn.configs_init import get_configs
+import sys
 from pymodconn import Model_Gen
+from pymodconn.configs.configs_init import get_configs
 import datetime as dt
 
-# Generate random time series data for training and evaluation (sequence-to-sequence)
-num_samples                 = 1000
-past_observation_window     = 25      
-future_prediction_window    = 10      
-num_features_known_past     = 5
-num_features_known_future   = 3
-num_features_unknown_future = 2
-
-# Known_past = Known past system dynamics + Known past control inputs to the system
-# Known_future = Control inputs to the system in future
-# Unknown_future = System dynamics of system in future with known future control inputs
-x_known_past      = np.random.random((num_samples, past_observation_window, num_features_known_past))
-x_known_future    = np.random.random((num_samples, future_prediction_window, num_features_known_future))
-x_unknown_future  = np.random.random((num_samples, output_sequence_length, num_features_unknown_future))
-
-# Split the data into training and testing sets using a basic Python function
-train_test_split_percentage                     = 0.8
-split_index                                     = int(train_test_split_percentage * num_samples)
-x_train_known_past, x_test_known_past           = x_known_past[:split_index], x_known_past[split_index:]
-x_train_known_future, x_test_known_future       = x_known_future[:split_index], x_known_future[split_index:]
-y_train_unknown_future, y_test_unknown_future   = x_unknown_future[:split_index], x_unknown_future[split_index:]
-
-# Load the configurations for the model
-configs = get_configs('config_model.yaml')
-
-# 'ident' is a string used to ensure unique file and prediction case names
-ident = 'test_'
-ident = ident + str(dt.datetime.now().strftime('%H.%M.%S'))
-
-# Initialize and build the model using your library
-model_class = Model_Gen(configs, ident)
-model_class.build_model()
-model = model_class.model
-
-# Note: Model compilation happens inside Model_Gen.build_model() and is dependent on the user's choice.
-# For point-based forecasts, users can decide not to compile the model inside build_model() to have more
-# control over the available compile options (e.g., loss function, metrics, and learning rate schedulers).
-# For probabilistic forecasts, model.compile() occurs inside build_model() since custom loss functions are used.
-
-# Train the model
-history = model.fit(
-    [x_train_known_past, x_train_known_future],
-    y_train_unknown_future,
-    batch_size=32,          # for example
-    epochs=10,              # for example
-    validation_split=0.2    # for example
-)
-
-# Evaluate the model
-test_loss, test_accuracy = model.evaluate([x_test_known_past, x_test_known_future], y_test_unknown_future)
-print(f'Test loss: {test_loss}, Test accuracy: {test_accuracy}')
+class MultiprocessingWindow():
+    """
+     Wrapper class to spawn a multiprocessing window for training and testing 
+     to avoid the issue of 'Tensorflow not releasing GPU memory'
+    """
+    def __init__(self, function_to_run, its_args):
+        self.function_to_run = function_to_run
+        self.its_args = its_args
+
+    def __call__(self):
+        multiprocessing.set_start_method('spawn', force=True)
+        print("Multiprocessing window spawned")
+        p = multiprocessing.Process(target=self.function_to_run, args=self.its_args)
+        p.start()
+        p.join()
+
+def train_test(MODEL_CONFIG_FILENAME):
+    # Load the configurations for the model
+    configs = get_configs(MODEL_CONFIG_FILENAME)
+    configs['if_model_image'] = 0
+    configs['n_past'] = 25 #Number of past observations timesteps to be considered for prediction
+    configs['n_future'] = 10 #Number of future predictions timesteps to be made
+    configs['known_past_features'] = 2 #Number of features in the past observation window data
+    configs['known_future_features'] = 3 #Number of features in the future prediction window data
+    configs['unknown_future_features'] = 2 #Number of features in the future prediction window data to be predicted
+    
+    # Generate random time series data for training and evaluation (sequence-to-sequence)
+    num_samples = 1000
+    x_known_past = np.random.random((num_samples, configs['n_past'], configs['known_past_features']))
+    x_known_future = np.random.random((num_samples, configs['n_future'], configs['known_future_features']))
+    y_unknown_future = np.random.random((num_samples, configs['n_future'], configs['unknown_future_features']))
+
+    # Split the data into training and testing sets using a basic Python function
+    train_test_split_percentage = 0.8
+    split_index = int(train_test_split_percentage * num_samples)
+    x_train_known_past, x_test_known_past = x_known_past[:split_index], x_known_past[split_index:]
+    x_train_known_future, x_test_known_future = x_known_future[:split_index], x_known_future[split_index:]
+    y_train_unknown_future, y_test_unknown_future = y_unknown_future[:split_index], y_unknown_future[split_index:]
+
+    # 'ident' is a string used to ensure unique file and prediction case names
+    ident = 'test_'
+    current_run_dt = ident + str(dt.datetime.now().strftime('%d.%m-%H.%M.%S'))
+
+    # Initialize and build the model using your library
+    model_class = Model_Gen(configs, ident)
+    model_class.build_model()
+
+    # Note: Model compilation happens inside Model_Gen.build_model() and is dependent on the user's choice.
+    # Note: User can also compile model again using different optimizer and loss function
+
+    # Train the model
+    model_class.model.fit([x_train_known_past, x_train_known_future], 
+                            y_train_unknown_future, 
+                            batch_size=128, 
+                            epochs=3, 
+                            validation_split=0.2)
+
+    # Evaluate the model
+    test_loss, test_accuracy = model_class.model.evaluate([x_test_known_past, x_test_known_future], y_test_unknown_future)
+    print(f'Test loss: {test_loss}, Test accuracy: {test_accuracy}')
+
+    # Save the model with a unique filename based on ‘current_run_dt'. 
+    # Can use both keras.model.save_weights() or keras.model.save()
+    model_class.model.save(f'{current_run_dt}_random_time_series_model.h5')
 
-# Save the model with a unique filename based on 'current_run_dt'
-model.save(f'{current_run_dt}_random_time_series_model.h5')
+if __name__ == '__main__':
+    MultiprocessingWindow(train_test, (['default_config.yaml']))()
 ```
 
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture2.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture3.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture4.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture5.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture6.jpg)
-
 
 ## License
 
 MIT License
 
 **Free Software, Hell Yeah!**
 
-   [pymodconn\configs\default_config.yaml]: <https://github.com/gaurav306/pymodconn/blob/master/pymodconn/configs/default_config.yaml>
+   [pymodconn\configs\default_config.yaml]: <https://github.com/gaurav306/pymodconn/blob/master/pymodconn/configs/default_config.yaml>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodconn-1.0.0/pymodconn/Decoder_class_layer.py` & `pymodconn-1.0.1/pymodconn/Decoder_class_layer.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/Encoder_class_layer.py` & `pymodconn-1.0.1/pymodconn/Encoder_class_layer.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/MHA_block_class_function.py` & `pymodconn-1.0.1/pymodconn/MHA_block_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/RNN_block_class_function.py` & `pymodconn-1.0.1/pymodconn/RNN_block_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/TCN_addnorm_class_function.py` & `pymodconn-1.0.1/pymodconn/TCN_addnorm_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/cit_block.py` & `pymodconn-1.0.1/pymodconn/cit_block.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/configs/configs_init.py` & `pymodconn-1.0.1/pymodconn/configs/configs_init.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/keras_tcn.py` & `pymodconn-1.0.1/pymodconn/keras_tcn.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/model_gen.py` & `pymodconn-1.0.1/pymodconn/model_gen.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/model_gen_utils.py` & `pymodconn-1.0.1/pymodconn/model_gen_utils.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn/utils_layers.py` & `pymodconn-1.0.1/pymodconn/utils_layers.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/pymodconn.egg-info/PKG-INFO` & `pymodconn-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,121 @@
 Metadata-Version: 2.1
 Name: pymodconn
-Version: 1.0.0
-Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
+Version: 1.0.1
+Summary: Develops sequence to sequence control-oriented deep neural networks in a highly modular way.
 Home-page: https://github.com/gaurav306/pymodconn
 Author: Gaurav Chaudhary
 Author-email: gaurav.chaudhary@ntnu.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pymodconn
+# _pymodconn_ : A Python package for developing modular sequence to sequence control-oriented deep neural networks
+*To prevent plagarism, more details will be added here after the paper is published.*
 
-## _pymodconn_ : A Python package for developing modular sequence to sequence control oriented neural networks
+![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/FIG1.png)
 
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture1.jpg)
+A control-oriented deep neural network (CONN) is a deep neural network designed to predict the future behaviour and response of complex dynamic systems, taking into account *Known past data* and *Known future data*. 
+- *Known past data* includes historical information such as weather data, time information, system dynamics, and control inputs, which are used to train the CONN to understand the relationships between these variables and their effects on the system. 
+- *Known future data* encompasses forecasted weather data, time information, schedules, and most importantly targeted control inputs, representing the expected conditions and desired actions that the system will be subject to in the future. 
 
-A Control-Oriented Neural Network (CONN) is an artificial neural network designed to predict the future behavior and response of highly complex dynamic systems, taking into account past known data and future known data.
-
-1. Past known data includes historical information such as weather data, system dynamics, and control inputs, which is used to train the neural network to understand the relationships between these variables and their effects on the system.
-2. Future known data encompasses forecasted weather data and targeted control inputs, representing the expected conditions and desired actions that the system will be subject to in the future.
-
-The neural network leverages this information to predict future unknown data, referring to the system dynamics or states that are not yet known. This prediction enables the control system to anticipate changes in the environment and adapt its actions accordingly, ensuring optimal performance and robustness in the face of uncertainties.
-
-CONN is particularly useful in applications where systems are affected by external factors (such as weather) and require precise control over their dynamics, such as energy management systems, water resource management, and other infrastructure systems that must be optimized to ensure reliability and efficiency.
+The CONN leverages this information to predict future, i.e., *Unknown future data*, referring to the system dynamics or states that are not yet known. This prediction enables the control system to anticipate changes in the environment and adapt its actions, accordingly, ensuring optimal performance and robustness in spite of uncertainties.
 
 ## Instructions
 
 ### 1. Install:
 ```
 pip install pymodconn
 ```
 ### 2. Usage:
 Download congifuration file from [pymodconn\configs\default_config.yaml]
 
 ```python
+import multiprocessing
 import numpy as np
-from pymodconn.configs_init import get_configs
+import sys
 from pymodconn import Model_Gen
+from pymodconn.configs.configs_init import get_configs
 import datetime as dt
 
-# Generate random time series data for training and evaluation (sequence-to-sequence)
-num_samples                 = 1000
-past_observation_window     = 25      
-future_prediction_window    = 10      
-num_features_known_past     = 5
-num_features_known_future   = 3
-num_features_unknown_future = 2
-
-# Known_past = Known past system dynamics + Known past control inputs to the system
-# Known_future = Control inputs to the system in future
-# Unknown_future = System dynamics of system in future with known future control inputs
-x_known_past      = np.random.random((num_samples, past_observation_window, num_features_known_past))
-x_known_future    = np.random.random((num_samples, future_prediction_window, num_features_known_future))
-x_unknown_future  = np.random.random((num_samples, output_sequence_length, num_features_unknown_future))
-
-# Split the data into training and testing sets using a basic Python function
-train_test_split_percentage                     = 0.8
-split_index                                     = int(train_test_split_percentage * num_samples)
-x_train_known_past, x_test_known_past           = x_known_past[:split_index], x_known_past[split_index:]
-x_train_known_future, x_test_known_future       = x_known_future[:split_index], x_known_future[split_index:]
-y_train_unknown_future, y_test_unknown_future   = x_unknown_future[:split_index], x_unknown_future[split_index:]
-
-# Load the configurations for the model
-configs = get_configs('config_model.yaml')
-
-# 'ident' is a string used to ensure unique file and prediction case names
-ident = 'test_'
-ident = ident + str(dt.datetime.now().strftime('%H.%M.%S'))
-
-# Initialize and build the model using your library
-model_class = Model_Gen(configs, ident)
-model_class.build_model()
-model = model_class.model
-
-# Note: Model compilation happens inside Model_Gen.build_model() and is dependent on the user's choice.
-# For point-based forecasts, users can decide not to compile the model inside build_model() to have more
-# control over the available compile options (e.g., loss function, metrics, and learning rate schedulers).
-# For probabilistic forecasts, model.compile() occurs inside build_model() since custom loss functions are used.
-
-# Train the model
-history = model.fit(
-    [x_train_known_past, x_train_known_future],
-    y_train_unknown_future,
-    batch_size=32,          # for example
-    epochs=10,              # for example
-    validation_split=0.2    # for example
-)
-
-# Evaluate the model
-test_loss, test_accuracy = model.evaluate([x_test_known_past, x_test_known_future], y_test_unknown_future)
-print(f'Test loss: {test_loss}, Test accuracy: {test_accuracy}')
+class MultiprocessingWindow():
+    """
+     Wrapper class to spawn a multiprocessing window for training and testing 
+     to avoid the issue of 'Tensorflow not releasing GPU memory'
+    """
+    def __init__(self, function_to_run, its_args):
+        self.function_to_run = function_to_run
+        self.its_args = its_args
+
+    def __call__(self):
+        multiprocessing.set_start_method('spawn', force=True)
+        print("Multiprocessing window spawned")
+        p = multiprocessing.Process(target=self.function_to_run, args=self.its_args)
+        p.start()
+        p.join()
+
+def train_test(MODEL_CONFIG_FILENAME):
+    # Load the configurations for the model
+    configs = get_configs(MODEL_CONFIG_FILENAME)
+    configs['if_model_image'] = 0
+    configs['n_past'] = 25 #Number of past observations timesteps to be considered for prediction
+    configs['n_future'] = 10 #Number of future predictions timesteps to be made
+    configs['known_past_features'] = 2 #Number of features in the past observation window data
+    configs['known_future_features'] = 3 #Number of features in the future prediction window data
+    configs['unknown_future_features'] = 2 #Number of features in the future prediction window data to be predicted
+    
+    # Generate random time series data for training and evaluation (sequence-to-sequence)
+    num_samples = 1000
+    x_known_past = np.random.random((num_samples, configs['n_past'], configs['known_past_features']))
+    x_known_future = np.random.random((num_samples, configs['n_future'], configs['known_future_features']))
+    y_unknown_future = np.random.random((num_samples, configs['n_future'], configs['unknown_future_features']))
+
+    # Split the data into training and testing sets using a basic Python function
+    train_test_split_percentage = 0.8
+    split_index = int(train_test_split_percentage * num_samples)
+    x_train_known_past, x_test_known_past = x_known_past[:split_index], x_known_past[split_index:]
+    x_train_known_future, x_test_known_future = x_known_future[:split_index], x_known_future[split_index:]
+    y_train_unknown_future, y_test_unknown_future = y_unknown_future[:split_index], y_unknown_future[split_index:]
+
+    # 'ident' is a string used to ensure unique file and prediction case names
+    ident = 'test_'
+    current_run_dt = ident + str(dt.datetime.now().strftime('%d.%m-%H.%M.%S'))
+
+    # Initialize and build the model using your library
+    model_class = Model_Gen(configs, ident)
+    model_class.build_model()
+
+    # Note: Model compilation happens inside Model_Gen.build_model() and is dependent on the user's choice.
+    # Note: User can also compile model again using different optimizer and loss function
+
+    # Train the model
+    model_class.model.fit([x_train_known_past, x_train_known_future], 
+                            y_train_unknown_future, 
+                            batch_size=128, 
+                            epochs=3, 
+                            validation_split=0.2)
+
+    # Evaluate the model
+    test_loss, test_accuracy = model_class.model.evaluate([x_test_known_past, x_test_known_future], y_test_unknown_future)
+    print(f'Test loss: {test_loss}, Test accuracy: {test_accuracy}')
+
+    # Save the model with a unique filename based on ‘current_run_dt'. 
+    # Can use both keras.model.save_weights() or keras.model.save()
+    model_class.model.save(f'{current_run_dt}_random_time_series_model.h5')
 
-# Save the model with a unique filename based on 'current_run_dt'
-model.save(f'{current_run_dt}_random_time_series_model.h5')
+if __name__ == '__main__':
+    MultiprocessingWindow(train_test, (['default_config.yaml']))()
 ```
 
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture2.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture3.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture4.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture5.jpg)
-![alt text](https://github.com/gaurav306/pymodconn/blob/master/Readme_images/Picture6.jpg)
-
 
 ## License
 
 MIT License
 
 **Free Software, Hell Yeah!**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodconn-1.0.0/pymodconn.egg-info/SOURCES.txt` & `pymodconn-1.0.1/pymodconn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.0/setup.cfg` & `pymodconn-1.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pymodconn
-version = 1.0.0
+version = 1.0.1
 author = Gaurav Chaudhary
 author_email = gaurav.chaudhary@ntnu.no
-description = Develops sequence to sequence control oriented neural networks in a highly modular way.
+description = Develops sequence to sequence control-oriented deep neural networks in a highly modular way.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gaurav306/pymodconn
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

