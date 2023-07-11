# Comparing `tmp/pymodconn-0.0.4.tar.gz` & `tmp/pymodconn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodconn-0.0.4.tar", last modified: Tue Apr 25 15:13:13 2023, max compression
+gzip compressed data, was "pymodconn-1.0.0.tar", last modified: Tue Jul 11 10:33:17 2023, max compression
```

## Comparing `pymodconn-0.0.4.tar` & `pymodconn-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 15:12:59.000000 pymodconn-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-25 15:13:13.167431 pymodconn-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-25 15:12:59.000000 pymodconn-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/pymodconn/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/configs_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/major_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/model_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/model_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/utils_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/pymodconn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 15:13:13.167431 pymodconn-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 15:12:59.000000 pymodconn-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 10:33:06.000000 pymodconn-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-11 10:33:17.463890 pymodconn-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-11 10:33:06.000000 pymodconn-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.459890 pymodconn-1.0.0/pymodconn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/Decoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/Encoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/MHA_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/RNN_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/TCN_addnorm_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/cit_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/pymodconn/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/configs/configs_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/keras_tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/model_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/model_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pymodconn/utils_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:17.463890 pymodconn-1.0.0/pymodconn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 10:33:17.000000 pymodconn-1.0.0/pymodconn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 10:33:07.000000 pymodconn-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 10:33:17.463890 pymodconn-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 10:33:07.000000 pymodconn-1.0.0/setup.py
```

### Comparing `pymodconn-0.0.4/LICENSE` & `pymodconn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodconn-0.0.4/pymodconn/model_gen.py` & `pymodconn-1.0.0/pymodconn/model_gen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,129 @@
 import pymodconn.model_gen_utils as Model_utils
-from pymodconn.major_layers import Encoder_class
-from pymodconn.major_layers import Decoder_class
+from pymodconn.Encoder_class_layer import Encoder_class
+from pymodconn.Decoder_class_layer import Decoder_class
 from pymodconn.utils_layers import *
 import numpy as np
 import tensorflow as tf
-from tensorflow.keras import backend as K
-from tensorflow.keras.models import Model
+from tensorflow import keras
+import keras.backend as K
+from keras.models import Model
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '1'
 
 
-class ModelClass():
+class Model_Gen():
     def __init__(self, cfg, current_dt):
         self.cfg = cfg
         self.current_dt = current_dt
 
         if cfg['if_seed']:
             np.random.seed(cfg['seed'])
             tf.random.set_seed(cfg['seed'])
-        self.epochs = cfg['epochs']
-        self.batch_size = cfg['batch_size']
-        self.save_models_dir = cfg['save_models_dir']
-        self.save_results_dir = cfg['save_results_dir']
-        self.future_data_col = cfg['future_data_col']
+            tf.keras.utils.set_random_seed(cfg['seed'])
+            tf.config.experimental.enable_op_determinism()
+        
         self.n_past = cfg['n_past']
-        self.n_features_input = cfg['n_features_input']
+        self.n_future = cfg['n_future']
+        self.known_past_features = cfg['known_past_features']
+        self.unknown_future_features = cfg['unknown_future_features']
+        self.known_future_features = cfg['known_future_features']
+
         self.all_layers_neurons = cfg['all_layers_neurons']
-        self.input_enc_rnn_depth = cfg['input_enc_rnn_depth']
         self.all_layers_dropout = cfg['all_layers_dropout']
-        self.n_future = cfg['n_future']
-        self.n_features_output = cfg['n_features_output']
-        self.optimizer = cfg['optimizer']  # new
-        self.SGD_lr = cfg['SGD']['lr']  # new
-        self.SGD_mom = cfg['SGD']['momentum']  # new
-        self.Adam_lr = cfg['Adam']['lr']
-        self.Adam_b1 = cfg['Adam']['b1']
-        self.Adam_b2 = cfg['Adam']['b2']
-        self.Adam_epsi = cfg['Adam']['epsi']
-        self.loss_func = cfg['loss']
+        
         self.model_type_prob = cfg['model_type_prob']
         self.loss_prob = cfg['loss_prob']
         self.q = cfg['quantiles']
-        self.control_future_cells = cfg['control_future_cells']
-
-        self.n_features_output_block = 1
-
-        self.n_outputs_lastlayer = 2 if self.loss_prob == 'parametric' else len(
-            self.q)
-
-        self.metrics = cfg['metrics']
-        self.mha_head = cfg['mha_head']
-
-        self.cfg = cfg
-        self.rnn_type = cfg['rnn_type']
-        self.dec_attn_mask = cfg['dec_attn_mask']
-
-        self.fit_type = cfg['fit_type']
-        self.seq_len = cfg['seq_len']
-        self.if_save_model_image = cfg['if_model_image']
-        self.if_model_summary = cfg['if_model_summary']
-
-        self.model_size_GB = 0
-
-        # model structure
-        self.IFRNN1 = cfg['IFRNN_input']
-        self.IFRNN2 = cfg['IFRNN_output']
-        self.IFSELF_MHA = cfg['IFSELF_MHA']
-        self.IFCASUAL_MHA = cfg['IFCASUAL_MHA']
-        self.IFCROSS_MHA = cfg['IFCROSS_MHA']
-
-        self.save_training_history_file = os.path.join(
-            self.save_results_dir, '%s.csv' % (self.current_dt))
-        self.save_training_history = os.path.join(
-            self.save_results_dir, '%s_history.png' % (self.current_dt))
-        self.save_hf5_name = os.path.join(
-            self.save_models_dir, '%s.h5' % (self.current_dt))
-        self.save_modelimage_name = os.path.join(
-            self.save_models_dir, '%s_modelimage.png' % (self.current_dt))
-        self.save_modelsummary_name = os.path.join(
-            self.save_models_dir, '%s_modelsummary.txt' % (self.current_dt))
+        self.n_outputs_lastlayer = 2 if self.loss_prob == 'parametric' else len(self.q)
 
+        self.save_models_dir = cfg['save_models_dir']
         if not os.path.exists(cfg['save_models_dir']):
             os.makedirs(cfg['save_models_dir'])
 
     def build_model(self):
         """
-        Full transformer biLSTM 1 single = input > MHA > biLSTM > output
-        here Input goes to MHA and then to biLSTM
+        The build_model() method is responsible for constructing the architecture of your deep learning model according to the 
+        specifications outlined in the provided configuration file. The model is built using the Keras API of TensorFlow, 
+        which allows for the flexible construction of a variety of neural network models.
+
+        This method first creates an input layer for the encoder, encoder_inputs, and passes this to an instance of Encoder_class. 
+        The encoder processes the input data and returns two outputs: encoder_outputs_seq and encoder_outputs_allstates. 
+        These outputs represent the sequence of hidden states and the final state of the encoder, respectively.
+
+        Next, the method enters a loop where it creates a number of decoders based on the control_future_cells parameter, 
+        which can range from 1 to 6. For each iteration, it creates a new input layer decoder_{i}_inputs and passes it, 
+        along with the encoder outputs, to an instance of Decoder_class. The output of each decoder is added to decoder_outputs_list.
+
+        After all decoders have been processed, the method concatenates their outputs using a custom MERGE_LIST layer.
+
+        The method then determines whether the model uses a probabilistic or non-probabilistic forecast approach based 
+        on the model_type_prob parameter. Depending on the approach, it applies different operations to the concatenated 
+        decoder outputs to produce the final model output, decoder_outputs4.
+
+        Finally, it creates a Keras Model instance with the encoder inputs and decoder inputs as inputs and decoder_outputs4 
+        as the output. The Build_utils method is called to post-process the model, where it selects the appropriate 
+        loss function, optimizer, and metrics based on the user input from the configuration file.
         """
         timer = Model_utils.Timer()
         timer.start()
-        print('[ModelClass] Model Compiling.....')
-        self.future_data_col = self.future_data_col - self.control_future_cells + 1
+        print('[pymodconn] Model Compiling.....')
 
         # input for encoder_past
         encoder_inputs = tf.keras.layers.Input(
-            shape=(self.n_past, self.n_features_input), name='encoder_past_inputs')
+            shape=(self.n_past, self.known_past_features), name='encoder_past_inputs')
         
         encoder_outputs_seq, encoder_outputs_allstates = Encoder_class(
             self.cfg, str(1))(encoder_inputs, init_states=None)
 
+        '''
         decoder_outputs_list = []
         
         for i in range(1, self.control_future_cells+1):
-            locals()[f"decoder_{i}_inputs"] = tf.keras.layers.Input(shape=(self.n_future, self.future_data_col), name=f"decoder_{i}_inputs")
-            
+            locals()[f"decoder_{i}_inputs"] = tf.keras.layers.Input(shape=(self.n_future, self.known_future_features), name=f"decoder_{i}_inputs")
             locals()[f"decoder_{i}_outputs"] = Decoder_class(self.cfg, str(i))(locals()[f"decoder_{i}_inputs"],
                                                                                 encoder_outputs_seq,
                                                                                 encoder_states=encoder_outputs_allstates)
             decoder_outputs_list.append(locals()[f"decoder_{i}_outputs"])
         
-        decoder_outputs_all = MERGE_LIST(self.n_features_output)(decoder_outputs_list)
+        decoder_outputs_all = MERGE_LIST(self.unknown_future_features)(decoder_outputs_list)
+        '''
+        decoder_inputs = tf.keras.layers.Input(
+            shape=(self.n_future, self.known_future_features), name=f"decoder_inputs")
+
+        decoder_outputs = Decoder_class(self.cfg, '1')(decoder_inputs,
+                                                        encoder_outputs_seq,
+                                                        encoder_states=encoder_outputs_allstates)        
 
-        # print('Probabilistic or non probabilistic changes')
         # If or not using the probabilistic loss, reshape the output to match the shape required by the loss function.
         if self.model_type_prob == 'prob':
             decoder_outputs3 = tf.keras.layers.Dense(
-                units=self.n_features_output * self.n_outputs_lastlayer)(decoder_outputs_all)  # this one
+                units=self.unknown_future_features * self.n_outputs_lastlayer)(decoder_outputs)  # this one
             # Reshape the encoder output to match the shape required by the loss function.
             decoder_outputs4 = tf.keras.layers.Reshape(target_shape=(
-                self.n_future, self.n_features_output, self.n_outputs_lastlayer))(decoder_outputs3)
+                self.n_future, self.unknown_future_features, self.n_outputs_lastlayer))(decoder_outputs3)
             # If using the parametric loss, apply the soft ReLU activation to ensure a positive standard deviation.
             if self.loss_prob == 'parametric':
                 decoder_outputs4 = tf.keras.layers.Lambda(function=lambda x: tf.stack(
                     [x[:, :, :, 0], soft_relu(x[:, :, :, 1])], axis=-1))(decoder_outputs4)
         elif self.model_type_prob == 'nonprob':
             decoder_outputs4 = tf.keras.layers.Lambda(
-                lambda x: tf.clip_by_value(x, -1, 1))(decoder_outputs_all)
+                lambda x: tf.clip_by_value(x, -1, 1))(decoder_outputs)
         else:
             raise ValueError(
                 'model_type_prob should be either prob or nonprob')
 
-        decoder_inputs = []
-        for i in range(1, self.control_future_cells+1):
-            decoder_inputs.append(locals()[f"decoder_{i}_inputs"])
-
         self.model = Model(
             [encoder_inputs, decoder_inputs], decoder_outputs4)
 
         Model_utils.Build_utils(
             self.cfg, self.current_dt).postbuild_model(self.model)
 
     def load_model(self, filepath):
-        print('[ModelClass_tfp] Loading model from file %s' % filepath)
+        print('[pymodconn_tfp] Loading model from file %s' % filepath)
         # self.model = load_model(filepath)
         self.model.load_weights(filepath)
         # https://stackoverflow.com/a/69663259/6510598
 
     def forget_model(self):
         del self.model
         K.clear_session()
```

### Comparing `pymodconn-0.0.4/pymodconn/model_gen_utils.py` & `pymodconn-1.0.0/pymodconn/model_gen_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from keras.utils.layer_utils import count_params
+from pymodconn.configs.configs_init import read_write_yaml
 import os
 from typing import *
 
 import numpy as np
 import tensorflow as tf
 from keras.utils.vis_utils import plot_model
 import datetime as dt
@@ -26,79 +27,50 @@
 
 class Build_utils():
     """
     This class is used to compile, make sumamry and save as png.
     """
 
     def __init__(self, cfg, current_dt):
-        if cfg['if_seed']:
-            np.random.seed(cfg['seed'])
-            tf.random.set_seed(cfg['seed'])
-        self.epochs = cfg['epochs']
+        self.cfg = cfg
+        self.current_dt = current_dt
         self.batch_size = cfg['batch_size']
-        self.future_data_col = cfg['future_data_col']
-        self.n_past = cfg['n_past']
-        self.n_features_input = cfg['n_features_input']
-        self.all_layers_neurons = cfg['all_layers_neurons']
-        self.all_layers_dropout = cfg['all_layers_dropout']
-        self.n_future = cfg['n_future']
-        self.n_features_output = cfg['n_features_output']
         self.optimizer = cfg['optimizer']  # new
         self.SGD_lr = cfg['SGD']['lr']  # new
         self.SGD_mom = cfg['SGD']['momentum']  # new
         self.Adam_lr = cfg['Adam']['lr']
         self.Adam_b1 = cfg['Adam']['b1']
         self.Adam_b2 = cfg['Adam']['b2']
         self.Adam_epsi = cfg['Adam']['epsi']
         self.loss_func = cfg['loss']
         self.model_type_prob = cfg['model_type_prob']
         self.loss_prob = cfg['loss_prob']
         self.q = cfg['quantiles']
-        self.control_future_cells = cfg['control_future_cells']
 
         self.n_features_output_block = 1
 
         self.q = np.unique(np.array(self.q))
         if 0.5 not in self.q:
             self.q = np.sort(np.append(0.5, self.q))
         self.n_outputs_lastlayer = 2 if self.loss_prob == 'parametric' else len(
             self.q)
 
         self.metrics = cfg['metrics']
-        self.mha_head = cfg['mha_head']
-
-        self.cfg = cfg
-        self.rnn_type = cfg['rnn_type']
-        self.dec_attn_mask = cfg['dec_attn_mask']
 
-        self.model_type = cfg['model_type']
-        self.fit_type = cfg['fit_type']
-        self.seq_len = cfg['seq_len']
         self.if_save_model_image = cfg['if_model_image']
         self.if_model_summary = cfg['if_model_summary']
 
-        # model structure
-        self.IFRNN1 = cfg['IFRNN_input']
-        self.IFRNN2 = cfg['IFRNN_output']
-        self.IFSELF_MHA = cfg['IFSELF_MHA']
-        self.IFCASUAL_MHA = cfg['IFCASUAL_MHA']
-        self.IFCROSS_MHA = cfg['IFCROSS_MHA']
-
         self.save_models_dir = cfg['save_models_dir']
-        self.save_results_dir = cfg['save_results_dir']
-        self.save_training_history_file = os.path.join(
-            self.save_results_dir, '%s.csv' % (current_dt))
-        self.save_training_history = os.path.join(
-            self.save_results_dir, '%s_history.png' % (current_dt))
-        self.save_hf5_name = os.path.join(
-            self.save_models_dir, '%s.h5' % (current_dt))
         self.save_modelimage_name = os.path.join(
-            self.save_models_dir, '%s_modelimage.png' % (current_dt))
+            self.save_models_dir, '%s_modelimage.png' % (self.current_dt))
         self.save_modelsummary_name = os.path.join(
-            self.save_models_dir, '%s_modelsummary.txt' % (current_dt))
+            self.save_models_dir, '%s_modelsummary.txt' % (self.current_dt))
+        self.save_modelconfig = os.path.join(
+            self.save_models_dir, '%s_modelconfig.yaml' % (self.current_dt))
+        
 
     def CVRMSE_Q50_prob_nonparametric(self, y_true, y_pred):
         return K.sqrt(K.mean(K.square(y_pred[:, :, :, 3] - y_true)))/(K.mean(y_true))
 
     def CVRMSE_Q50_prob_parametric(self, y_true, y_pred):
         return K.sqrt(K.mean(K.square(y_pred[:, :, :, 0] - y_true)))/(K.mean(y_true))
 
@@ -143,33 +115,35 @@
                                metrics=self.metrics,
                                run_eagerly=True)
 
         if self.if_model_summary:
             self.model.summary()
 
         self.trainable_count = count_params(model.trainable_weights)
-        '''
         self.GET_MODEL_SIZE_GB = get_model_memory_usage(
             self.batch_size, self.model)
         print('Trainable parameters in the model : %d' % self.trainable_count)
-        '''
+        
         with open(self.save_modelsummary_name, 'w') as f:
             self.model.summary(print_fn=lambda x: f.write(x + '\n'), 
                                line_length = 250, 
                                expand_nested=True,
                                show_trainable=True)
-        '''
+
         with open(self.save_modelsummary_name, 'a') as f:
             f.write('_' * 25 + '\n')
             f.write('Model size in GB : %f' % self.GET_MODEL_SIZE_GB)
-        '''
+        
         if self.if_save_model_image:
             print('Saving model as %s' % self.save_modelimage_name)
             plot_model(self.model, to_file=self.save_modelimage_name,
                        show_shapes=True, show_layer_names=True, dpi=600, expand_nested=True)
+        
+        read_write_yaml(self.save_modelconfig, 'w', self.cfg)
+
         print("[ModelClass] Building postmodel DONE!! model can be used as self.model")
 
 
 def get_model_memory_usage(batch_size, model):
     shapes_mem_count = 0
     internal_model_mem_count = 0
     for l in model.layers:
@@ -179,15 +153,15 @@
         single_layer_mem = 1
         out_shape = l.output_shape
         if type(out_shape) is list:
             out_shape = out_shape[0]
         for s in out_shape:
             if s is None:
                 continue
-            single_layer_mem *= s
+            single_layer_mem  = single_layer_mem * s
         shapes_mem_count += single_layer_mem
 
     trainable_count = np.sum([K.count_params(p)
                              for p in model.trainable_weights])
     non_trainable_count = np.sum([K.count_params(p)
                                  for p in model.non_trainable_weights])
```

### Comparing `pymodconn-0.0.4/setup.cfg` & `pymodconn-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymodconn
-version = 0.0.4
+version = 1.0.0
 author = Gaurav Chaudhary
 author_email = gaurav.chaudhary@ntnu.no
 description = Develops sequence to sequence control oriented neural networks in a highly modular way.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gaurav306/pymodconn
 classifiers =
```

