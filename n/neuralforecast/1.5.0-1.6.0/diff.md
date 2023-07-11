# Comparing `tmp/neuralforecast-1.5.0.tar.gz` & `tmp/neuralforecast-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralforecast-1.5.0.tar", last modified: Sat Apr 22 19:28:50 2023, max compression
+gzip compressed data, was "neuralforecast-1.6.0.tar", last modified: Tue Jul 11 17:46:23 2023, max compression
```

## Comparing `neuralforecast-1.5.0.tar` & `neuralforecast-1.6.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.662371 neuralforecast-1.5.0/neuralforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   111564 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    24293 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    26826 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_scalers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    70389 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/neuralforecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25546 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/autoformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/dilated_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nbeatsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)    35403 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/patchtst.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/stemgnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    28684 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/tft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/vanillatransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/tsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.617325 neuralforecast-1.6.0/neuralforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127213 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.621325 neuralforecast-1.6.0/neuralforecast/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26007 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29923 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27205 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.621325 neuralforecast-1.6.0/neuralforecast/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83647 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/neuralforecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26097 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/dilated_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/fedformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nbeatsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35871 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/patchtst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/stemgnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/tft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/vanillatransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/tsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.617325 neuralforecast-1.6.0/neuralforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/setup.py
```

### Comparing `neuralforecast-1.5.0/LICENSE` & `neuralforecast-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/PKG-INFO` & `neuralforecast-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.5.0
+Version: 1.6.0
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neuralforecast-1.5.0/README.md` & `neuralforecast-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/_modidx.py` & `neuralforecast-1.6.0/neuralforecast/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,23 @@
                 'lib_path': 'neuralforecast'},
   'syms': { 'neuralforecast.auto': { 'neuralforecast.auto.AutoAutoformer': ('models.html#autoautoformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoAutoformer.__init__': ( 'models.html#autoautoformer.__init__',
                                                                                       'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN': ('models.html#autodilatedrnn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN.__init__': ( 'models.html#autodilatedrnn.__init__',
                                                                                       'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoFEDformer': ('models.html#autofedformer', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoFEDformer.__init__': ( 'models.html#autofedformer.__init__',
+                                                                                     'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoGRU': ('models.html#autogru', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoGRU.__init__': ('models.html#autogru.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoHINT': ('models.html#autohint', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoHINT.__init__': ('models.html#autohint.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoHINT._fit_model': ( 'models.html#autohint._fit_model',
+                                                                                  'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoInformer': ('models.html#autoinformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoInformer.__init__': ( 'models.html#autoinformer.__init__',
                                                                                     'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoLSTM': ('models.html#autolstm', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoLSTM.__init__': ('models.html#autolstm.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP': ('models.html#automlp', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP.__init__': ('models.html#automlp.__init__', 'neuralforecast/auto.py'),
@@ -53,16 +60,14 @@
                                                                                               'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.fit': ('core.html#neuralforecast.fit', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.load': ('core.html#neuralforecast.load', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.predict': ( 'core.html#neuralforecast.predict',
                                                                                      'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.predict_insample': ( 'core.html#neuralforecast.predict_insample',
                                                                                               'neuralforecast/core.py'),
-                                     'neuralforecast.core.NeuralForecast.predict_rolled': ( 'core.html#neuralforecast.predict_rolled',
-                                                                                            'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.save': ('core.html#neuralforecast.save', 'neuralforecast/core.py'),
                                      'neuralforecast.core._cv_dates': ('core.html#_cv_dates', 'neuralforecast/core.py'),
                                      'neuralforecast.core._future_dates': ('core.html#_future_dates', 'neuralforecast/core.py'),
                                      'neuralforecast.core._insample_dates': ('core.html#_insample_dates', 'neuralforecast/core.py')},
             'neuralforecast.losses.numpy': { 'neuralforecast.losses.numpy._divide_no_nan': ( 'losses.numpy.html#_divide_no_nan',
                                                                                              'neuralforecast/losses/numpy.py'),
                                              'neuralforecast.losses.numpy._metric_protections': ( 'losses.numpy.html#_metric_protections',
@@ -111,14 +116,38 @@
                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.GMM.neglog_likelihood': ( 'losses.pytorch.html#gmm.neglog_likelihood',
                                                                                                         'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.GMM.sample': ( 'losses.pytorch.html#gmm.sample',
                                                                                              'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.GMM.scale_decouple': ( 'losses.pytorch.html#gmm.scale_decouple',
                                                                                                      'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberLoss': ( 'losses.pytorch.html#huberloss',
+                                                                                            'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberLoss.__call__': ( 'losses.pytorch.html#huberloss.__call__',
+                                                                                                     'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberLoss.__init__': ( 'losses.pytorch.html#huberloss.__init__',
+                                                                                                     'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberLoss.domain_map': ( 'losses.pytorch.html#huberloss.domain_map',
+                                                                                                       'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberMQLoss': ( 'losses.pytorch.html#hubermqloss',
+                                                                                              'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberMQLoss.__call__': ( 'losses.pytorch.html#hubermqloss.__call__',
+                                                                                                       'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberMQLoss.__init__': ( 'losses.pytorch.html#hubermqloss.__init__',
+                                                                                                       'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberMQLoss.domain_map': ( 'losses.pytorch.html#hubermqloss.domain_map',
+                                                                                                         'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberQLoss': ( 'losses.pytorch.html#huberqloss',
+                                                                                             'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberQLoss.__call__': ( 'losses.pytorch.html#huberqloss.__call__',
+                                                                                                      'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberQLoss.__init__': ( 'losses.pytorch.html#huberqloss.__init__',
+                                                                                                      'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.HuberQLoss.domain_map': ( 'losses.pytorch.html#huberqloss.domain_map',
+                                                                                                        'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.MAE': ( 'losses.pytorch.html#mae',
                                                                                       'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.MAE.__call__': ( 'losses.pytorch.html#mae.__call__',
                                                                                                'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.MAE.__init__': ( 'losses.pytorch.html#mae.__init__',
                                                                                                'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.MAE.domain_map': ( 'losses.pytorch.html#mae.domain_map',
@@ -203,14 +232,24 @@
                                                                                         'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.SMAPE.__call__': ( 'losses.pytorch.html#smape.__call__',
                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.SMAPE.__init__': ( 'losses.pytorch.html#smape.__init__',
                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.SMAPE.domain_map': ( 'losses.pytorch.html#smape.domain_map',
                                                                                                    'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.TukeyLoss': ( 'losses.pytorch.html#tukeyloss',
+                                                                                            'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.TukeyLoss.__call__': ( 'losses.pytorch.html#tukeyloss.__call__',
+                                                                                                     'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.TukeyLoss.__init__': ( 'losses.pytorch.html#tukeyloss.__init__',
+                                                                                                     'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.TukeyLoss.domain_map': ( 'losses.pytorch.html#tukeyloss.domain_map',
+                                                                                                       'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.TukeyLoss.masked_mean': ( 'losses.pytorch.html#tukeyloss.masked_mean',
+                                                                                                        'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.Tweedie': ( 'losses.pytorch.html#tweedie',
                                                                                           'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.Tweedie.__init__': ( 'losses.pytorch.html#tweedie.__init__',
                                                                                                    'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.Tweedie.log_prob': ( 'losses.pytorch.html#tweedie.log_prob',
                                                                                                    'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.Tweedie.mean': ( 'losses.pytorch.html#tweedie.mean',
@@ -387,34 +426,110 @@
                                                                                                               'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.ResLSTMLayer': ( 'models.dilated_rnn.html#reslstmlayer',
                                                                                                        'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.ResLSTMLayer.__init__': ( 'models.dilated_rnn.html#reslstmlayer.__init__',
                                                                                                                 'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.ResLSTMLayer.forward': ( 'models.dilated_rnn.html#reslstmlayer.forward',
                                                                                                                'neuralforecast/models/dilated_rnn.py')},
+            'neuralforecast.models.fedformer': { 'neuralforecast.models.fedformer.AutoCorrelationLayer': ( 'models.fedformer.html#autocorrelationlayer',
+                                                                                                           'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.AutoCorrelationLayer.__init__': ( 'models.fedformer.html#autocorrelationlayer.__init__',
+                                                                                                                    'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.AutoCorrelationLayer.forward': ( 'models.fedformer.html#autocorrelationlayer.forward',
+                                                                                                                   'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Decoder': ( 'models.fedformer.html#decoder',
+                                                                                              'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Decoder.__init__': ( 'models.fedformer.html#decoder.__init__',
+                                                                                                       'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Decoder.forward': ( 'models.fedformer.html#decoder.forward',
+                                                                                                      'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.DecoderLayer': ( 'models.fedformer.html#decoderlayer',
+                                                                                                   'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.DecoderLayer.__init__': ( 'models.fedformer.html#decoderlayer.__init__',
+                                                                                                            'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.DecoderLayer.forward': ( 'models.fedformer.html#decoderlayer.forward',
+                                                                                                           'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Encoder': ( 'models.fedformer.html#encoder',
+                                                                                              'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Encoder.__init__': ( 'models.fedformer.html#encoder.__init__',
+                                                                                                       'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.Encoder.forward': ( 'models.fedformer.html#encoder.forward',
+                                                                                                      'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.EncoderLayer': ( 'models.fedformer.html#encoderlayer',
+                                                                                                   'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.EncoderLayer.__init__': ( 'models.fedformer.html#encoderlayer.__init__',
+                                                                                                            'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.EncoderLayer.forward': ( 'models.fedformer.html#encoderlayer.forward',
+                                                                                                           'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FEDformer': ( 'models.fedformer.html#fedformer',
+                                                                                                'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FEDformer.__init__': ( 'models.fedformer.html#fedformer.__init__',
+                                                                                                         'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FEDformer.forward': ( 'models.fedformer.html#fedformer.forward',
+                                                                                                        'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierBlock': ( 'models.fedformer.html#fourierblock',
+                                                                                                   'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierBlock.__init__': ( 'models.fedformer.html#fourierblock.__init__',
+                                                                                                            'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierBlock.compl_mul1d': ( 'models.fedformer.html#fourierblock.compl_mul1d',
+                                                                                                               'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierBlock.forward': ( 'models.fedformer.html#fourierblock.forward',
+                                                                                                           'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierCrossAttention': ( 'models.fedformer.html#fouriercrossattention',
+                                                                                                            'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierCrossAttention.__init__': ( 'models.fedformer.html#fouriercrossattention.__init__',
+                                                                                                                     'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierCrossAttention.compl_mul1d': ( 'models.fedformer.html#fouriercrossattention.compl_mul1d',
+                                                                                                                        'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.FourierCrossAttention.forward': ( 'models.fedformer.html#fouriercrossattention.forward',
+                                                                                                                    'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.LayerNorm': ( 'models.fedformer.html#layernorm',
+                                                                                                'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.LayerNorm.__init__': ( 'models.fedformer.html#layernorm.__init__',
+                                                                                                         'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.LayerNorm.forward': ( 'models.fedformer.html#layernorm.forward',
+                                                                                                        'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.MovingAvg': ( 'models.fedformer.html#movingavg',
+                                                                                                'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.MovingAvg.__init__': ( 'models.fedformer.html#movingavg.__init__',
+                                                                                                         'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.MovingAvg.forward': ( 'models.fedformer.html#movingavg.forward',
+                                                                                                        'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.SeriesDecomp': ( 'models.fedformer.html#seriesdecomp',
+                                                                                                   'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.SeriesDecomp.__init__': ( 'models.fedformer.html#seriesdecomp.__init__',
+                                                                                                            'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.SeriesDecomp.forward': ( 'models.fedformer.html#seriesdecomp.forward',
+                                                                                                           'neuralforecast/models/fedformer.py'),
+                                                 'neuralforecast.models.fedformer.get_frequency_modes': ( 'models.fedformer.html#get_frequency_modes',
+                                                                                                          'neuralforecast/models/fedformer.py')},
             'neuralforecast.models.gru': { 'neuralforecast.models.gru.GRU': ('models.gru.html#gru', 'neuralforecast/models/gru.py'),
                                            'neuralforecast.models.gru.GRU.__init__': ( 'models.gru.html#gru.__init__',
                                                                                        'neuralforecast/models/gru.py'),
                                            'neuralforecast.models.gru.GRU.forward': ( 'models.gru.html#gru.forward',
                                                                                       'neuralforecast/models/gru.py')},
             'neuralforecast.models.hint': { 'neuralforecast.models.hint.HINT': ('models.hint.html#hint', 'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.__init__': ( 'models.hint.html#hint.__init__',
                                                                                           'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.__repr__': ( 'models.hint.html#hint.__repr__',
                                                                                           'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.fit': ( 'models.hint.html#hint.fit',
                                                                                      'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.get_test_size': ( 'models.hint.html#hint.get_test_size',
+                                                                                               'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.predict': ( 'models.hint.html#hint.predict',
                                                                                          'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.save': ( 'models.hint.html#hint.save',
                                                                                       'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.HINT.set_test_size': ( 'models.hint.html#hint.set_test_size',
                                                                                                'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.get_bottomup_P': ( 'models.hint.html#get_bottomup_p',
                                                                                            'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.get_identity_P': ( 'models.hint.html#get_identity_p',
+                                                                                           'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.get_mintrace_ols_P': ( 'models.hint.html#get_mintrace_ols_p',
                                                                                                'neuralforecast/models/hint.py'),
                                             'neuralforecast.models.hint.get_mintrace_wls_P': ( 'models.hint.html#get_mintrace_wls_p',
                                                                                                'neuralforecast/models/hint.py')},
             'neuralforecast.models.informer': { 'neuralforecast.models.informer.ConvLayer': ( 'models.informer.html#convlayer',
                                                                                               'neuralforecast/models/informer.py'),
                                                 'neuralforecast.models.informer.ConvLayer.__init__': ( 'models.informer.html#convlayer.__init__',
@@ -688,20 +803,14 @@
                                            'neuralforecast.models.tft.StaticCovariateEncoder.forward': ( 'models.tft.html#staticcovariateencoder.forward',
                                                                                                          'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT': ('models.tft.html#tft', 'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.__init__': ( 'models.tft.html#tft.__init__',
                                                                                        'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.forward': ( 'models.tft.html#tft.forward',
                                                                                       'neuralforecast/models/tft.py'),
-                                           'neuralforecast.models.tft.TFT.predict_step': ( 'models.tft.html#tft.predict_step',
-                                                                                           'neuralforecast/models/tft.py'),
-                                           'neuralforecast.models.tft.TFT.training_step': ( 'models.tft.html#tft.training_step',
-                                                                                            'neuralforecast/models/tft.py'),
-                                           'neuralforecast.models.tft.TFT.validation_step': ( 'models.tft.html#tft.validation_step',
-                                                                                              'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding': ( 'models.tft.html#tftembedding',
                                                                                        'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding.__init__': ( 'models.tft.html#tftembedding.__init__',
                                                                                                 'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding._apply_embedding': ( 'models.tft.html#tftembedding._apply_embedding',
                                                                                                         'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding.forward': ( 'models.tft.html#tftembedding.forward',
```

### Comparing `neuralforecast-1.5.0/neuralforecast/auto.py` & `neuralforecast-1.6.0/neuralforecast/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/models.ipynb.
 
 # %% auto 0
 __all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDilatedRNN', 'AutoMLP', 'AutoNBEATS', 'AutoNBEATSx', 'AutoNHITS',
-           'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoPatchTST', 'AutoStemGNN']
+           'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST',
+           'AutoStemGNN', 'AutoHINT']
 
 # %% ../nbs/models.ipynb 2
 from os import cpu_count
 import torch
 
 from ray import tune
 from ray.tune.search.basic_variant import BasicVariantGenerator
@@ -24,17 +25,19 @@
 from .models.nbeatsx import NBEATSx
 from .models.nhits import NHITS
 
 from .models.tft import TFT
 from .models.vanillatransformer import VanillaTransformer
 from .models.informer import Informer
 from .models.autoformer import Autoformer
+from .models.fedformer import FEDformer
 from .models.patchtst import PatchTST
 
 from .models.stemgnn import StemGNN
+from .models.hint import HINT
 
 from .losses.pytorch import MAE
 
 # %% ../nbs/models.ipynb 8
 class AutoRNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
@@ -74,15 +77,18 @@
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
             config["inference_input_size"] = tune.choice(
                 [h * x for x in self.default_config["inference_input_size_multiplier"]]
             )
-            del config["input_size_multiplier"]
+            del (
+                config["input_size_multiplier"],
+                config["inference_input_size_multiplier"],
+            )
 
         super(AutoRNN, self).__init__(
             cls_model=RNN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
@@ -90,15 +96,15 @@
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
-# %% ../nbs/models.ipynb 13
+# %% ../nbs/models.ipynb 12
 class AutoLSTM(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
@@ -129,15 +135,18 @@
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
             config["inference_input_size"] = tune.choice(
                 [h * x for x in self.default_config["inference_input_size_multiplier"]]
             )
-            del config["input_size_multiplier"]
+            del (
+                config["input_size_multiplier"],
+                config["inference_input_size_multiplier"],
+            )
 
         super(AutoLSTM, self).__init__(
             cls_model=LSTM,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
@@ -145,15 +154,15 @@
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
-# %% ../nbs/models.ipynb 17
+# %% ../nbs/models.ipynb 16
 class AutoGRU(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
@@ -185,15 +194,18 @@
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
             config["inference_input_size"] = tune.choice(
                 [h * x for x in self.default_config["inference_input_size_multiplier"]]
             )
-            del config["input_size_multiplier"]
+            del (
+                config["input_size_multiplier"],
+                config["inference_input_size_multiplier"],
+            )
 
         super(AutoGRU, self).__init__(
             cls_model=GRU,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
@@ -202,15 +214,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 21
+# %% ../nbs/models.ipynb 19
 class AutoTCN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "context_size": tune.choice([5, 10, 50]),
@@ -241,15 +253,18 @@
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
             config["inference_input_size"] = tune.choice(
                 [h * x for x in self.default_config["inference_input_size_multiplier"]]
             )
-            del config["input_size_multiplier"]
+            del (
+                config["input_size_multiplier"],
+                config["inference_input_size_multiplier"],
+            )
 
         super(AutoTCN, self).__init__(
             cls_model=TCN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
@@ -258,15 +273,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 25
+# %% ../nbs/models.ipynb 22
 class AutoDilatedRNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "cell_type": tune.choice(["LSTM", "GRU"]),
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
@@ -299,15 +314,18 @@
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
             config["inference_input_size"] = tune.choice(
                 [h * x for x in self.default_config["inference_input_size_multiplier"]]
             )
-            del config["input_size_multiplier"]
+            del (
+                config["input_size_multiplier"],
+                config["inference_input_size_multiplier"],
+            )
 
         super(AutoDilatedRNN, self).__init__(
             cls_model=DilatedRNN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
@@ -316,15 +334,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 30
+# %% ../nbs/models.ipynb 26
 class AutoMLP(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([256, 512, 1024]),
         "num_layers": tune.randint(2, 6),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -373,15 +391,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 34
+# %% ../nbs/models.ipynb 29
 class AutoNBEATS(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
@@ -428,15 +446,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 38
+# %% ../nbs/models.ipynb 32
 class AutoNBEATSx(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
@@ -483,39 +501,43 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 42
+# %% ../nbs/models.ipynb 35
 class AutoNHITS(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_pool_kernel_size": tune.choice(
-            [3 * [1], 3 * [2], 3 * [4], [8, 4, 1], [16, 8, 1]]
+            [[2, 2, 1], 3 * [1], 3 * [2], 3 * [4], [8, 4, 1], [16, 8, 1]]
         ),
         "n_freq_downsample": tune.choice(
             [
                 [168, 24, 1],
                 [24, 12, 1],
                 [180, 60, 1],
                 [60, 8, 1],
                 [40, 20, 1],
                 [1, 1, 1],
             ]
         ),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
-        "max_steps": tune.choice([500, 1000]),
-        "batch_size": tune.choice([32, 64, 128, 256]),
-        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "max_steps": tune.quniform(lower=500, upper=1500, q=100),
+        "batch_size": tune.qloguniform(
+            lower=5, upper=9, base=2, q=1
+        ),  # [32, 64, 128, 256]
+        "windows_batch_size": tune.qloguniform(
+            lower=7, upper=10, base=2, q=1
+        ),  # [128, 256, 512, 1024]
         "loss": None,
-        "random_seed": tune.randint(1, 20),
+        "random_seed": tune.randint(lower=1, upper=20),
     }
 
     def __init__(
         self,
         h,
         loss=MAE(),
         valid_loss=None,
@@ -551,15 +573,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 47
+# %% ../nbs/models.ipynb 39
 class AutoTFT(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -608,15 +630,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 51
+# %% ../nbs/models.ipynb 42
 class AutoVanillaTransformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -665,15 +687,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 55
+# %% ../nbs/models.ipynb 45
 class AutoInformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -722,15 +744,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 59
+# %% ../nbs/models.ipynb 48
 class AutoAutoformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -779,15 +801,71 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 63
+# %% ../nbs/models.ipynb 51
+class AutoFEDformer(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([64, 128, 256]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoFEDformer, self).__init__(
+            cls_model=FEDformer,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 54
 class AutoPatchTST(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3],
         "h": None,
         "hidden_size": tune.choice([16, 128, 256]),
         "n_head": tune.choice([4, 16]),
         "patch_len": tune.choice([16, 24]),
@@ -838,15 +916,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 68
+# %% ../nbs/models.ipynb 59
 class AutoStemGNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_stacks": tune.choice([2, 3]),
         "multi_layer": tune.choice([3, 5, 7]),
@@ -898,7 +976,59 @@
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
+
+# %% ../nbs/models.ipynb 63
+class AutoHINT(BaseAuto):
+    def __init__(
+        self,
+        cls_model,
+        h,
+        loss,
+        valid_loss,
+        S,
+        config,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        refit_with_val=False,
+        verbose=False,
+        alias=None,
+    ):
+        super(AutoHINT, self).__init__(
+            cls_model=cls_model,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+        # Validate presence of reconciliation strategy
+        # parameter in configuration space
+        if not ("reconciliation" in config.keys()):
+            raise Exception(
+                "config needs reconciliation, \
+                            try tune.choice(['BottomUp', 'MinTraceOLS', 'MinTraceWLS'])"
+            )
+        self.S = S
+
+    def _fit_model(self, cls_model, config, dataset, val_size, test_size):
+        # Overwrite _fit_model for HINT two-stage instantiation
+        reconciliation = config.pop("reconciliation")
+        base_model = cls_model(**config)
+        model = HINT(
+            h=base_model.h, model=base_model, S=self.S, reconciliation=reconciliation
+        )
+        model.test_size = test_size
+        model.fit(dataset, val_size=val_size, test_size=test_size)
+        return model
```

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_base_auto.py` & `neuralforecast-1.6.0/neuralforecast/common/_base_auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,74 +11,17 @@
 import pytorch_lightning as pl
 
 from pytorch_lightning.callbacks import TQDMProgressBar
 from ray import air, tune
 from ray.tune.integration.pytorch_lightning import TuneReportCallback
 from ray.tune.search.basic_variant import BasicVariantGenerator
 
-from ..losses.pytorch import MAE
-
 # %% ../../nbs/common.base_auto.ipynb 6
-def train_tune(config_step, cls_model, dataset, val_size, test_size):
-    metrics = {"loss": "ptl/val_loss"}
-    callbacks = [TQDMProgressBar(), TuneReportCallback(metrics, on="validation_end")]
-    if "callbacks" in config_step.keys():
-        callbacks += config_step["callbacks"]
-    config_step = {**config_step, **{"callbacks": callbacks}}
-    model = cls_model(**config_step)
-    model.fit(dataset, val_size=val_size, test_size=test_size)
-
-# %% ../../nbs/common.base_auto.ipynb 7
-def tune_model(
-    cls_model,
-    dataset,
-    val_size,
-    test_size,
-    cpus,
-    gpus,
-    verbose,
-    num_samples,
-    search_alg,
-    config,
-):
-    train_fn_with_parameters = tune.with_parameters(
-        train_tune,
-        cls_model=cls_model,
-        dataset=dataset,
-        val_size=val_size,
-        test_size=test_size,
-    )
-
-    # Device
-    if gpus > 0:
-        device_dict = {"gpu": gpus}
-    else:
-        device_dict = {"cpu": cpus}
-
-    tuner = tune.Tuner(
-        tune.with_resources(train_fn_with_parameters, device_dict),
-        run_config=air.RunConfig(
-            verbose=verbose,
-            # checkpoint_config=air.CheckpointConfig(
-            # num_to_keep=0,
-            # keep_checkpoints_num=None
-            # )
-        ),
-        tune_config=tune.TuneConfig(
-            metric="loss", mode="min", num_samples=num_samples, search_alg=search_alg
-        ),
-        param_space=config,
-    )
-    results = tuner.fit()
-    return results
-
-# %% ../../nbs/common.base_auto.ipynb 8
 class BaseAuto(pl.LightningModule):
-    """BaseAuto
-
+    """
     Class for Automatic Hyperparameter Optimization, it builds on top of `ray` to
     give access to a wide variety of hyperparameter optimization tools ranging
     from classic grid search, to Bayesian optimization and HyperBand algorithm.
 
     The validation loss to be optimized is defined by the `config['loss']` dictionary
     value, the config also contains the rest of the hyperparameter search space.
 
@@ -129,75 +72,183 @@
             raise Exception(
                 "Please use `valid_loss` init argument instead of `config['valid_loss']`."
             )
 
         # Deepcopy to avoid modifying the original config
         config_base = deepcopy(config)
 
+        # Add losses to config and protect valid_loss default
         config_base["h"] = h
         config_base["loss"] = loss
         if valid_loss is None:
             valid_loss = loss
         config_base["valid_loss"] = valid_loss
-        self.cls_model = cls_model
+
         self.h = h
-        self.loss = loss
+        self.cls_model = cls_model
+
         self.config = config_base
+        self.loss = self.config["loss"]
+        self.valid_loss = self.config["valid_loss"]
+
+        # This attribute helps to protect
+        # model and datasets interactions protections
+        if "early_stop_patience_steps" in config.keys():
+            self.early_stop_patience_steps = 1
+        else:
+            self.early_stop_patience_steps = -1
+
         self.num_samples = num_samples
         self.search_alg = search_alg
         self.cpus = cpus
         self.gpus = gpus
         self.refit_with_val = refit_with_val
         self.verbose = verbose
-        self.loss = self.config.get("loss", MAE())
-        self.valid_loss = self.config.get("valid_loss", self.loss)
         self.alias = alias
 
         # Base Class attributes
         self.SAMPLING_TYPE = cls_model.SAMPLING_TYPE
 
     def __repr__(self):
         return type(self).__name__ if self.alias is None else self.alias
 
-    def fit(self, dataset, val_size=0, test_size=0):
+    def _train_tune(self, config_step, cls_model, dataset, val_size, test_size):
+        """BaseAuto._train_tune
+
+        Internal function that instantiates a NF class model, then automatically
+        explores the validation loss (ptl/val_loss) on which the hyperparameter
+        exploration is based.
+
+        **Parameters:**<br>
+        `config_step`: Dict, initialization parameters of a NF model.<br>
+        `cls_model`: NeuralForecast model class, yet to be instantiated.<br>
+        `dataset`: NeuralForecast dataset, to fit the model.<br>
+        `val_size`: int, validation size for temporal cross-validation.<br>
+        `test_size`: int, test size for temporal cross-validation.<br>
+        """
+        metrics = {"loss": "ptl/val_loss"}
+        callbacks = [
+            TQDMProgressBar(),
+            TuneReportCallback(metrics, on="validation_end"),
+        ]
+        if "callbacks" in config_step.keys():
+            callbacks += config_step["callbacks"]
+        config_step = {**config_step, **{"callbacks": callbacks}}
+
+        # Protect dtypes from tune samplers
+        if "batch_size" in config_step.keys():
+            config_step["batch_size"] = int(config_step["batch_size"])
+        if "windows_batch_size" in config_step.keys():
+            config_step["windows_batch_size"] = int(config_step["windows_batch_size"])
+
+        # Tune session receives validation signal
+        # from the specialized PL TuneReportCallback
+        _ = self._fit_model(
+            cls_model=cls_model,
+            config=config_step,
+            dataset=dataset,
+            val_size=val_size,
+            test_size=test_size,
+        )
+
+    def _tune_model(
+        self,
+        cls_model,
+        dataset,
+        val_size,
+        test_size,
+        cpus,
+        gpus,
+        verbose,
+        num_samples,
+        search_alg,
+        config,
+    ):
+        train_fn_with_parameters = tune.with_parameters(
+            self._train_tune,
+            cls_model=cls_model,
+            dataset=dataset,
+            val_size=val_size,
+            test_size=test_size,
+        )
+
+        # Device
+        if gpus > 0:
+            device_dict = {"gpu": gpus}
+        else:
+            device_dict = {"cpu": cpus}
+
+        tuner = tune.Tuner(
+            tune.with_resources(train_fn_with_parameters, device_dict),
+            run_config=air.RunConfig(
+                verbose=verbose,
+                # checkpoint_config=air.CheckpointConfig(
+                # num_to_keep=0,
+                # keep_checkpoints_num=None
+                # )
+            ),
+            tune_config=tune.TuneConfig(
+                metric="loss",
+                mode="min",
+                num_samples=num_samples,
+                search_alg=search_alg,
+            ),
+            param_space=config,
+        )
+        results = tuner.fit()
+        return results
+
+    def _fit_model(self, cls_model, config, dataset, val_size, test_size):
+        model = cls_model(**config)
+        model.fit(dataset, val_size=val_size, test_size=test_size)
+        return model
+
+    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
         """BaseAuto.fit
 
         Perform the hyperparameter optimization as specified by the BaseAuto configuration
         dictionary `config`.
 
         The optimization is performed on the `TimeSeriesDataset` using temporal cross validation with
         the validation set that sequentially precedes the test set.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset` see details [here](https://nixtla.github.io/neuralforecast/tsdataset.html)<br>
         `val_size`: int, size of temporal validation set (needs to be bigger than 0).<br>
         `test_size`: int, size of temporal test set (default 0).<br>
-
+        `random_seed`: int=None, random_seed for hyperparameter exploration algorithms, not yet implemented.<br>
         **Returns:**<br>
         `self`: fitted instance of `BaseAuto` with best hyperparameters and results<br>.
         """
         # we need val_size > 0 to perform
         # hyperparameter selection.
         search_alg = deepcopy(self.search_alg)
         val_size = val_size if val_size > 0 else self.h
-        results = tune_model(
+        results = self._tune_model(
             cls_model=self.cls_model,
             dataset=dataset,
             val_size=val_size,
             test_size=test_size,
             cpus=self.cpus,
             gpus=self.gpus,
             verbose=self.verbose,
             num_samples=self.num_samples,
             search_alg=search_alg,
             config=self.config,
         )
         best_config = results.get_best_result().config
-        self.model = self.cls_model(**best_config)
-        self.model.fit(
+        # self.model = self.cls_model(**best_config)
+        # self.model.fit(
+        #    dataset=dataset,
+        #    val_size=val_size * (1 - self.refit_with_val),
+        #    test_size=test_size,
+        # )
+        self.model = self._fit_model(
+            cls_model=self.cls_model,
+            config=best_config,
             dataset=dataset,
             val_size=val_size * (1 - self.refit_with_val),
             test_size=test_size,
         )
         self.results = results
 
     def predict(self, dataset, step_size=1, **data_kwargs):
@@ -205,15 +256,15 @@
 
         Predictions of the best performing model on validation.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset` see details [here](https://nixtla.github.io/neuralforecast/tsdataset.html)<br>
         `step_size`: int, steps between sequential predictions, (default 1).<br>
         `**data_kwarg`: additional parameters for the dataset module.<br>
-
+        `random_seed`: int=None, random_seed for hyperparameter exploration algorithms (not implemented).<br>
         **Returns:**<br>
         `y_hat`: numpy predictions of the `NeuralForecast` model.<br>
         """
         return self.model.predict(dataset=dataset, step_size=step_size, **data_kwargs)
 
     def set_test_size(self, test_size):
         self.model.set_test_size(test_size)
```

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_base_multivariate.py` & `neuralforecast-1.6.0/neuralforecast/common/_base_multivariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,21 +104,18 @@
         self.test_size = 0
 
         # Model state
         self.decompose_forecast = False
 
         ## Trainer arguments ##
         # Max steps, validation steps and check_val_every_n_epoch
-        if "max_epochs" in trainer_kwargs.keys():
-            warnings.warn("max_epochs will be deprecated, use max_steps instead.")
-        else:
-            trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
+        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
 
         if "max_epochs" in trainer_kwargs.keys():
-            warnings.warn("max_epochs will be deprecated, use max_steps instead.")
+            raise Exception("max_epochs is deprecated, use max_steps instead.")
 
         # Callbacks
         if trainer_kwargs.get("callbacks", None) is None:
             callbacks = [TQDMProgressBar()]
             # Early stopping
             if self.early_stop_patience_steps > 0:
                 callbacks += [
@@ -407,14 +404,21 @@
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             loss = self.loss(y=outsample_y, distr_args=distr_args, mask=outsample_mask)
         else:
             loss = self.loss(y=outsample_y, y_hat=output, mask=outsample_mask)
 
+        if torch.isnan(loss):
+            print("Model Parameters", self.hparams)
+            print("insample_y", torch.isnan(insample_y).sum())
+            print("outsample_y", torch.isnan(outsample_y).sum())
+            print("output", torch.isnan(output).sum())
+            raise Exception("Loss is NaN, training stopped.")
+
         self.log("train_loss", loss, prog_bar=True, on_epoch=True)
         self.train_trajectories.append((self.global_step, float(loss)))
         return loss
 
     def validation_step(self, batch, batch_idx):
         if self.val_size == 0:
             return np.nan
@@ -464,14 +468,17 @@
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
+        if torch.isnan(valid_loss):
+            raise Exception("Loss is NaN, training stopped.")
+
         self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def on_validation_epoch_end(self):
         if self.val_size == 0:
             return
@@ -558,34 +565,22 @@
         datamodule = TimeSeriesDataModule(
             dataset=dataset,
             batch_size=self.n_series,
             num_workers=self.num_workers_loader,
             drop_last=self.drop_last_loader,
         )
 
-        ### Check validation every steps ###
-        steps_in_epoch = np.ceil(dataset.n_groups / self.n_series)
-
-        assert steps_in_epoch == 1, "n_series must be equal to number of series"
-
-        # In v1.6.5 of PL, val_check_interval can be used for multiple validation steps
-        # within one epoch (steps_in_epoch > self.val_check_steps)
-        if steps_in_epoch > self.val_check_steps:
-            val_check_interval = self.val_check_steps / steps_in_epoch
-            check_val_every_n_epoch = 1
-        # Use check_val_every_n_epoch to check validation at end of some epochs,
-        # closest to self.val_check_steps.
-        else:
-            val_check_interval = None
-            check_val_every_n_epoch = int(
-                np.round(self.val_check_steps / steps_in_epoch)
-            )
-
-        self.trainer_kwargs["val_check_interval"] = val_check_interval
-        self.trainer_kwargs["check_val_every_n_epoch"] = check_val_every_n_epoch
+        if self.val_check_steps > self.max_steps:
+            warnings.warn(
+                "val_check_steps is greater than max_steps, \
+                    setting val_check_steps to max_steps"
+            )
+        val_check_interval = min(self.val_check_steps, self.max_steps)
+        self.trainer_kwargs["val_check_interval"] = int(val_check_interval)
+        self.trainer_kwargs["check_val_every_n_epoch"] = None
 
         trainer = pl.Trainer(**self.trainer_kwargs)
         trainer.fit(self, datamodule=datamodule)
 
     def predict(
         self,
         dataset,
```

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_base_recurrent.py` & `neuralforecast-1.6.0/neuralforecast/common/_base_recurrent.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,23 @@
         if valid_loss is None:
             self.valid_loss = loss
         else:
             self.valid_loss = valid_loss
         self.train_trajectories = []
         self.valid_trajectories = []
 
+        if (
+            str(type(self.loss))
+            == "<class 'neuralforecast.losses.pytorch.DistributionLoss'>"
+            and self.loss.distribution == "Bernoulli"
+        ):
+            raise Exception(
+                "Temporal Classification not yet available for Recurrent-based models"
+            )
+
         # Valid batch_size
         self.batch_size = batch_size
         if valid_batch_size is None:
             self.valid_batch_size = batch_size
         else:
             self.valid_batch_size = valid_batch_size
 
@@ -105,18 +114,18 @@
 
         # Fit arguments
         self.val_size = 0
         self.test_size = 0
 
         ## Trainer arguments ##
         # Max steps, validation steps and check_val_every_n_epoch
+        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
+
         if "max_epochs" in trainer_kwargs.keys():
-            warnings.warn("max_epochs will be deprecated, use max_steps instead.")
-        else:
-            trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
+            raise Exception("max_epochs is deprecated, use max_steps instead.")
 
         # Callbacks
         if trainer_kwargs.get("callbacks", None) is None:
             callbacks = [TQDMProgressBar()]
             # Early stopping
             if self.early_stop_patience_steps > 0:
                 callbacks += [
@@ -374,14 +383,21 @@
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             loss = self.loss(y=outsample_y, distr_args=distr_args, mask=outsample_mask)
         else:
             loss = self.loss(y=outsample_y, y_hat=output, mask=outsample_mask)
 
+        if torch.isnan(loss):
+            print("Model Parameters", self.hparams)
+            print("insample_y", torch.isnan(insample_y).sum())
+            print("outsample_y", torch.isnan(outsample_y).sum())
+            print("output", torch.isnan(output).sum())
+            raise Exception("Loss is NaN, training stopped.")
+
         self.log(
             "train_loss", loss, batch_size=self.batch_size, prog_bar=True, on_epoch=True
         )
         self.train_trajectories.append((self.global_step, float(loss)))
         return loss
 
     def validation_step(self, batch, batch_idx):
@@ -458,14 +474,17 @@
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
+        if torch.isnan(valid_loss):
+            raise Exception("Loss is NaN, training stopped.")
+
         self.log(
             "valid_loss",
             valid_loss,
             batch_size=self.batch_size,
             prog_bar=True,
             on_epoch=True,
         )
@@ -549,14 +568,15 @@
         By default the `model` is not saving training checkpoints to protect
         disk memory, to get them change `enable_checkpointing=True` in `__init__`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `val_size`: int, validation size for temporal cross-validation.<br>
         `test_size`: int, test size for temporal cross-validation.<br>
+        `random_seed`: int=None, random_seed for pytorch initializer and numpy generators, overwrites model.__init__'s.<br>
         """
         # Restart random seed
         if random_seed is None:
             random_seed = self.random_seed
         torch.manual_seed(random_seed)
 
         self.val_size = val_size
@@ -565,44 +585,35 @@
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             num_workers=self.num_workers_loader,
             drop_last=self.drop_last_loader,
         )
 
-        ### Check validation every steps ###
-        steps_in_epoch = np.ceil(dataset.n_groups / self.batch_size)
-
-        # In v1.6.5 of PL, val_check_interval can be used for multiple validation steps
-        # within one epoch (steps_in_epoch > self.val_check_steps)
-        if steps_in_epoch > self.val_check_steps:
-            val_check_interval = self.val_check_steps / steps_in_epoch
-            check_val_every_n_epoch = 1
-        # Use check_val_every_n_epoch to check validation at end of some epochs,
-        # closest to self.val_check_steps.
-        else:
-            val_check_interval = None
-            check_val_every_n_epoch = int(
-                np.round(self.val_check_steps / steps_in_epoch)
-            )
-
-        self.trainer_kwargs["val_check_interval"] = val_check_interval
-        self.trainer_kwargs["check_val_every_n_epoch"] = check_val_every_n_epoch
+        if self.val_check_steps > self.max_steps:
+            warnings.warn(
+                "val_check_steps is greater than max_steps, \
+                    setting val_check_steps to max_steps"
+            )
+        val_check_interval = min(self.val_check_steps, self.max_steps)
+        self.trainer_kwargs["val_check_interval"] = int(val_check_interval)
+        self.trainer_kwargs["check_val_every_n_epoch"] = None
 
         trainer = pl.Trainer(**self.trainer_kwargs)
         trainer.fit(self, datamodule=datamodule)
 
     def predict(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """Predict.
 
         Neural network prediction with PL's `Trainer` execution of `predict_step`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `step_size`: int=1, Step size between each window.<br>
+        `random_seed`: int=None, random_seed for pytorch initializer and numpy generators, overwrites model.__init__'s.<br>
         `**data_module_kwargs`: PL's TimeSeriesDataModule args, see [documentation](https://pytorch-lightning.readthedocs.io/en/1.6.1/extensions/datamodules.html#using-a-datamodule).
         """
         # Restart random seed
         if random_seed is None:
             random_seed = self.random_seed
         torch.manual_seed(random_seed)
```

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_base_windows.py` & `neuralforecast-1.6.0/neuralforecast/common/_base_windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,23 +36,25 @@
         input_size,
         loss,
         valid_loss,
         learning_rate,
         max_steps,
         val_check_steps,
         batch_size,
-        windows_batch_size,
         valid_batch_size,
+        windows_batch_size,
+        inference_windows_batch_size,
         step_size=1,
         num_lr_decays=0,
         early_stop_patience_steps=-1,
         scaler_type="identity",
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
+        exclude_insample_y=False,
         num_workers_loader=0,
         drop_last_loader=False,
         random_seed=1,
         alias=None,
         **trainer_kwargs,
     ):
         super(BaseWindows, self).__init__()
@@ -72,20 +74,24 @@
         if valid_loss is None:
             self.valid_loss = loss
         else:
             self.valid_loss = valid_loss
         self.train_trajectories = []
         self.valid_trajectories = []
 
-        # Valid batch_size
+        # Batch sizes
         self.batch_size = batch_size
         if valid_batch_size is None:
             self.valid_batch_size = batch_size
         else:
             self.valid_batch_size = valid_batch_size
+        if inference_windows_batch_size is None:
+            self.inference_windows_batch_size = windows_batch_size
+        else:
+            self.inference_windows_batch_size = inference_windows_batch_size
 
         # Optimization
         self.learning_rate = learning_rate
         self.max_steps = max_steps
         self.num_lr_decays = num_lr_decays
         self.lr_decay_steps = (
             max(max_steps // self.num_lr_decays, 1) if self.num_lr_decays > 0 else 10e7
@@ -100,31 +106,29 @@
             scaler_type=scaler_type, dim=1
         )  # Time dimension is 1.
 
         # Variables
         self.futr_exog_list = futr_exog_list if futr_exog_list is not None else []
         self.hist_exog_list = hist_exog_list if hist_exog_list is not None else []
         self.stat_exog_list = stat_exog_list if stat_exog_list is not None else []
+        self.exclude_insample_y = exclude_insample_y
 
         # Fit arguments
         self.val_size = 0
         self.test_size = 0
 
         # Model state
         self.decompose_forecast = False
 
         ## Trainer arguments ##
         # Max steps, validation steps and check_val_every_n_epoch
-        if "max_epochs" in trainer_kwargs.keys():
-            warnings.warn("max_epochs will be deprecated, use max_steps instead.")
-        else:
-            trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
+        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
 
         if "max_epochs" in trainer_kwargs.keys():
-            warnings.warn("max_epochs will be deprecated, use max_steps instead.")
+            raise Exception("max_epochs is deprecated, use max_steps instead.")
 
         # Callbacks
         if trainer_kwargs.get("callbacks", None) is None:
             callbacks = [TQDMProgressBar()]
             # Early stopping
             if self.early_stop_patience_steps > 0:
                 callbacks += [
@@ -171,15 +175,15 @@
                 optimizer=optimizer, step_size=self.lr_decay_steps, gamma=0.5
             ),
             "frequency": 1,
             "interval": "step",
         }
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
-    def _create_windows(self, batch, step):
+    def _create_windows(self, batch, step, w_idxs=None):
         # Parse common data
         window_size = self.input_size + self.h
         temporal_cols = batch["temporal_cols"]
         temporal = batch["temporal"]
 
         if step == "train":
             if self.val_size + self.test_size > 0:
@@ -285,14 +289,20 @@
             static = batch.get("static", None)
             static_cols = batch.get("static_cols", None)
             if static is not None:
                 static = torch.repeat_interleave(
                     static, repeats=windows_per_serie, dim=0
                 )
 
+            # Sample windows for batched prediction
+            if w_idxs is not None:
+                windows = windows[w_idxs]
+                if static is not None:
+                    static = static[w_idxs]
+
             windows_batch = dict(
                 temporal=windows,
                 temporal_cols=temporal_cols,
                 static=static,
                 static_cols=static_cols,
             )
             return windows_batch
@@ -334,18 +344,24 @@
         else:
             remove_dimension = False
 
         temporal_data_cols = temporal_cols.drop("available_mask")
         y_scale = self.scaler.x_scale[:, :, temporal_data_cols.get_indexer(["y"])]
         y_loc = self.scaler.x_shift[:, :, temporal_data_cols.get_indexer(["y"])]
 
-        y_scale = torch.repeat_interleave(y_scale, repeats=y_hat.shape[-1], dim=-1)
-        y_loc = torch.repeat_interleave(y_loc, repeats=y_hat.shape[-1], dim=-1)
+        y_scale = torch.repeat_interleave(y_scale, repeats=y_hat.shape[-1], dim=-1).to(
+            y_hat.device
+        )
+        y_loc = torch.repeat_interleave(y_loc, repeats=y_hat.shape[-1], dim=-1).to(
+            y_hat.device
+        )
 
         y_hat = self.scaler.inverse_transform(z=y_hat, x_scale=y_scale, x_shift=y_loc)
+        y_loc = y_loc.to(y_hat.device)
+        y_scale = y_scale.to(y_hat.device)
 
         if remove_dimension:
             y_hat = y_hat.squeeze(-1)
             y_loc = y_loc.squeeze(-1)
             y_scale = y_scale.squeeze(-1)
 
         return y_hat, y_loc, y_scale
@@ -375,14 +391,17 @@
         # Filter static variables
         if len(self.stat_exog_list):
             static_idx = windows["static_cols"].get_indexer(self.stat_exog_list)
             stat_exog = windows["static"][:, static_idx]
         else:
             stat_exog = None
 
+        if self.exclude_insample_y:
+            insample_y = insample_y * 0
+
         return (
             insample_y,
             insample_mask,
             outsample_y,
             outsample_mask,
             hist_exog,
             futr_exog,
@@ -424,53 +443,30 @@
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             loss = self.loss(y=outsample_y, distr_args=distr_args, mask=outsample_mask)
         else:
             loss = self.loss(y=outsample_y, y_hat=output, mask=outsample_mask)
 
+        if torch.isnan(loss):
+            print("Model Parameters", self.hparams)
+            print("insample_y", torch.isnan(insample_y).sum())
+            print("outsample_y", torch.isnan(outsample_y).sum())
+            print("output", torch.isnan(output).sum())
+            raise Exception("Loss is NaN, training stopped.")
+
         self.log("train_loss", loss, prog_bar=True, on_epoch=True)
         self.train_trajectories.append((self.global_step, float(loss)))
         return loss
 
-    def validation_step(self, batch, batch_idx):
-        if self.val_size == 0:
-            return np.nan
-
-        # Create and normalize windows [Ws, L+H, C]
-        windows = self._create_windows(batch, step="val")
-        original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
-        windows = self._normalization(windows=windows)
-
-        # Parse windows
-        (
-            insample_y,
-            insample_mask,
-            outsample_y,
-            outsample_mask,
-            hist_exog,
-            futr_exog,
-            stat_exog,
-        ) = self._parse_windows(batch, windows)
-
-        windows_batch = dict(
-            insample_y=insample_y,  # [Ws, L]
-            insample_mask=insample_mask,  # [Ws, L]
-            futr_exog=futr_exog,  # [Ws, L+H]
-            hist_exog=hist_exog,  # [Ws, L]
-            stat_exog=stat_exog,
-        )  # [Ws, 1]
-
-        # Model Predictions
-        output = self(windows_batch)
+    def _compute_valid_loss(self, outsample_y, output, outsample_mask, temporal_cols):
         if self.loss.is_distribution_output:
             _, y_loc, y_scale = self._inv_normalization(
-                y_hat=outsample_y, temporal_cols=batch["temporal_cols"]
+                y_hat=outsample_y, temporal_cols=temporal_cols
             )
-            outsample_y = original_outsample_y
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
 
             if str(type(self.valid_loss)) in [
                 "<class 'neuralforecast.losses.pytorch.sCRPS'>",
@@ -487,73 +483,152 @@
             valid_loss = self.valid_loss(
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
+        return valid_loss
+
+    def validation_step(self, batch, batch_idx):
+        if self.val_size == 0:
+            return np.nan
+
+        # TODO: Hack to compute number of windows
+        windows = self._create_windows(batch, step="val")
+        n_windows = len(windows["temporal"])
+
+        # Number of windows in batch
+        windows_batch_size = self.inference_windows_batch_size
+        if windows_batch_size < 0:
+            windows_batch_size = n_windows
+        n_batches = int(np.ceil(n_windows / windows_batch_size))
+
+        valid_losses = []
+        batch_sizes = []
+        for i in range(n_batches):
+            # Create and normalize windows [Ws, L+H, C]
+            w_idxs = np.arange(
+                i * windows_batch_size, min((i + 1) * windows_batch_size, n_windows)
+            )
+            windows = self._create_windows(batch, step="val", w_idxs=w_idxs)
+            original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
+            windows = self._normalization(windows=windows)
+
+            # Parse windows
+            (
+                insample_y,
+                insample_mask,
+                _,
+                outsample_mask,
+                hist_exog,
+                futr_exog,
+                stat_exog,
+            ) = self._parse_windows(batch, windows)
+            windows_batch = dict(
+                insample_y=insample_y,  # [Ws, L]
+                insample_mask=insample_mask,  # [Ws, L]
+                futr_exog=futr_exog,  # [Ws, L+H]
+                hist_exog=hist_exog,  # [Ws, L]
+                stat_exog=stat_exog,
+            )  # [Ws, 1]
+
+            # Model Predictions
+            output_batch = self(windows_batch)
+            valid_loss_batch = self._compute_valid_loss(
+                outsample_y=original_outsample_y,
+                output=output_batch,
+                outsample_mask=outsample_mask,
+                temporal_cols=batch["temporal_cols"],
+            )
+            valid_losses.append(valid_loss_batch)
+            batch_sizes.append(len(output_batch))
+
+        valid_loss = torch.stack(valid_losses)
+        batch_sizes = torch.tensor(batch_sizes).to(valid_loss.device)
+        valid_loss = torch.sum(valid_loss * batch_sizes) / torch.sum(batch_sizes)
+
+        if torch.isnan(valid_loss):
+            raise Exception("Loss is NaN, training stopped.")
 
         self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def on_validation_epoch_end(self):
         if self.val_size == 0:
             return
         avg_loss = torch.stack(self.validation_step_outputs).mean()
         self.log("ptl/val_loss", avg_loss)
         self.valid_trajectories.append((self.global_step, float(avg_loss)))
         self.validation_step_outputs.clear()  # free memory (compute `avg_loss` per epoch)
 
     def predict_step(self, batch, batch_idx):
-        # Create and normalize windows [Ws, L+H, C]
+        # TODO: Hack to compute number of windows
         windows = self._create_windows(batch, step="predict")
-        windows = self._normalization(windows=windows)
-
-        # Parse windows
-        (
-            insample_y,
-            insample_mask,
-            _,
-            _,
-            hist_exog,
-            futr_exog,
-            stat_exog,
-        ) = self._parse_windows(batch, windows)
-
-        windows_batch = dict(
-            insample_y=insample_y,  # [Ws, L]
-            insample_mask=insample_mask,  # [Ws, L]
-            futr_exog=futr_exog,  # [Ws, L+H]
-            hist_exog=hist_exog,  # [Ws, L]
-            stat_exog=stat_exog,
-        )  # [Ws, 1]
+        n_windows = len(windows["temporal"])
 
-        # Model Predictions
-        output = self(windows_batch)
-        if self.loss.is_distribution_output:
-            _, y_loc, y_scale = self._inv_normalization(
-                y_hat=output[0], temporal_cols=batch["temporal_cols"]
-            )
-            distr_args = self.loss.scale_decouple(
-                output=output, loc=y_loc, scale=y_scale
-            )
-            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
-            y_hat = torch.concat((sample_mean, quants), axis=2)
+        # Number of windows in batch
+        windows_batch_size = self.inference_windows_batch_size
+        if windows_batch_size < 0:
+            windows_batch_size = n_windows
+        n_batches = int(np.ceil(n_windows / windows_batch_size))
+
+        y_hats = []
+        for i in range(n_batches):
+            # Create and normalize windows [Ws, L+H, C]
+            w_idxs = np.arange(
+                i * windows_batch_size, min((i + 1) * windows_batch_size, n_windows)
+            )
+            windows = self._create_windows(batch, step="predict", w_idxs=w_idxs)
+            windows = self._normalization(windows=windows)
+
+            # Parse windows
+            (
+                insample_y,
+                insample_mask,
+                _,
+                _,
+                hist_exog,
+                futr_exog,
+                stat_exog,
+            ) = self._parse_windows(batch, windows)
+            windows_batch = dict(
+                insample_y=insample_y,  # [Ws, L]
+                insample_mask=insample_mask,  # [Ws, L]
+                futr_exog=futr_exog,  # [Ws, L+H]
+                hist_exog=hist_exog,  # [Ws, L]
+                stat_exog=stat_exog,
+            )  # [Ws, 1]
+
+            # Model Predictions
+            output_batch = self(windows_batch)
+            # Inverse normalization and sampling
+            if self.loss.is_distribution_output:
+                _, y_loc, y_scale = self._inv_normalization(
+                    y_hat=output_batch[0], temporal_cols=batch["temporal_cols"]
+                )
+                distr_args = self.loss.scale_decouple(
+                    output=output_batch, loc=y_loc, scale=y_scale
+                )
+                _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
+                y_hat = torch.concat((sample_mean, quants), axis=2)
 
-            if self.loss.return_params:
-                distr_args = torch.stack(distr_args, dim=-1)
-                distr_args = torch.reshape(
-                    distr_args, (len(windows["temporal"]), self.h, -1)
+                if self.loss.return_params:
+                    distr_args = torch.stack(distr_args, dim=-1)
+                    distr_args = torch.reshape(
+                        distr_args, (len(windows["temporal"]), self.h, -1)
+                    )
+                    y_hat = torch.concat((y_hat, distr_args), axis=2)
+            else:
+                y_hat, _, _ = self._inv_normalization(
+                    y_hat=output_batch, temporal_cols=batch["temporal_cols"]
                 )
-                y_hat = torch.concat((y_hat, distr_args), axis=2)
-        else:
-            y_hat, _, _ = self._inv_normalization(
-                y_hat=output, temporal_cols=batch["temporal_cols"]
-            )
+            y_hats.append(y_hat)
+        y_hat = torch.cat(y_hats, dim=0)
         return y_hat
 
     def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `windows_batch_size`, ...)
@@ -567,14 +642,15 @@
 
         By default the `model` is not saving training checkpoints to protect
         disk memory, to get them change `enable_checkpointing=True` in `__init__`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `val_size`: int, validation size for temporal cross-validation.<br>
+        `random_seed`: int=None, random_seed for pytorch initializer and numpy generators, overwrites model.__init__'s.<br>
         `test_size`: int, test size for temporal cross-validation.<br>
         """
         # Restart random seed
         if random_seed is None:
             random_seed = self.random_seed
         torch.manual_seed(random_seed)
 
@@ -584,32 +660,22 @@
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             num_workers=self.num_workers_loader,
             drop_last=self.drop_last_loader,
         )
 
-        ### Check validation every steps ###
-        steps_in_epoch = np.ceil(dataset.n_groups / self.batch_size)
-
-        # In v1.6.5 of PL, val_check_interval can be used for multiple validation steps
-        # within one epoch (steps_in_epoch > self.val_check_steps)
-        if steps_in_epoch > self.val_check_steps:
-            val_check_interval = self.val_check_steps / steps_in_epoch
-            check_val_every_n_epoch = 1
-        # Use check_val_every_n_epoch to check validation at end of some epochs,
-        # closest to self.val_check_steps.
-        else:
-            val_check_interval = None
-            check_val_every_n_epoch = int(
-                np.round(self.val_check_steps / steps_in_epoch)
-            )
-
-        self.trainer_kwargs["val_check_interval"] = val_check_interval
-        self.trainer_kwargs["check_val_every_n_epoch"] = check_val_every_n_epoch
+        if self.val_check_steps > self.max_steps:
+            warnings.warn(
+                "val_check_steps is greater than max_steps, \
+                    setting val_check_steps to max_steps"
+            )
+        val_check_interval = min(self.val_check_steps, self.max_steps)
+        self.trainer_kwargs["val_check_interval"] = int(val_check_interval)
+        self.trainer_kwargs["check_val_every_n_epoch"] = None
 
         trainer = pl.Trainer(**self.trainer_kwargs)
         trainer.fit(self, datamodule=datamodule)
 
     def predict(
         self,
         dataset,
@@ -622,14 +688,15 @@
 
         Neural network prediction with PL's `Trainer` execution of `predict_step`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `test_size`: int=None, test size for temporal cross-validation.<br>
         `step_size`: int=1, Step size between each window.<br>
+        `random_seed`: int=None, random_seed for pytorch initializer and numpy generators, overwrites model.__init__'s.<br>
         `**data_module_kwargs`: PL's TimeSeriesDataModule args, see [documentation](https://pytorch-lightning.readthedocs.io/en/1.6.1/extensions/datamodules.html#using-a-datamodule).
         """
         # Restart random seed
         if random_seed is None:
             random_seed = self.random_seed
         torch.manual_seed(random_seed)
```

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_modules.py` & `neuralforecast-1.6.0/neuralforecast/common/_modules.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/common/_scalers.py` & `neuralforecast-1.6.0/neuralforecast/common/_scalers.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,25 @@
             dimension dim to avoid NaNs from zero division.<br>
     `eps` (float, optional): Small value to avoid division by zero. Defaults to 1e-6.<br>
     `dim` (int, optional): Dimension over to compute min and max. Defaults to -1.<br>
 
     **Returns:**<br>
     `z`: torch.Tensor same shape as `x`, except scaled.
     """
-    max_mask = (mask == 0) * (-1e12)
-    min_mask = (mask == 0) * (1e12)
-    x_max = torch.max(x + max_mask, dim=dim, keepdim=True)[0]
-    x_min = torch.min(x + min_mask, dim=dim, keepdim=True)[0]
+    mask = mask.clone()
+    mask[mask == 0] = torch.inf
+    mask[mask == 1] = 0
+    x_max = torch.max(
+        torch.nan_to_num(x - mask, nan=-torch.inf), dim=dim, keepdim=True
+    )[0]
+    x_min = torch.min(torch.nan_to_num(x + mask, nan=torch.inf), dim=dim, keepdim=True)[
+        0
+    ]
+    x_max = x_max.type(x.dtype)
+    x_min = x_min.type(x.dtype)
 
     # x_range and prevent division by zero
     x_range = x_max - x_min
     x_range[x_range == 0] = 1.0
     x_range = x_range + eps
 
     z = (x - x_min) / x_range
@@ -111,18 +118,26 @@
             dimension dim to avoid NaNs from zero division.<br>
     `eps` (float, optional): Small value to avoid division by zero. Defaults to 1e-6.<br>
     `dim` (int, optional): Dimension over to compute min and max. Defaults to -1.<br>
 
     **Returns:**<br>
     `z`: torch.Tensor same shape as `x`, except scaled.
     """
-    max_mask = (mask == 0) * (-1e12)
-    min_mask = (mask == 0) * (1e12)
-    x_max = torch.max(x + max_mask, dim=dim, keepdim=True)[0]
-    x_min = torch.min(x + min_mask, dim=dim, keepdim=True)[0]
+    # Mask values (set masked to -inf or +inf)
+    mask = mask.clone()
+    mask[mask == 0] = torch.inf
+    mask[mask == 1] = 0
+    x_max = torch.max(
+        torch.nan_to_num(x - mask, nan=-torch.inf), dim=dim, keepdim=True
+    )[0]
+    x_min = torch.min(torch.nan_to_num(x + mask, nan=torch.inf), dim=dim, keepdim=True)[
+        0
+    ]
+    x_max = x_max.type(x.dtype)
+    x_min = x_min.type(x.dtype)
 
     # x_range and prevent division by zero
     x_range = x_max - x_min
     x_range[x_range == 0] = 1.0
     x_range = x_range + eps
 
     x = (x - x_min) / x_range
@@ -197,17 +212,18 @@
     **Returns:**<br>
     `z`: torch.Tensor same shape as `x`, except scaled.
     """
     x_median = masked_median(x=x, mask=mask, dim=dim)
     x_mad = masked_median(x=torch.abs(x - x_median), mask=mask, dim=dim)
 
     # Protect x_mad=0 values
+    # Assuming normality and relationship between mad and std
     x_means = masked_mean(x=x, mask=mask, dim=dim)
     x_stds = torch.sqrt(masked_mean(x=(x - x_means) ** 2, mask=mask, dim=dim))
-    x_mad_aux = x_stds / 0.6744897501960817
+    x_mad_aux = x_stds * 0.6744897501960817
     x_mad = x_mad * (x_mad > 0) + x_mad_aux * (x_mad == 0)
 
     # Protect against division by zero
     x_mad[x_mad == 0] = 1.0
     x_mad = x_mad + eps
 
     z = (x - x_median) / x_mad
@@ -242,17 +258,18 @@
     **Returns:**<br>
     `z`: torch.Tensor same shape as `x`, except scaled.
     """
     x_median = masked_median(x=x, mask=mask, dim=dim)
     x_mad = masked_median(x=torch.abs(x - x_median), mask=mask, dim=dim)
 
     # Protect x_mad=0 values
+    # Assuming normality and relationship between mad and std
     x_means = masked_mean(x=x, mask=mask, dim=dim)
     x_stds = torch.sqrt(masked_mean(x=(x - x_means) ** 2, mask=mask, dim=dim))
-    x_mad_aux = x_stds / 0.6744897501960817
+    x_mad_aux = x_stds * 0.6744897501960817
     x_mad = x_mad * (x_mad > 0) + x_mad_aux * (x_mad == 0)
 
     # Protect against division by zero
     x_mad[x_mad == 0] = 1.0
     x_mad = x_mad + eps
 
     z = torch.arcsinh((x - x_median) / x_mad)
```

### Comparing `neuralforecast-1.5.0/neuralforecast/core.py` & `neuralforecast-1.6.0/neuralforecast/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% auto 0
 __all__ = ['NeuralForecast']
 
 # %% ../nbs/core.ipynb 4
 import os
 import pickle
 import warnings
-
+from copy import deepcopy
 from os.path import isfile, join
 from typing import Any, List, Optional
 
 import numpy as np
 import pandas as pd
 
 from .tsdataset import TimeSeriesDataset
@@ -25,14 +25,15 @@
     NHITS,
     NBEATS,
     NBEATSx,
     TFT,
     VanillaTransformer,
     Informer,
     Autoformer,
+    FEDformer,
     StemGNN,
     PatchTST,
 )
 
 # %% ../nbs/core.ipynb 5
 def _cv_dates(last_dates, freq, h, test_size, step_size=1):
     # assuming step_size = 1
@@ -119,29 +120,34 @@
     "tcn": TCN,
     "dilatedrnn": DilatedRNN,
     "mlp": MLP,
     "nbeats": NBEATS,
     "nbeatsx": NBEATSx,
     "nhits": NHITS,
     "tft": TFT,
-    "stemgnn": StemGNN,
+    "vanillatransformer": VanillaTransformer,
     "informer": Informer,
+    "autoformer": Autoformer,
+    "patchtst": PatchTST,
+    "stemgnn": StemGNN,
     "autogru": GRU,
     "autolstm": LSTM,
     "autornn": RNN,
     "autotcn": TCN,
     "autodilatedrnn": DilatedRNN,
     "automlp": MLP,
     "autonbeats": NBEATS,
+    "autonbeatsx": NBEATSx,
     "autonhits": NHITS,
     "autotft": TFT,
     "autovanillatransformer": VanillaTransformer,
     "autoinformer": Informer,
     "autoautoformer": Autoformer,
     "autopatchtst": PatchTST,
+    "autofedformer": FEDformer,
     "autostemgnn": StemGNN,
 }
 
 # %% ../nbs/core.ipynb 12
 class NeuralForecast:
     def __init__(self, models: List[Any], freq: str):
         """
@@ -184,43 +190,52 @@
 
     def fit(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         val_size: Optional[int] = 0,
         sort_df: bool = True,
+        use_init_models: bool = True,
         verbose: bool = False,
     ):
         """Fit the core.NeuralForecast.
 
         Fit `models` to a large set of time series from DataFrame `df`.
         and store fitted models for later inspection.
 
         Parameters
         ----------
         df : pandas.DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
             If None, a previously stored dataset is required.
         static_df : pandas.DataFrame, optional (default=None)
-            DataFrame with columns [`unique_id`, `ds`] and static exogenous.
+            DataFrame with columns [`unique_id`] and static exogenous.
         val_size : int, optional (default=0)
             Size of validation set.
         sort_df : bool, optional (default=False)
             Sort `df` before fitting.
+        use_init_models : bool, optional (default=True)
+            Use initial model passed when NeuralForecast object was instantiated.
         verbose : bool (default=False)
             Print processing steps.
 
         Returns
         -------
         self : NeuralForecast
             Returns `NeuralForecast` class with fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
             raise Exception("You must pass a DataFrame or have one stored.")
 
+        # Model and datasets interactions protections
+        if (any(model.early_stop_patience_steps > 0 for model in self.models)) and (
+            val_size == 0
+        ):
+            raise Exception("Set val_size>0 if early stopping is enabled.")
+
         # Process and save new dataset (in self)
         if df is not None:
             self.dataset, self.uids, self.last_dates, self.ds = self._prepare_fit(
                 df=df, static_df=static_df, sort_df=sort_df
             )
             self.sort_df = sort_df
         else:
@@ -229,18 +244,20 @@
 
         if val_size is not None:
             if self.dataset.min_size < val_size:
                 warnings.warn(
                     "Validation set size is larger than the shorter time-series."
                 )
 
-        # train + validation
-        for model in self.models:
+        # Recover initial model if use_init_models or is the first time fitting
+        if (use_init_models) or (not self._fitted):
+            self.models_fitted = [deepcopy(model) for model in self.models]
+
+        for model in self.models_fitted:
             model.fit(self.dataset, val_size=val_size)
-        # train with the full dataset
 
         self._fitted = True
 
     def predict(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
@@ -255,15 +272,15 @@
 
         Parameters
         ----------
         df : pandas.DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
             If a DataFrame is passed, it is used to generate forecasts.
         static_df : pandas.DataFrame, optional (default=None)
-            DataFrame with columns [`unique_id`, `ds`] and static exogenous.
+            DataFrame with columns [`unique_id`] and static exogenous.
         futr_df : pandas.DataFrame, optional (default=None)
             DataFrame with [`unique_id`, `ds`] columns and `df`'s future exogenous.
         sort_df : bool (default=True)
             Sort `df` before fitting.
         verbose : bool (default=False)
             Print processing steps.
         data_kwargs : kwargs
@@ -274,29 +291,32 @@
         fcsts_df : pandas.DataFrame
             DataFrame with insample `models` columns for point predictions and probabilistic
             predictions for all fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
             raise Exception("You must pass a DataFrame or have one stored.")
 
+        if not self._fitted:
+            raise Exception("You must fit the model before predicting.")
+
         # Process new dataset but does not store it.
         if df is not None:
             dataset, uids, last_dates, _ = self._prepare_fit(
                 df=df, static_df=static_df, sort_df=sort_df
             )
         else:
             dataset = self.dataset
             uids = self.uids
             last_dates = self.last_dates
             if verbose:
                 print("Using stored dataset.")
 
         cols = []
         count_names = {"model": 0}
-        for model in self.models:
+        for model in self.models_fitted:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         # Placeholder dataframe for predictions with unique_id and ds
@@ -312,15 +332,15 @@
         else:
             dataset = TimeSeriesDataset.update_dataset(
                 dataset=dataset, future_df=fcsts_df.reset_index()
             )
 
         col_idx = 0
         fcsts = np.full((self.h * len(uids), len(cols)), fill_value=np.nan)
-        for model in self.models:
+        for model in self.models_fitted:
             old_test_size = model.get_test_size()
             model.set_test_size(self.h)  # To predict h steps ahead
             model_fcsts = model.predict(dataset=dataset, **data_kwargs)
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : col_idx + output_length] = model_fcsts
             col_idx += output_length
@@ -337,42 +357,42 @@
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         n_windows: int = 1,
         step_size: int = 1,
         val_size: Optional[int] = 0,
         test_size: Optional[int] = None,
         sort_df: bool = True,
-        fit_models: bool = True,
+        use_init_models: bool = True,
         verbose: bool = False,
         **data_kwargs,
     ):
         """Temporal Cross-Validation with core.NeuralForecast.
 
         `core.NeuralForecast`'s cross-validation efficiently fits a list of NeuralForecast
         models through multiple windows, in either chained or rolled manner.
 
         Parameters
         ----------
         df : pandas.DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
             If None, a previously stored dataset is required.
         static_df : pandas.DataFrame, optional (default=None)
-            DataFrame with columns [`unique_id`, `ds`] and static exogenous.
+            DataFrame with columns [`unique_id`] and static exogenous.
         n_windows : int (default=1)
             Number of windows used for cross validation.
         step_size : int (default=1)
             Step size between each window.
         val_size : int, optional (default=None)
             Length of validation size. If passed, set `n_windows=None`.
         test_size : int, optional (default=None)
             Length of test size. If passed, set `n_windows=None`.
         sort_df : bool (default=True)
             Sort `df` before fitting.
-        fit_models: bool (default=True)
-            Fit models before cross-validation.
+        use_init_models : bool, option (default=True)
+            Use initial model passed when object was instantiated.
         verbose : bool (default=False)
             Print processing steps.
         data_kwargs : kwargs
             Extra arguments to be passed to the dataset within each model.
 
         Returns
         -------
@@ -389,24 +409,28 @@
                 df=df, static_df=static_df, sort_df=sort_df
             )
             self.sort_df = sort_df
         else:
             if verbose:
                 print("Using stored dataset.")
 
+        # Recover initial model if use_init_models and not fitted. If already fitted, will use models_fitted
+        if (use_init_models) or (not self._fitted):
+            self.models_fitted = [deepcopy(model) for model in self.models]
+
         cols = []
         count_names = {"model": 0}
-        for model in self.models:
+        for model in self.models_fitted:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
-        h = self.models[0].h
+        h = self.models_fitted[0].h
         if test_size is None:
             test_size = h + step_size * (n_windows - 1)
         elif n_windows is None:
             if (test_size - h) % step_size:
                 raise Exception("`test_size - h` should be module `step_size`")
             n_windows = int((test_size - h) / step_size) + 1
         elif (n_windows is None) and (test_size is None):
@@ -430,32 +454,27 @@
         idx = pd.Index(np.repeat(self.uids, h * n_windows), name="unique_id")
         fcsts_df.index = idx
 
         col_idx = 0
         fcsts = np.full(
             (self.dataset.n_groups * h * n_windows, len(cols)), np.nan, dtype=np.float32
         )
-        for model in self.models:
-            # Fit
-            if fit_models:
-                model.fit(dataset=self.dataset, val_size=val_size, test_size=test_size)
-            else:
-                model.set_test_size(test_size=test_size)
 
-            # Predict
+        for model in self.models_fitted:
+            model.fit(dataset=self.dataset, val_size=val_size, test_size=test_size)
             model_fcsts = model.predict(
                 self.dataset, step_size=step_size, **data_kwargs
             )
 
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : (col_idx + output_length)] = model_fcsts
             col_idx += output_length
-        if fit_models:
-            self._fitted = True
+
+        self._fitted = True
 
         # Add predictions to forecasts DataFrame
         fcsts = pd.DataFrame.from_records(fcsts, columns=cols, index=fcsts_df.index)
         fcsts_df = pd.concat([fcsts_df, fcsts], axis=1)
 
         # Add original input df's y to forecasts DataFrame
         fcsts_df = fcsts_df.merge(df, how="left", on=["unique_id", "ds"])
@@ -491,23 +510,23 @@
                 print(
                     f"WARNING: Predict insample might not provide accurate predictions for \
                       recurrent model {repr(model)} class yet due to scaling."
                 )
 
         cols = []
         count_names = {"model": 0}
-        for model in self.models:
+        for model in self.models_fitted:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         # Remove test set from dataset and last dates
-        test_size = self.models[0].get_test_size()
+        test_size = self.models_fitted[0].get_test_size()
         if test_size > 0:
             trimmed_dataset = TimeSeriesDataset.trim_dataset(
                 dataset=self.dataset, right_trim=test_size, left_trim=0
             )
             last_dates_train = self.last_dates.shift(-test_size, freq=self.freq)
         else:
             trimmed_dataset = self.dataset
@@ -526,15 +545,15 @@
             step_size=step_size,
         )
         fcsts_df = fcsts_df.set_index("unique_id")
 
         col_idx = 0
         fcsts = np.full((len(fcsts_df), len(cols)), np.nan, dtype=np.float32)
 
-        for model in self.models:
+        for model in self.models_fitted:
             # Test size is the number of periods to forecast (full size of trimmed dataset)
             model.set_test_size(test_size=trimmed_dataset.max_size)
 
             # Predict
             model_fcsts = model.predict(trimmed_dataset, step_size=step_size)
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
@@ -550,71 +569,14 @@
         Y_df = pd.DataFrame.from_records(
             self.dataset.temporal[:, [0]].numpy(), columns=["y"], index=self.ds
         )
         Y_df = Y_df.reset_index(drop=False)
         fcsts_df = fcsts_df.merge(Y_df, how="left", on=["unique_id", "ds"])
         return fcsts_df
 
-    def predict_rolled(
-        self,
-        df: Optional[pd.DataFrame] = None,
-        static_df: Optional[pd.DataFrame] = None,
-        n_windows: int = 1,
-        step_size: int = 1,
-        insample_size: Optional[int] = None,
-        sort_df: bool = True,
-        verbose: bool = False,
-        **data_kwargs,
-    ):
-        """Predict insample with core.NeuralForecast.
-
-        Use stored fitted `models` to predict historic values of a time series from DataFrame `df`.
-
-        Parameters
-        ----------
-        df : pandas.DataFrame, optional (default=None)
-            DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
-            If None, a previously stored dataset is required.
-        static_df : pandas.DataFrame, optional (default=None)
-            DataFrame with columns [`unique_id`, `ds`] and static exogenous.
-        n_windows : int (default=1)
-            Number of windows used for cross validation.
-        step_size : int (default=1)
-            Step size between each window.
-        insample_size : int, optional (default=None)
-            Length of insample size to produce forecasts. If passed, set `n_windows=None`.
-        sort_df : bool (default=True)
-            Sort `df` before fitting.
-        verbose : bool (default=False)
-            Print processing steps.
-        data_kwargs : kwargs
-            Extra arguments to be passed to the dataset within each model.
-
-        Returns
-        -------
-        fcsts_df : pandas.DataFrame
-            DataFrame with insample `models` columns for point predictions and probabilistic
-            predictions for all fitted `models`.
-        """
-        print(
-            "WARNING: this method will be deprecated. Use `cross_validation` or `predict_insample` instead."
-        )
-        fcsts_df = self.cross_validation(
-            df=df,
-            static_df=static_df,
-            n_windows=n_windows,
-            step_size=step_size,
-            val_size=0,
-            test_size=insample_size,
-            sort_df=sort_df,
-            fit_models=False,
-            verbose=verbose,
-        )
-        return fcsts_df
-
     # Save list of models with pytorch lightning save_checkpoint function
     def save(
         self,
         path: str,
         model_index: Optional[List] = None,
         save_dataset: bool = True,
         overwrite: bool = False,
@@ -638,15 +600,15 @@
         """
         # Standarize path without '/'
         if path[-1] == "/":
             path = path[:-1]
 
         # Model index list
         if model_index is None:
-            model_index = list(range(len(self.models)))
+            model_index = list(range(len(self.models_fitted)))
 
         # Create directory if not exists
         os.makedirs(path, exist_ok=True)
 
         # Check if directory is empty to protect overwriting files
         dir = os.listdir(path)
 
@@ -654,15 +616,15 @@
         if (len(dir) > 0) and (not overwrite):
             raise Exception(
                 "Directory is not empty. Set `overwrite=True` to overwrite files."
             )
 
         # Save models
         count_names = {"model": 0}
-        for i, model in enumerate(self.models):
+        for i, model in enumerate(self.models_fitted):
             # Skip model if not in list
             if i not in model_index:
                 continue
 
             model_name = repr(model).lower().replace("_", "")
             count_names[model_name] = count_names.get(model_name, -1) + 1
             model.save(f"{path}/{model_name}_{count_names[model_name]}.ckpt")
@@ -756,11 +718,15 @@
         if dataset is not None:
             neuralforecast.dataset = dataset
             neuralforecast.uids = config_dict["uids"]
             neuralforecast.last_dates = config_dict["last_dates"]
             neuralforecast.ds = config_dict["ds"]
             neuralforecast.sort_df = config_dict["sort_df"]
 
-        # Fitted flag
+        # Fitted flag and models_fitted
         neuralforecast._fitted = config_dict["_fitted"]
+        if config_dict["_fitted"]:
+            neuralforecast.models_fitted = [
+                deepcopy(model) for model in neuralforecast.models
+            ]
 
         return neuralforecast
```

### Comparing `neuralforecast-1.5.0/neuralforecast/losses/numpy.py` & `neuralforecast-1.6.0/neuralforecast/losses/numpy.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/losses/pytorch.py` & `neuralforecast-1.6.0/neuralforecast/losses/pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/losses.pytorch.ipynb.
 
 # %% auto 0
-__all__ = ['MAE', 'MSE', 'RMSE', 'MAPE', 'SMAPE', 'MASE', 'QuantileLoss', 'Accuracy', 'MQLoss', 'wMQLoss', 'sCRPS', 'relMSE',
-           'DistributionLoss', 'PMM', 'GMM', 'NBMM']
+__all__ = ['MAE', 'MSE', 'RMSE', 'MAPE', 'SMAPE', 'MASE', 'relMSE', 'QuantileLoss', 'MQLoss', 'wMQLoss', 'DistributionLoss',
+           'PMM', 'GMM', 'NBMM', 'HuberLoss', 'TukeyLoss', 'HuberQLoss', 'HuberMQLoss', 'Accuracy', 'sCRPS']
 
 # %% ../../nbs/losses.pytorch.ipynb 3
 from typing import Optional, Union, Tuple
 
 import math
 import numpy as np
 import torch
@@ -189,14 +189,17 @@
     accuracy of a forecasting method by calculating the percentual deviation
     of the prediction and the observed value at a given time and
     averages these devations over the length of the series.
     The closer to zero an observed value is, the higher penalty MAPE loss
     assigns to the corresponding error.
 
     $$ \mathrm{MAPE}(\\mathbf{y}_{\\tau}, \\mathbf{\hat{y}}_{\\tau}) = \\frac{1}{H} \\sum^{t+H}_{\\tau=t+1} \\frac{|y_{\\tau}-\hat{y}_{\\tau}|}{|y_{\\tau}|} $$
+
+    **References:**<br>
+    [Makridakis S., "Accuracy measures: theoretical and practical concerns".](https://www.sciencedirect.com/science/article/pii/0169207093900793)
     """
 
     def __init__(self):
         super(MAPE, self).__init__()
         self.outputsize_multiplier = 1
         self.output_names = [""]
         self.is_distribution_output = False
@@ -352,15 +355,66 @@
             axis=1,
         )
         mase = _divide_no_nan(delta_y, scale[:, None])
         mase = mase * mask
         mase = torch.mean(mase)
         return mase
 
-# %% ../../nbs/losses.pytorch.ipynb 40
+# %% ../../nbs/losses.pytorch.ipynb 39
+class relMSE(torch.nn.Module):
+    """Relative Mean Squared Error
+    Computes Relative Mean Squared Error (relMSE), as proposed by Hyndman & Koehler (2006)
+    as an alternative to percentage errors, to avoid measure unstability.
+    $$ \mathrm{relMSE}(\\mathbf{y}, \\mathbf{\hat{y}}, \\mathbf{\hat{y}}^{naive1}) =
+    \\frac{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}})}{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}}^{naive1})} $$
+    **Parameters:**<br>
+    `y_train`: numpy array, Training values.<br>
+    **References:**<br>
+    - [Hyndman, R. J and Koehler, A. B. (2006).
+       "Another look at measures of forecast accuracy",
+       International Journal of Forecasting, Volume 22, Issue 4.](https://www.sciencedirect.com/science/article/pii/S0169207006000239)<br>
+    - [Kin G. Olivares, O. Nganba Meetei, Ruijun Ma, Rohan Reddy, Mengfei Cao, Lee Dicker.
+       "Probabilistic Hierarchical Forecasting with Deep Poisson Mixtures.
+       Submitted to the International Journal Forecasting, Working paper available at arxiv.](https://arxiv.org/pdf/2110.13179.pdf)
+    """
+
+    def __init__(self, y_train):
+        super(relMSE, self).__init__()
+        self.y_train = y_train
+        self.mse = MSE()
+        self.is_distribution_output = False
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
+
+        **Returns:**<br>
+        `relmse`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y)
+        n_series, horizon = y.shape
+
+        last_col = self.y_train[:, -1].unsqueeze(1)
+        y_naive = last_col.repeat(1, horizon)
+
+        norm = self.mse(y=y, y_hat=y_naive)
+        loss = self.mse(y=y, y_hat=y_hat, mask=mask)
+        loss = loss / (norm + 1e-5)
+        return loss
+
+# %% ../../nbs/losses.pytorch.ipynb 44
 class QuantileLoss(torch.nn.Module):
     """Quantile Loss
 
     Computes the quantile loss between `y` and `y_hat`.
     QL measures the deviation of a quantile forecast.
     By weighting the absolute deviation in a non symmetric way, the
     loss pays more attention to under or over estimation.
@@ -409,61 +463,14 @@
 
         delta_y = y - y_hat
         loss = torch.max(torch.mul(self.q, delta_y), torch.mul((self.q - 1), delta_y))
         loss = loss * mask
         quantile_loss = torch.mean(loss)
         return quantile_loss
 
-# %% ../../nbs/losses.pytorch.ipynb 45
-class Accuracy(torch.nn.Module):
-    """Accuracy
-
-    Computes the accuracy between categorical `y` and `y_hat`.
-    This evaluation metric is only meant for evalution, as it
-    is not differentiable.
-
-    $$ \mathrm{Accuracy}(\\mathbf{y}_{\\tau}, \\mathbf{\hat{y}}_{\\tau}) = \\frac{1}{H} \\sum^{t+H}_{\\tau=t+1} \mathrm{1}\{\\mathbf{y}_{\\tau}==\\mathbf{\hat{y}}_{\\tau}\} $$
-
-    """
-
-    def __init__(
-        self,
-    ):
-        super(Accuracy, self).__init__()
-        self.is_distribution_output = False
-
-    def domain_map(self, y_hat: torch.Tensor):
-        """
-        Univariate loss operates in dimension [B,T,H]/[B,H]
-        This changes the network's output from [B,H,1]->[B,H]
-        """
-        return y_hat.squeeze(-1)
-
-    def __call__(
-        self,
-        y: torch.Tensor,
-        y_hat: torch.Tensor,
-        mask: Union[torch.Tensor, None] = None,
-    ):
-        """
-        **Parameters:**<br>
-        `y`: tensor, Actual values.<br>
-        `y_hat`: tensor, Predicted values.<br>
-        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
-
-        **Returns:**<br>
-        `accuracy`: tensor (single value).
-        """
-        if mask is None:
-            mask = torch.ones_like(y_hat)
-
-        measure = (y.unsqueeze(-1) == y_hat) * mask.unsqueeze(-1)
-        accuracy = torch.mean(measure)
-        return accuracy
-
 # %% ../../nbs/losses.pytorch.ipynb 49
 def level_to_outputs(level):
     qs = sum([[50 - l / 2, 50 + l / 2] for l in level], [])
     output_names = sum([[f"-lo-{l}", f"-hi-{l}"] for l in level], [])
 
     sort_idx = np.argsort(qs)
     quantiles = np.array(qs)[sort_idx]
@@ -637,124 +644,15 @@
         mask = mask.unsqueeze(-1)
         wmqloss = _divide_no_nan(
             torch.sum(loss * mask, axis=-2),
             torch.sum(torch.abs(y.unsqueeze(-1)) * mask, axis=-2),
         )
         return torch.mean(wmqloss)
 
-# %% ../../nbs/losses.pytorch.ipynb 59
-class sCRPS(torch.nn.Module):
-    """Scaled Continues Ranked Probability Score
-
-    Calculates a scaled variation of the CRPS, as proposed by Rangapuram (2021),
-    to measure the accuracy of predicted quantiles `y_hat` compared to the observation `y`.
-
-    This metric averages percentual weighted absolute deviations as
-    defined by the quantile losses.
-
-    $$ \mathrm{sCRPS}(\\mathbf{\hat{y}}^{(q)}_{\\tau}, \mathbf{y}_{\\tau}) = \\frac{2}{N} \sum_{i}
-    \int^{1}_{0}
-    \\frac{\mathrm{QL}(\\mathbf{\hat{y}}^{(q}_{\\tau} y_{i,\\tau})_{q}}{\sum_{i} | y_{i,\\tau} |} dq $$
-
-    where $\\mathbf{\hat{y}}^{(q}_{\\tau}$ is the estimated quantile, and $y_{i,\\tau}$
-    are the target variable realizations.
-
-    **Parameters:**<br>
-    `level`: int list [0,100]. Probability levels for prediction intervals (Defaults median).
-    `quantiles`: float list [0., 1.]. Alternative to level, quantiles to estimate from y distribution.
-
-    **References:**<br>
-    - [Gneiting, Tilmann. (2011). \"Quantiles as optimal point forecasts\".
-    International Journal of Forecasting.](https://www.sciencedirect.com/science/article/pii/S0169207010000063)<br>
-    - [Spyros Makridakis, Evangelos Spiliotis, Vassilios Assimakopoulos, Zhi Chen, Anil Gaba, Ilia Tsetlin, Robert L. Winkler. (2022).
-    \"The M5 uncertainty competition: Results, findings and conclusions\".
-    International Journal of Forecasting.](https://www.sciencedirect.com/science/article/pii/S0169207021001722)<br>
-    - [Syama Sundar Rangapuram, Lucien D Werner, Konstantinos Benidis, Pedro Mercado, Jan Gasthaus, Tim Januschowski. (2021).
-    \"End-to-End Learning of Coherent Probabilistic Forecasts for Hierarchical Time Series\".
-    Proceedings of the 38th International Conference on Machine Learning (ICML).](https://proceedings.mlr.press/v139/rangapuram21a.html)
-    """
-
-    def __init__(self, level=[80, 90], quantiles=None):
-        super(sCRPS, self).__init__()
-        self.mql = MQLoss(level=level, quantiles=quantiles)
-        self.is_distribution_output = False
-
-    def __call__(
-        self,
-        y: torch.Tensor,
-        y_hat: torch.Tensor,
-        mask: Union[torch.Tensor, None] = None,
-    ):
-        """
-        **Parameters:**<br>
-        `y`: tensor, Actual values.<br>
-        `y_hat`: tensor, Predicted values.<br>
-        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
-
-        **Returns:**<br>
-        `scrps`: tensor (single value).
-        """
-        mql = self.mql(y=y, y_hat=y_hat, mask=mask)
-        norm = torch.sum(torch.abs(y))
-        unmean = torch.sum(mask)
-        scrps = 2 * mql * unmean / (norm + 1e-5)
-        return scrps
-
-# %% ../../nbs/losses.pytorch.ipynb 62
-class relMSE(torch.nn.Module):
-    """Relative Mean Squared Error
-    Computes Relative Mean Squared Error (relMSE), as proposed by Hyndman & Koehler (2006)
-    as an alternative to percentage errors, to avoid measure unstability.
-    $$ \mathrm{relMSE}(\\mathbf{y}, \\mathbf{\hat{y}}, \\mathbf{\hat{y}}^{naive1}) =
-    \\frac{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}})}{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}}^{naive1})} $$
-    **Parameters:**<br>
-    `y_train`: numpy array, Training values.<br>
-    **References:**<br>
-    - [Hyndman, R. J and Koehler, A. B. (2006).
-       "Another look at measures of forecast accuracy",
-       International Journal of Forecasting, Volume 22, Issue 4.](https://www.sciencedirect.com/science/article/pii/S0169207006000239)<br>
-    - [Kin G. Olivares, O. Nganba Meetei, Ruijun Ma, Rohan Reddy, Mengfei Cao, Lee Dicker.
-       "Probabilistic Hierarchical Forecasting with Deep Poisson Mixtures.
-       Submitted to the International Journal Forecasting, Working paper available at arxiv.](https://arxiv.org/pdf/2110.13179.pdf)
-    """
-
-    def __init__(self, y_train):
-        super(relMSE, self).__init__()
-        self.y_train = y_train
-        self.mse = MSE()
-        self.is_distribution_output = False
-
-    def __call__(
-        self,
-        y: torch.Tensor,
-        y_hat: torch.Tensor,
-        mask: Union[torch.Tensor, None] = None,
-    ):
-        """
-        **Parameters:**<br>
-        `y`: tensor, Actual values.<br>
-        `y_hat`: tensor, Predicted values.<br>
-        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
-
-        **Returns:**<br>
-        `relmse`: tensor (single value).
-        """
-        if mask is None:
-            mask = torch.ones_like(y)
-        n_series, horizon = y.shape
-
-        last_col = self.y_train[:, -1].unsqueeze(1)
-        y_naive = last_col.repeat(1, horizon)
-
-        norm = self.mse(y=y, y_hat=y_naive)
-        loss = self.mse(y=y, y_hat=y_hat, mask=mask)
-        loss = loss / (norm + 1e-5)
-        return loss
-
-# %% ../../nbs/losses.pytorch.ipynb 66
+# %% ../../nbs/losses.pytorch.ipynb 60
 def weighted_average(
     x: torch.Tensor, weights: Optional[torch.Tensor] = None, dim=None
 ) -> torch.Tensor:
     """
     Computes the weighted average of a given tensor across a given dim, masking
     values associated with weight zero,
     meaning instead of `nan * 0 = nan` you will get `0 * 0 = 0`.
@@ -774,15 +672,15 @@
         )
         return (
             weighted_tensor.sum(dim=dim) if dim else weighted_tensor.sum()
         ) / sum_weights
     else:
         return x.mean(dim=dim)
 
-# %% ../../nbs/losses.pytorch.ipynb 67
+# %% ../../nbs/losses.pytorch.ipynb 61
 def bernoulli_domain_map(input: torch.Tensor):
     """Bernoulli Domain Map
     Maps input into distribution constraints, by construction input's
     last dimension is of matching `distr_args` length.
 
     **Parameters:**<br>
     `input`: tensor, of dimensions [B,T,H,theta] or [B,H,theta].<br>
@@ -931,15 +829,15 @@
     # mu = total_count * (probs/(1-probs))
     # => probs = mu / (total_count + mu)
     # => probs = mu / [total_count * (1 + mu * (1/total_count))]
     total_count = 1.0 / alpha
     probs = (mu * alpha / (1.0 + mu * alpha)) + 1e-8
     return (total_count, probs)
 
-# %% ../../nbs/losses.pytorch.ipynb 68
+# %% ../../nbs/losses.pytorch.ipynb 62
 def est_lambda(mu, rho):
     return mu ** (2 - rho) / (2 - rho)
 
 
 def est_alpha(rho):
     return (2 - rho) / (rho - 1)
 
@@ -1052,33 +950,34 @@
     Also adds Tweedie domain protection to the distribution parameters.
     """
     log_mu = output[0]
     if (loc is not None) and (scale is not None):
         log_mu += torch.log(loc)  # TODO : rho scaling
     return (log_mu,)
 
-# %% ../../nbs/losses.pytorch.ipynb 69
+# %% ../../nbs/losses.pytorch.ipynb 63
 class DistributionLoss(torch.nn.Module):
     """DistributionLoss
 
     This PyTorch module wraps the `torch.distribution` classes allowing it to
     interact with NeuralForecast models modularly. It shares the negative
     log-likelihood as the optimization objective and a sample method to
     generate empirically the quantiles defined by the `level` list.
 
     Additionally, it implements a distribution transformation that factorizes the
     scale-dependent likelihood parameters into a base scale and a multiplier
     efficiently learnable within the network's non-linearities operating ranges.
 
-    Available distributions:
-    - Poisson
-    - Normal
-    - StudentT
-    - NegativeBinomial
-    - Tweedie
+    Available distributions:<br>
+    - Poisson<br>
+    - Normal<br>
+    - StudentT<br>
+    - NegativeBinomial<br>
+    - Tweedie<br>
+    - Bernoulli (Temporal Classifiers)
 
     **Parameters:**<br>
     `distribution`: str, identifier of a torch.distributions.Distribution class.<br>
     `level`: float list [0,100], confidence levels for prediction intervals.<br>
     `quantiles`: float list [0,1], alternative to level list, target quantiles.<br>
     `num_samples`: int=500, number of samples for the empirical quantiles.<br>
     `return_params`: bool=False, wether or not return the Distribution parameters.<br><br>
@@ -1255,15 +1154,15 @@
         """
         # Instantiate Scaled Decoupled Distribution
         distr = self.get_distribution(distr_args=distr_args, **self.distribution_kwargs)
         loss_values = -distr.log_prob(y)
         loss_weights = mask
         return weighted_average(loss_values, weights=loss_weights)
 
-# %% ../../nbs/losses.pytorch.ipynb 75
+# %% ../../nbs/losses.pytorch.ipynb 69
 class PMM(torch.nn.Module):
     """Poisson Mixture Mesh
 
     This Poisson Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1453,15 +1352,15 @@
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
 
-# %% ../../nbs/losses.pytorch.ipynb 83
+# %% ../../nbs/losses.pytorch.ipynb 77
 class GMM(torch.nn.Module):
     """Gaussian Mixture Mesh
 
     This Gaussian Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1659,15 +1558,15 @@
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
 
-# %% ../../nbs/losses.pytorch.ipynb 91
+# %% ../../nbs/losses.pytorch.ipynb 85
 class NBMM(torch.nn.Module):
     """Negative Binomial Mixture Mesh
 
     This N. Binomial Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1871,7 +1770,420 @@
     def __call__(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
+
+# %% ../../nbs/losses.pytorch.ipynb 92
+class HuberLoss(torch.nn.Module):
+    """Huber Loss
+
+    The Huber loss, employed in robust regression, is a loss function that
+    exhibits reduced sensitivity to outliers in data when compared to the
+    squared error loss. This function is also refered as SmoothL1.
+
+    The Huber loss function is quadratic for small errors and linear for large
+    errors, with equal values and slopes of the different sections at the two
+    points where $(y_{\\tau}-\hat{y}_{\\tau})^{2}$=$|y_{\\tau}-\hat{y}_{\\tau}|$.
+
+    $$ L_{\delta}(y_{\\tau},\; \hat{y}_{\\tau})
+    =\\begin{cases}{\\frac{1}{2}}(y_{\\tau}-\hat{y}_{\\tau})^{2}\;{\\text{for }}|y_{\\tau}-\hat{y}_{\\tau}|\leq \delta \\\
+    \\delta \ \cdot \left(|y_{\\tau}-\hat{y}_{\\tau}|-{\\frac {1}{2}}\delta \\right),\;{\\text{otherwise.}}\end{cases}$$
+
+    where $\\delta$ is a threshold parameter that determines the point at which the loss transitions from quadratic to linear,
+    and can be tuned to control the trade-off between robustness and accuracy in the predictions.
+
+    **Parameters:**<br>
+    `delta`: float=1.0, Specifies the threshold at which to change between delta-scaled L1 and L2 loss.
+
+    **References:**<br>
+    [Huber Peter, J (1964). "Robust Estimation of a Location Parameter". Annals of Statistics](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-35/issue-1/Robust-Estimation-of-a-Location-Parameter/10.1214/aoms/1177703732.full)
+    """
+
+    def __init__(self, delta: float = 1.0):
+        super(HuberLoss, self).__init__()
+        self.outputsize_multiplier = 1
+        self.delta = delta
+        self.output_names = [""]
+        self.is_distribution_output = False
+
+    def domain_map(self, y_hat: torch.Tensor):
+        """
+        Univariate loss operates in dimension [B,T,H]/[B,H]
+        This changes the network's output from [B,H,1]->[B,H]
+        """
+        return y_hat.squeeze(-1)
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+
+        **Returns:**<br>
+        `huber_loss`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y_hat)
+
+        huber_loss = F.huber_loss(
+            y * mask, y_hat * mask, reduction="mean", delta=self.delta
+        )
+        return huber_loss
+
+# %% ../../nbs/losses.pytorch.ipynb 97
+class TukeyLoss(torch.nn.Module):
+    """Tukey Loss
+
+    The Tukey loss function, also known as Tukey's biweight function, is a
+    robust statistical loss function used in robust statistics. Tukey's loss exhibits
+    quadratic behavior near the origin, like the Huber loss; however, it is even more
+    robust to outliers as the loss for large residuals remains constant instead of
+    scaling linearly.
+
+    The parameter $c$ in Tukey's loss determines the ''saturation'' point
+    of the function: Higher values of $c$ enhance sensitivity, while lower values
+    increase resistance to outliers.
+
+    $$ L_{c}(y_{\\tau},\; \hat{y}_{\\tau})
+    =\\begin{cases}{
+    \\frac{c^{2}}{6}} \\left[1-(\\frac{y_{\\tau}-\hat{y}_{\\tau}}{c})^{2} \\right]^{3}    \;\\text{for } |y_{\\tau}-\hat{y}_{\\tau}|\leq c \\\
+    \\frac{c^{2}}{6} \qquad \\text{otherwise.}  \end{cases}$$
+
+    Please note that the Tukey loss function assumes the data to be stationary or
+    normalized beforehand. If the error values are excessively large, the algorithm
+    may need help to converge during optimization. It is advisable to employ small learning rates.
+
+    **Parameters:**<br>
+    `c`: float=4.685, Specifies the Tukey loss' threshold on which residuals are no longer considered.<br>
+    `normalize`: bool=True, Wether normalization is performed within Tukey loss' computation.<br>
+
+    **References:**<br>
+    [Beaton, A. E., and Tukey, J. W. (1974). "The Fitting of Power Series, Meaning Polynomials, Illustrated on Band-Spectroscopic Data."](https://www.jstor.org/stable/1267936)
+    """
+
+    def __init__(self, c: float = 4.685, normalize: bool = True):
+        super(TukeyLoss, self).__init__()
+        self.outputsize_multiplier = 1
+        self.c = c
+        self.normalize = normalize
+        self.output_names = [""]
+        self.is_distribution_output = False
+
+    def domain_map(self, y_hat: torch.Tensor):
+        """
+        Univariate loss operates in dimension [B,T,H]/[B,H]
+        This changes the network's output from [B,H,1]->[B,H]
+        """
+        return y_hat.squeeze(-1)
+
+    def masked_mean(self, x, mask, dim):
+        x_nan = x.masked_fill(mask < 1, float("nan"))
+        x_mean = x_nan.nanmean(dim=dim, keepdim=True)
+        x_mean = torch.nan_to_num(x_mean, nan=0.0)
+        return x_mean
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+
+        **Returns:**<br>
+        `tukey_loss`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y_hat)
+
+        # We normalize the Tukey loss, to satisfy 4.685 normal outlier bounds
+        if self.normalize:
+            y_mean = self.masked_mean(x=y, mask=mask, dim=-1)
+            y_std = (
+                torch.sqrt(self.masked_mean(x=(y - y_mean) ** 2, mask=mask, dim=-1))
+                + 1e-2
+            )
+        else:
+            y_std = 1.0
+        delta_y = torch.abs(y - y_hat) / y_std
+
+        tukey_mask = torch.greater_equal(self.c * torch.ones_like(delta_y), delta_y)
+        tukey_loss = tukey_mask * mask * (1 - (delta_y / (self.c)) ** 2) ** 3 + (
+            1 - (tukey_mask * 1)
+        )
+        tukey_loss = (self.c**2 / 6) * torch.mean(tukey_loss)
+        return tukey_loss
+
+# %% ../../nbs/losses.pytorch.ipynb 102
+class HuberQLoss(torch.nn.Module):
+    """Huberized Quantile Loss
+
+    The Huberized quantile loss is a modified version of the quantile loss function that
+    combines the advantages of the quantile loss and the Huber loss. It is commonly used
+    in regression tasks, especially when dealing with data that contains outliers or heavy tails.
+
+    The Huberized quantile loss between `y` and `y_hat` measure the Huber Loss in a non-symmetric way.
+    The loss pays more attention to under/over-estimation depending on the quantile parameter $q$;
+    and controls the trade-off between robustness and accuracy in the predictions with the parameter $delta$.
+
+    $$ \mathrm{HuberQL}(\\mathbf{y}_{\\tau}, \\mathbf{\hat{y}}^{(q)}_{\\tau}) =
+    (1-q)\, L_{\delta}(y_{\\tau},\; \hat{y}^{(q)}_{\\tau}) \mathbb{1}\{ \hat{y}^{(q)}_{\\tau} \geq y_{\\tau} \} +
+    q\, L_{\delta}(y_{\\tau},\; \hat{y}^{(q)}_{\\tau}) \mathbb{1}\{ \hat{y}^{(q)}_{\\tau} < y_{\\tau} \} $$
+
+    **Parameters:**<br>
+    `delta`: float=1.0, Specifies the threshold at which to change between delta-scaled L1 and L2 loss.<br>
+    `q`: float, between 0 and 1. The slope of the quantile loss, in the context of quantile regression, the q determines the conditional quantile level.<br>
+
+    **References:**<br>
+    [Huber Peter, J (1964). "Robust Estimation of a Location Parameter". Annals of Statistics](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-35/issue-1/Robust-Estimation-of-a-Location-Parameter/10.1214/aoms/1177703732.full)<br>
+    [Roger Koenker and Gilbert Bassett, Jr., "Regression Quantiles".](https://www.jstor.org/stable/1913643)
+    """
+
+    def __init__(self, q: float, delta: float = 1.0):
+        super(HuberQLoss, self).__init__()
+        self.q = q
+        self.delta = delta
+        self.outputsize_multiplier = 1
+        self.output_names = [f"_q{q}_d{delta}"]
+        self.is_distribution_output = False
+
+    def domain_map(self, y_hat: torch.Tensor):
+        """
+        Univariate loss operates in dimension [B,T,H]/[B,H]
+        This changes the network's output from [B,H,1]->[B,H]
+        """
+        return y_hat.squeeze(-1)
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+
+        **Returns:**<br>
+        `huber_qloss`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y_hat)
+
+        error = y_hat - y
+        zero_error = torch.zeros_like(error)
+        sq = torch.maximum(-error, zero_error)
+        s1_q = torch.maximum(error, zero_error)
+        hqloss = self.q * F.huber_loss(
+            sq * mask, zero_error * mask, reduction="mean", delta=self.delta
+        ) + (1 - self.q) * F.huber_loss(
+            s1_q * mask, zero_error * mask, reduction="mean", delta=self.delta
+        )
+        return hqloss
+
+# %% ../../nbs/losses.pytorch.ipynb 107
+class HuberMQLoss(torch.nn.Module):
+    """Huberized Multi-Quantile loss
+
+    The Huberized Multi-Quantile loss (HuberMQL) is a modified version of the multi-quantile loss function
+    that combines the advantages of the quantile loss and the Huber loss. HuberMQL is commonly used in regression
+    tasks, especially when dealing with data that contains outliers or heavy tails. The loss function pays
+    more attention to under/over-estimation depending on the quantile list $[q_{1},q_{2},\dots]$ parameter.
+    It controls the trade-off between robustness and prediction accuracy with the parameter $\\delta$.
+
+    $$ \mathrm{HuberMQL}_{\delta}(\\mathbf{y}_{\\tau},[\\mathbf{\hat{y}}^{(q_{1})}_{\\tau}, ... ,\hat{y}^{(q_{n})}_{\\tau}]) =
+    \\frac{1}{n} \\sum_{q_{i}} \mathrm{HuberQL}_{\\delta}(\\mathbf{y}_{\\tau}, \\mathbf{\hat{y}}^{(q_{i})}_{\\tau}) $$
+
+    **Parameters:**<br>
+    `level`: int list [0,100]. Probability levels for prediction intervals (Defaults median).
+    `quantiles`: float list [0., 1.]. Alternative to level, quantiles to estimate from y distribution.
+    `delta`: float=1.0, Specifies the threshold at which to change between delta-scaled L1 and L2 loss.<br>
+
+    **References:**<br>
+    [Huber Peter, J (1964). "Robust Estimation of a Location Parameter". Annals of Statistics](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-35/issue-1/Robust-Estimation-of-a-Location-Parameter/10.1214/aoms/1177703732.full)<br>
+    [Roger Koenker and Gilbert Bassett, Jr., "Regression Quantiles".](https://www.jstor.org/stable/1913643)
+    """
+
+    def __init__(self, level=[80, 90], quantiles=None, delta: float = 1.0):
+        super(HuberMQLoss, self).__init__()
+        # Transform level to MQLoss parameters
+        qs, self.output_names = level_to_outputs(level)
+        qs = torch.Tensor(qs)
+
+        # Transform quantiles to homogeneus output names
+        if quantiles is not None:
+            _, self.output_names = quantiles_to_outputs(quantiles)
+            qs = torch.Tensor(quantiles)
+
+        self.delta = delta
+        self.quantiles = torch.nn.Parameter(qs, requires_grad=False)
+        self.outputsize_multiplier = len(self.quantiles)
+        self.is_distribution_output = False
+
+    def domain_map(self, y_hat: torch.Tensor):
+        """
+        Identity domain map [B,T,H,Q]/[B,H,Q]
+        """
+        return y_hat
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+
+        **Returns:**<br>
+        `mqloss`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y_hat)
+
+        n_q = len(self.quantiles)
+
+        mask = mask.unsqueeze(-1)
+        error = y_hat - y.unsqueeze(-1)
+        zero_error = torch.zeros_like(error)
+        sq = torch.maximum(-error, torch.zeros_like(error))
+        s1_q = torch.maximum(error, torch.zeros_like(error))
+        hmqloss = F.huber_loss(
+            self.quantiles * sq * mask,
+            zero_error * mask,
+            reduction="mean",
+            delta=self.delta,
+        ) + F.huber_loss(
+            (1 - self.quantiles) * s1_q * mask,
+            zero_error * mask,
+            reduction="mean",
+            delta=self.delta,
+        )
+
+        # Match y/weights dimensions and compute weighted average
+        mask = mask / torch.sum(mask)
+
+        hmqloss = (1 / n_q) * hmqloss * mask
+        return torch.sum(hmqloss)
+
+# %% ../../nbs/losses.pytorch.ipynb 113
+class Accuracy(torch.nn.Module):
+    """Accuracy
+
+    Computes the accuracy between categorical `y` and `y_hat`.
+    This evaluation metric is only meant for evalution, as it
+    is not differentiable.
+
+    $$ \mathrm{Accuracy}(\\mathbf{y}_{\\tau}, \\mathbf{\hat{y}}_{\\tau}) = \\frac{1}{H} \\sum^{t+H}_{\\tau=t+1} \mathrm{1}\{\\mathbf{y}_{\\tau}==\\mathbf{\hat{y}}_{\\tau}\} $$
+
+    """
+
+    def __init__(
+        self,
+    ):
+        super(Accuracy, self).__init__()
+        self.is_distribution_output = False
+
+    def domain_map(self, y_hat: torch.Tensor):
+        """
+        Univariate loss operates in dimension [B,T,H]/[B,H]
+        This changes the network's output from [B,H,1]->[B,H]
+        """
+        return y_hat.squeeze(-1)
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+
+        **Returns:**<br>
+        `accuracy`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y_hat)
+
+        measure = (y.unsqueeze(-1) == y_hat) * mask.unsqueeze(-1)
+        accuracy = torch.mean(measure)
+        return accuracy
+
+# %% ../../nbs/losses.pytorch.ipynb 117
+class sCRPS(torch.nn.Module):
+    """Scaled Continues Ranked Probability Score
+
+    Calculates a scaled variation of the CRPS, as proposed by Rangapuram (2021),
+    to measure the accuracy of predicted quantiles `y_hat` compared to the observation `y`.
+
+    This metric averages percentual weighted absolute deviations as
+    defined by the quantile losses.
+
+    $$ \mathrm{sCRPS}(\\mathbf{\hat{y}}^{(q)}_{\\tau}, \mathbf{y}_{\\tau}) = \\frac{2}{N} \sum_{i}
+    \int^{1}_{0}
+    \\frac{\mathrm{QL}(\\mathbf{\hat{y}}^{(q}_{\\tau} y_{i,\\tau})_{q}}{\sum_{i} | y_{i,\\tau} |} dq $$
+
+    where $\\mathbf{\hat{y}}^{(q}_{\\tau}$ is the estimated quantile, and $y_{i,\\tau}$
+    are the target variable realizations.
+
+    **Parameters:**<br>
+    `level`: int list [0,100]. Probability levels for prediction intervals (Defaults median).
+    `quantiles`: float list [0., 1.]. Alternative to level, quantiles to estimate from y distribution.
+
+    **References:**<br>
+    - [Gneiting, Tilmann. (2011). \"Quantiles as optimal point forecasts\".
+    International Journal of Forecasting.](https://www.sciencedirect.com/science/article/pii/S0169207010000063)<br>
+    - [Spyros Makridakis, Evangelos Spiliotis, Vassilios Assimakopoulos, Zhi Chen, Anil Gaba, Ilia Tsetlin, Robert L. Winkler. (2022).
+    \"The M5 uncertainty competition: Results, findings and conclusions\".
+    International Journal of Forecasting.](https://www.sciencedirect.com/science/article/pii/S0169207021001722)<br>
+    - [Syama Sundar Rangapuram, Lucien D Werner, Konstantinos Benidis, Pedro Mercado, Jan Gasthaus, Tim Januschowski. (2021).
+    \"End-to-End Learning of Coherent Probabilistic Forecasts for Hierarchical Time Series\".
+    Proceedings of the 38th International Conference on Machine Learning (ICML).](https://proceedings.mlr.press/v139/rangapuram21a.html)
+    """
+
+    def __init__(self, level=[80, 90], quantiles=None):
+        super(sCRPS, self).__init__()
+        self.mql = MQLoss(level=level, quantiles=quantiles)
+        self.is_distribution_output = False
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
+
+        **Returns:**<br>
+        `scrps`: tensor (single value).
+        """
+        mql = self.mql(y=y, y_hat=y_hat, mask=mask)
+        norm = torch.sum(torch.abs(y))
+        unmean = torch.sum(mask)
+        scrps = 2 * mql * unmean / (norm + 1e-5)
+        return scrps
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/__init__.py` & `neuralforecast-1.6.0/neuralforecast/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = ['RNN', 'GRU', 'LSTM', 'TCN', 'DilatedRNN',
            'MLP', 'NHITS', 'NBEATS', 'NBEATSx',
-           'TFT', 'VanillaTransformer', 'Informer', 'Autoformer', 'PatchTST',
+           'TFT', 'VanillaTransformer', 'Informer', 'Autoformer', 'PatchTST', 'FEDformer',
            'StemGNN', 'HINT']
 
 from .rnn import RNN
 from .gru import GRU
 from .lstm import LSTM
 from .tcn import TCN
 from .dilated_rnn import DilatedRNN
@@ -13,9 +13,10 @@
 from .nbeats import NBEATS
 from .nbeatsx import NBEATSx
 from .tft import TFT
 from .stemgnn import StemGNN
 from .vanillatransformer import VanillaTransformer
 from .informer import Informer
 from .autoformer import Autoformer
+from .fedformer import FEDformer
 from .patchtst import PatchTST
 from .hint import HINT
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/autoformer.py` & `neuralforecast-1.6.0/neuralforecast/models/autoformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,32 +442,35 @@
 
     *Parameters:*<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
         `decoder_input_size_multiplier`: float = 0.5, .<br>
     `hidden_size`: int=128, units of embeddings and encoders.<br>
     `n_head`: int=4, controls number of multi-head's attention.<br>
     `dropout`: float (0, 1), dropout throughout Autoformer architecture.<br>
         `factor`: int=3, Probsparse attention factor.<br>
         `conv_hidden_size`: int=32, channels of the convolutional encoder.<br>
         `activation`: str=`GELU`, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid', 'GELU'].<br>
     `encoder_layers`: int=2, number of layers for the TCN encoder.<br>
     `decoder_layers`: int=1, number of layers for the MLP decoder.<br>
     `distil`: bool = True, wether the Autoformer decoder uses bottlenecks.<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int=32, number of differentseries in each batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=1024, number of windows to sample in each inference batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
@@ -481,14 +484,15 @@
     def __init__(
         self,
         h: int,
         input_size: int,
         stat_exog_list=None,
         hist_exog_list=None,
         futr_exog_list=None,
+        exclude_insample_y=False,
         decoder_input_size_multiplier: float = 0.5,
         hidden_size: int = 128,
         dropout: float = 0.05,
         factor: int = 3,
         n_head: int = 4,
         conv_hidden_size: int = 32,
         activation: str = "gelu",
@@ -501,37 +505,40 @@
         learning_rate: float = 1e-4,
         num_lr_decays: int = -1,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
         valid_batch_size: Optional[int] = None,
         windows_batch_size=1024,
+        inference_windows_batch_size=1024,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
         super(Autoformer, self).__init__(
             h=h,
             input_size=input_size,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
             futr_exog_list=futr_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
             windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/dilated_rnn.py` & `neuralforecast-1.6.0/neuralforecast/models/dilated_rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/gru.py` & `neuralforecast-1.6.0/neuralforecast/models/gru.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/hint.py` & `neuralforecast-1.6.0/neuralforecast/models/hint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/models.hint.ipynb.
 
 # %% auto 0
-__all__ = ['get_bottomup_P', 'get_mintrace_ols_P', 'get_mintrace_wls_P', 'HINT']
+__all__ = ['get_bottomup_P', 'get_mintrace_ols_P', 'get_mintrace_wls_P', 'get_identity_P', 'HINT']
 
-# %% ../../nbs/models.hint.ipynb 4
+# %% ../../nbs/models.hint.ipynb 5
 from typing import Optional
 
 import numpy as np
 import torch
 
-# %% ../../nbs/models.hint.ipynb 6
+# %% ../../nbs/models.hint.ipynb 7
 def get_bottomup_P(S: np.ndarray):
     """BottomUp Reconciliation Matrix.
 
     Creates BottomUp hierarchical \"projection\" matrix is defined as:
     $$\mathbf{P}_{\\text{BU}} = [\mathbf{0}_{\mathrm{[b],[a]}}\;|\;\mathbf{I}_{\mathrm{[b][b]}}]$$
 
     **Parameters:**<br>
@@ -97,26 +97,44 @@
     # Equation 10 from https://robjhyndman.com/papers/MinT.pdf
     A = S[:n_agg, :]
     U = np.hstack((np.eye(n_agg), -A)).T
     J = np.hstack((np.zeros((n_bottom, n_agg)), np.eye(n_bottom)))
     P = J - (J @ W @ U) @ np.linalg.pinv(U.T @ W @ U) @ U.T
     return P
 
-# %% ../../nbs/models.hint.ipynb 11
+
+def get_identity_P(S: np.ndarray):
+    # Placeholder function for identity P (no reconciliation).
+    pass
+
+# %% ../../nbs/models.hint.ipynb 12
 class HINT:
     """HINT
 
-    The Hierarchical Forecast Network (HINT) combines SoTA neural forecast methods with
-    flexible and efficient probability distributions and advanced hierarchical reconciliation strategies.
-    This powerful combination allows HINT to produce accurate and coherent probabilistic predictions.
+    The Hierarchical Mixture Networks (HINT) are a highly modular framework that
+    combines SoTA neural forecast architectures with a task-specialized mixture
+    probability and advanced hierarchical reconciliation strategies. This powerful
+    combination allows HINT to produce accurate and coherent probabilistic forecasts.
+
+    HINT's incorporates a `TemporalNorm` module into any neural forecast architecture,
+    the module normalizes inputs into the network's non-linearities operating range
+    and recomposes its output's scales through a global skip connection, improving
+    accuracy and training robustness. HINT ensures the forecast coherence via bootstrap
+    sample reconciliation that restores the aggregation constraints into its base samples.
+
+    Available reconciliations:<br>
+    - BottomUp<br>
+    - MinTraceOLS<br>
+    - MinTraceWLS<br>
+    - Identity
 
     **Parameters:**<br>
     `h`: int, Forecast horizon. <br>
-    `model`: NeuralForecast model, instantiated train loss class from [models collection](https://nixtla.github.io/neuralforecast/models.pytorch.html).<br>
-    `S`: np.ndarray, dumming matrix of size (`base`, `bottom`) see [aggregate method](https://nixtla.github.io/hierarchicalforecast/utils.html#aggregate).<br>
+    `model`: NeuralForecast model, instantiated model class from [architecture collection](https://nixtla.github.io/neuralforecast/models.pytorch.html).<br>
+    `S`: np.ndarray, dumming matrix of size (`base`, `bottom`) see HierarchicalForecast's [aggregate method](https://nixtla.github.io/hierarchicalforecast/utils.html#aggregate).<br>
     `reconciliation`: str, HINT's reconciliation method from ['BottomUp', 'MinTraceOLS', 'MinTraceWLS'].<br>
     `alias`: str, optional,  Custom name of the model.<br>
     """
 
     def __init__(
         self,
         h: int,
@@ -131,44 +149,50 @@
         if not model.loss.is_distribution_output:
             raise Exception(
                 f"The NeuralForecast model's loss {model.loss} is not a probabilistic objective"
             )
 
         self.h = h
         self.model = model
+        self.early_stop_patience_steps = model.early_stop_patience_steps
         self.S = S
         self.reconciliation = reconciliation
         self.loss = model.loss
 
         available_reconciliations = dict(
             BottomUp=get_bottomup_P,
             MinTraceOLS=get_mintrace_ols_P,
             MinTraceWLS=get_mintrace_wls_P,
+            Identity=get_identity_P,
         )
 
         if reconciliation not in available_reconciliations:
             raise Exception(f"Reconciliation {reconciliation} not available")
 
         # Get SP matrix
-        P = available_reconciliations[reconciliation](S=S)
-        self.SP = S @ P
+        self.reconciliation = reconciliation
+        if reconciliation == "Identity":
+            self.SP = None
+        else:
+            P = available_reconciliations[reconciliation](S=S)
+            self.SP = S @ P
 
         qs = torch.Tensor((np.arange(self.loss.num_samples) / self.loss.num_samples))
         self.sample_quantiles = torch.nn.Parameter(qs, requires_grad=False)
         self.alias = alias
 
     def __repr__(self):
         return type(self).__name__ if self.alias is None else self.alias
 
     def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
         """HINT.fit
 
-        HINT trains on the entire hierarchical dataset, by minimizing a composite log likelihood or likelihoood objective.
-        HINT's architecture integrates `TemporalNorm` for a scale-decoupled optimization that robustifies cross-learning
-        the hierachy's series scales.
+        HINT trains on the entire hierarchical dataset, by minimizing a composite log likelihood objective.
+        HINT framework integrates `TemporalNorm` into the neural forecast architecture for a scale-decoupled
+        optimization that robustifies cross-learning the hierachy's series scales.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset` see details [here](https://nixtla.github.io/neuralforecast/tsdataset.html)<br>
         `val_size`: int, size of the validation set, (default 0).<br>
         `test_size`: int, size of the test set, (default 0).<br>
         `random_seed`: int, random seed for the prediction.<br>
 
@@ -182,26 +206,36 @@
             random_seed=random_seed,
         )
 
     def predict(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """HINT.predict
 
         After fitting a base model on the entire hierarchical dataset.
-        HINT ensures hierarchical constraints using bootstrapped sample reconciliation
-        First sampling from its base forecast distribution.
+        HINT restores the hierarchical aggregation constraints using
+        bootstrapped sample reconciliation.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset` see details [here](https://nixtla.github.io/neuralforecast/tsdataset.html)<br>
         `step_size`: int, steps between sequential predictions, (default 1).<br>
         `random_seed`: int, random seed for the prediction.<br>
         `**data_kwarg`: additional parameters for the dataset module.<br>
 
         **Returns:**<br>
         `y_hat`: numpy predictions of the `NeuralForecast` model.<br>
         """
+        # Non-reconciled predictions
+        if self.reconciliation == "Identity":
+            forecasts = self.model.predict(
+                dataset=dataset,
+                step_size=step_size,
+                random_seed=random_seed,
+                **data_module_kwargs,
+            )
+            return forecasts
+
         num_samples = self.model.loss.num_samples
 
         # Hack to get samples by simulating quantiles (samples will be ordered)
         # Mysterious parsing associated to default [mean,quantiles] output
         quantiles_old = self.model.loss.quantiles
         names_old = self.model.loss.output_names
         self.model.loss.quantiles = self.sample_quantiles
@@ -233,14 +267,17 @@
         sample_mean = np.mean(forecasts, axis=-1, keepdims=True)
         forecasts = np.concatenate([sample_mean, forecasts], axis=-1)
         return forecasts
 
     def set_test_size(self, test_size):
         self.model.test_size = test_size
 
+    def get_test_size(self):
+        return self.model.test_size
+
     def save(self, path):
         """HINT.save
 
         Save the HINT fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/informer.py` & `neuralforecast-1.6.0/neuralforecast/models/informer.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,32 +181,35 @@
 
     *Parameters:*<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
         `decoder_input_size_multiplier`: float = 0.5, .<br>
     `hidden_size`: int=128, units of embeddings and encoders.<br>
     `n_head`: int=4, controls number of multi-head's attention.<br>
     `dropout`: float (0, 1), dropout throughout Informer architecture.<br>
         `factor`: int=3, Probsparse attention factor.<br>
         `conv_hidden_size`: int=32, channels of the convolutional encoder.<br>
         `activation`: str=`GELU`, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid', 'GELU'].<br>
     `encoder_layers`: int=2, number of layers for the TCN encoder.<br>
     `decoder_layers`: int=1, number of layers for the MLP decoder.<br>
     `distil`: bool = True, wether the Informer decoder uses bottlenecks.<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int=32, number of differentseries in each batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=1024, number of windows to sample in each inference batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
@@ -220,14 +223,15 @@
     def __init__(
         self,
         h: int,
         input_size: int,
         stat_exog_list=None,
         hist_exog_list=None,
         futr_exog_list=None,
+        exclude_insample_y=False,
         decoder_input_size_multiplier: float = 0.5,
         hidden_size: int = 128,
         dropout: float = 0.05,
         factor: int = 3,
         n_head: int = 4,
         conv_hidden_size: int = 32,
         activation: str = "gelu",
@@ -240,37 +244,40 @@
         learning_rate: float = 1e-4,
         num_lr_decays: int = -1,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
         valid_batch_size: Optional[int] = None,
         windows_batch_size=1024,
+        inference_windows_batch_size=1024,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
         super(Informer, self).__init__(
             h=h,
             input_size=input_size,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
             futr_exog_list=futr_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
-            windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            windows_batch_size=windows_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/lstm.py` & `neuralforecast-1.6.0/neuralforecast/models/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/mlp.py` & `neuralforecast-1.6.0/neuralforecast/models/mlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,28 @@
 
     **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, considered autorregresive inputs (lags), y=[1,2,3,4] input_size=2 -> lags=[1,2].<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
     `n_layers`: int, number of layers for the MLP.<br>
     `hidden_size`: int, number of units for each layer of the MLP.<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int=32, number of differentseries in each batch.<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
-    `windows_batch_size`: int=None, windows sampled from rolled data, if None uses all.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=-1, number of windows to sample in each inference batch, -1 uses all.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
@@ -55,50 +57,54 @@
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
+        exclude_insample_y=False,
         num_layers=2,
         hidden_size=1024,
         loss=MAE(),
         valid_loss=None,
         max_steps: int = 1000,
         learning_rate: float = 1e-3,
         num_lr_decays: int = -1,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
         valid_batch_size: Optional[int] = None,
         windows_batch_size=1024,
+        inference_windows_batch_size=-1,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs
     ):
         # Inherit BaseWindows class
         super(MLP, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
             valid_batch_size=valid_batch_size,
             windows_batch_size=windows_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/nbeats.py` & `neuralforecast-1.6.0/neuralforecast/models/nbeats.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,17 +213,18 @@
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
     `num_lr_decays`: int=3, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int, number of different series in each batch.<br>
-    `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=-1, number of windows to sample in each inference batch, -1 uses all.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
@@ -252,16 +253,17 @@
         valid_loss=None,
         max_steps: int = 1000,
         learning_rate: float = 1e-3,
         num_lr_decays: int = 3,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
-        windows_batch_size: int = 1024,
         valid_batch_size: Optional[int] = None,
+        windows_batch_size: int = 1024,
+        inference_windows_batch_size: int = -1,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
@@ -275,14 +277,15 @@
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
             windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/nbeatsx.py` & `neuralforecast-1.6.0/neuralforecast/models/nbeatsx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/models.nbeatsx.ipynb.
 
 # %% auto 0
 __all__ = ['NBEATSx']
 
-# %% ../../nbs/models.nbeatsx.ipynb 5
+# %% ../../nbs/models.nbeatsx.ipynb 6
 from typing import Tuple, Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from ..losses.pytorch import MAE
@@ -188,16 +188,15 @@
             nn.Linear(in_features=input_size, out_features=mlp_units[0][0])
         ]
         for layer in mlp_units:
             hidden_layers.append(nn.Linear(in_features=layer[0], out_features=layer[1]))
             hidden_layers.append(activ)
 
             if self.dropout_prob > 0:
-                raise NotImplementedError("dropout")
-                # hidden_layers.append(nn.Dropout(p=self.dropout_prob))
+                hidden_layers.append(nn.Dropout(p=self.dropout_prob))
 
         output_layer = [nn.Linear(in_features=mlp_units[-1][1], out_features=n_theta)]
         layers = hidden_layers + output_layer
         self.layers = nn.Sequential(*layers)
         self.basis = basis
 
     def forward(
@@ -242,31 +241,33 @@
 
     **Parameters:**<br>
     `h`: int, Forecast horizon. <br>
     `input_size`: int, autorregresive inputs size, y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2].<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
-    `n_harmonics`: int, Number of harmonic terms for trend stack type. Note that len(n_harmonics) = len(stack_types). Note that it will only be used if a trend stack is used.<br>
-    `n_polynomials`: int, Number of polynomial terms for seasonality stack type. Note that len(n_polynomials) = len(stack_types). Note that it will only be used if a seasonality stack is used.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
+    `n_harmonics`: int, Number of harmonic oscillations in the SeasonalityBasis [cos(i * t/n_harmonics), sin(i * t/n_harmonics)]. Note that it will only be used if 'seasonality' is in `stack_types`.<br>
+    `n_polynomials`: int, Number of polynomial terms for TrendBasis [1,t,...,t^n_poly]. Note that it will only be used if 'trend' is in `stack_types`.<br>
     `stack_types`: List[str], List of stack types. Subset from ['seasonality', 'trend', 'identity'].<br>
     `n_blocks`: List[int], Number of blocks for each stack. Note that len(n_blocks) = len(stack_types).<br>
     `mlp_units`: List[List[int]], Structure of hidden layers for each stack type. Each internal list should contain the number of units of each hidden layer. Note that len(n_hidden) = len(stack_types).<br>
     `dropout_prob_theta`: float, Float between (0, 1). Dropout for N-BEATS basis.<br>
     `activation`: str, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid'].<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
     `num_lr_decays`: int=3, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int, number of different series in each batch.<br>
-    `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=-1, number of windows to sample in each inference batch, -1 uses all.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random seed initialization for replicability.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
@@ -282,14 +283,15 @@
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
+        exclude_insample_y=False,
         n_harmonics=2,
         n_polynomials=2,
         stack_types: list = ["identity", "trend", "seasonality"],
         n_blocks: list = [1, 1, 1],
         mlp_units: list = 3 * [[512, 512]],
         dropout_prob_theta=0.0,
         activation="ReLU",
@@ -298,40 +300,49 @@
         valid_loss=None,
         max_steps: int = 1000,
         learning_rate: float = 1e-3,
         num_lr_decays: int = 3,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size=32,
-        windows_batch_size: int = 1024,
         valid_batch_size: Optional[int] = None,
+        windows_batch_size: int = 1024,
+        inference_windows_batch_size: int = -1,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
+        # Protect horizon collapsed seasonality and trend NBEATSx-i basis
+        if h == 1 and (("seasonality" in stack_types) or ("trend" in stack_types)):
+            raise Exception(
+                "Horizon `h=1` incompatible with `seasonality` or `trend` in stacks"
+            )
+
         # Inherit BaseWindows class
         super(NBEATSx, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
-            windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            windows_batch_size=windows_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/nhits.py` & `neuralforecast-1.6.0/neuralforecast/models/nhits.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,27 +41,32 @@
         if self.interpolation_mode in ["nearest", "linear"]:
             # knots = knots[:,None,:]
             forecast = F.interpolate(
                 knots, size=self.forecast_size, mode=self.interpolation_mode
             )
             # forecast = forecast[:,0,:]
         elif "cubic" in self.interpolation_mode:
+            if self.out_features > 1:
+                raise Exception(
+                    "Cubic interpolation not available with multiple outputs."
+                )
             batch_size = len(backcast)
             knots = knots[:, None, :, :]
             forecast = torch.zeros((len(knots), self.forecast_size)).to(knots.device)
             n_batches = int(np.ceil(len(knots) / batch_size))
             for i in range(n_batches):
                 forecast_i = F.interpolate(
                     knots[i * batch_size : (i + 1) * batch_size],
                     size=self.forecast_size,
                     mode="bicubic",
                 )
                 forecast[i * batch_size : (i + 1) * batch_size] += forecast_i[
-                    :, 0, :, :
-                ]
+                    :, 0, 0, :
+                ]  # [B,None,H,H] -> [B,H]
+            forecast = forecast[:, None, :]  # [B,H] -> [B,None,H]
 
         # [B,Q,H] -> [B,H,Q]
         forecast = forecast.permute(0, 2, 1)
         return backcast, forecast
 
 # %% ../../nbs/models.nhits.ipynb 9
 ACTIVATIONS = ["ReLU", "Softplus", "Tanh", "SELU", "LeakyReLU", "PReLU", "Sigmoid"]
@@ -120,16 +125,16 @@
             nn.Linear(in_features=input_size, out_features=mlp_units[0][0])
         ]
         for layer in mlp_units:
             hidden_layers.append(nn.Linear(in_features=layer[0], out_features=layer[1]))
             hidden_layers.append(activ)
 
             if self.dropout_prob > 0:
-                raise NotImplementedError("dropout")
-                # hidden_layers.append(nn.Dropout(p=self.dropout_prob))
+                # raise NotImplementedError('dropout')
+                hidden_layers.append(nn.Dropout(p=self.dropout_prob))
 
         output_layer = [nn.Linear(in_features=mlp_units[-1][1], out_features=n_theta)]
         layers = hidden_layers + output_layer
         self.layers = nn.Sequential(*layers)
         self.basis = basis
 
     def forward(
@@ -185,55 +190,60 @@
 
     **Parameters:**<br>
     `h`: int, Forecast horizon. <br>
     `input_size`: int, autorregresive inputs size, y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2].<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
     `activation`: str, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid'].<br>
-    `stack_types`: List[str], List of stack types. Subset from ['seasonality', 'trend', 'identity'].<br>
+    `stack_types`: List[str], stacks list in the form N * ['identity'], to be deprecated in favor of `n_stacks`. Note that len(stack_types)=len(n_freq_downsample)=len(n_pool_kernel_size).<br>
     `n_blocks`: List[int], Number of blocks for each stack. Note that len(n_blocks) = len(stack_types).<br>
     `mlp_units`: List[List[int]], Structure of hidden layers for each stack type. Each internal list should contain the number of units of each hidden layer. Note that len(n_hidden) = len(stack_types).<br>
-    `n_harmonics`: int, Number of harmonic terms for seasonality stack type. Note that len(n_harmonics) = len(stack_types). Note that it will only be used if a seasonality stack is used.<br>
-    `n_polynomials`: int, polynomial degree for trend stack. Note that len(n_polynomials) = len(stack_types). Note that it will only be used if a trend stack is used.<br>
-    `dropout_prob_theta`: float, Float between (0, 1). Dropout for N-BEATS basis.<br>
+    `n_freq_downsample`: List[int], list with the stack's coefficients (inverse expressivity ratios). Note that len(stack_types)=len(n_freq_downsample)=len(n_pool_kernel_size).<br>
+    `interpolation_mode`: str='linear', interpolation basis from ['linear', 'nearest', 'cubic'].<br>
+    `n_pool_kernel_size`: List[int], list with the size of the windows to take a max/avg over. Note that len(stack_types)=len(n_freq_downsample)=len(n_pool_kernel_size).<br>
+    `pooling_mode`: str, input pooling module from ['MaxPool1d', 'AvgPool1d'].<br>
+    `dropout_prob_theta`: float, Float between (0, 1). Dropout for NHITS basis.<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int, number of different series in each batch.<br>
-    `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=-1, number of windows to sample in each inference batch, -1 uses all.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
     **References:**<br>
     -[Cristian Challu, Kin G. Olivares, Boris N. Oreshkin, Federico Garza,
-    Max Mergenthaler-Canseco, Artur Dubrawski (2022). "NHITS: Neural Hierarchical Interpolation for Time Series Forecasting".
+    Max Mergenthaler-Canseco, Artur Dubrawski (2023). "NHITS: Neural Hierarchical Interpolation for Time Series Forecasting".
     Accepted at the Thirty-Seventh AAAI Conference on Artificial Intelligence.](https://arxiv.org/abs/2201.12886)
     """
 
     # Class attributes
     SAMPLING_TYPE = "windows"
 
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
+        exclude_insample_y=False,
         stack_types: list = ["identity", "identity", "identity"],
         n_blocks: list = [1, 1, 1],
         mlp_units: list = 3 * [[512, 512]],
         n_pool_kernel_size: list = [2, 2, 1],
         n_freq_downsample: list = [4, 2, 1],
         pooling_mode: str = "MaxPool1d",
         interpolation_mode: str = "linear",
@@ -243,40 +253,43 @@
         valid_loss=None,
         max_steps: int = 1000,
         learning_rate: float = 1e-3,
         num_lr_decays: int = 3,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
-        windows_batch_size: int = 1024,
         valid_batch_size: Optional[int] = None,
+        windows_batch_size: int = 1024,
+        inference_windows_batch_size: int = -1,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs,
     ):
         # Inherit BaseWindows class
         super(NHITS, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
             windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/patchtst.py` & `neuralforecast-1.6.0/neuralforecast/models/patchtst.py`

 * *Files 2% similar despite different names*

```diff
@@ -825,14 +825,15 @@
 
     **Parameters:**<br>
     `h`: int, Forecast horizon. <br>
     `input_size`: int, autorregresive inputs size, y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2].<br>
     `stat_exog_list`: str list, static exogenous columns.<br>
     `hist_exog_list`: str list, historic exogenous columns.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
+    `exclude_insample_y`: bool=False, the model skips the autoregressive features y[t-input_size:t] if True.<br>
     `encoder_layers`: int, number of layers for encoder.<br>
     `n_heads`: int=16, number of multi-head's attention.<br>
     `hidden_size`: int=128, units of embeddings and encoders.<br>
     `linear_hidden_size`: int=256, units of linear layer.<br>
     `dropout`: float=0.1, dropout rate for residual connection.<br>
     `fc_dropout`: float=0.1, dropout rate for linear layer.<br>
     `head_dropout`: float=0.1, dropout rate for Flatten head layer.<br>
@@ -849,17 +850,18 @@
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int, number of different series in each batch.<br>
-    `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=1024, number of windows to sample in each inference batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
@@ -874,14 +876,15 @@
     def __init__(
         self,
         h,
         input_size,
         stat_exog_list=None,
         hist_exog_list=None,
         futr_exog_list=None,
+        exclude_insample_y=False,
         encoder_layers: int = 3,
         n_heads: int = 16,
         hidden_size: int = 128,
         linear_hidden_size: int = 256,
         dropout: float = 0.2,
         fc_dropout: float = 0.2,
         head_dropout: float = 0.0,
@@ -901,37 +904,40 @@
         learning_rate: float = 1e-4,
         num_lr_decays: int = -1,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
         valid_batch_size: Optional[int] = None,
         windows_batch_size=1024,
+        inference_windows_batch_size: int = 1024,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs
     ):
         super(PatchTST, self).__init__(
             h=h,
             input_size=input_size,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
             futr_exog_list=futr_exog_list,
+            exclude_insample_y=exclude_insample_y,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
-            windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            windows_batch_size=windows_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs
         )
```

### Comparing `neuralforecast-1.5.0/neuralforecast/models/rnn.py` & `neuralforecast-1.6.0/neuralforecast/models/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/stemgnn.py` & `neuralforecast-1.6.0/neuralforecast/models/stemgnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/tcn.py` & `neuralforecast-1.6.0/neuralforecast/models/tcn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.5.0/neuralforecast/models/vanillatransformer.py` & `neuralforecast-1.6.0/neuralforecast/models/vanillatransformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,19 +96,21 @@
         `conv_hidden_size`: int=32, channels of the convolutional encoder.<br>
         `activation`: str=`GELU`, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid', 'GELU'].<br>
     `encoder_layers`: int=2, number of layers for the TCN encoder.<br>
     `decoder_layers`: int=1, number of layers for the MLP decoder.<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
-    `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
-    `batch_size`: int=32, number of differentseries in each batch.<br>
+    `batch_size`: int=32, number of different series in each batch.<br>
+    `valid_batch_size`: int=None, number of different series in each validation and test batch, if None uses batch_size.<br>
+    `windows_batch_size`: int=1024, number of windows to sample in each training batch, default uses all.<br>
+    `inference_windows_batch_size`: int=1024, number of windows to sample in each inference batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
     `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
@@ -140,14 +142,15 @@
         learning_rate: float = 1e-4,
         num_lr_decays: int = -1,
         early_stop_patience_steps: int = -1,
         val_check_steps: int = 100,
         batch_size: int = 32,
         valid_batch_size: Optional[int] = None,
         windows_batch_size=1024,
+        inference_windows_batch_size: int = 1024,
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
@@ -161,16 +164,17 @@
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
             batch_size=batch_size,
-            windows_batch_size=windows_batch_size,
             valid_batch_size=valid_batch_size,
+            windows_batch_size=windows_batch_size,
+            inference_windows_batch_size=inference_windows_batch_size,
             step_size=step_size,
             scaler_type=scaler_type,
             num_workers_loader=num_workers_loader,
             drop_last_loader=drop_last_loader,
             random_seed=random_seed,
             **trainer_kwargs,
         )
@@ -287,15 +291,15 @@
         if self.futr_input_size > 0:
             x_mark_enc = futr_exog[:, : self.input_size, :]
             x_mark_dec = futr_exog[:, -(self.label_len + self.h) :, :]
         else:
             x_mark_enc = None
             x_mark_dec = None
 
-        x_dec = torch.zeros(size=(len(insample_y), self.h, 1))
+        x_dec = torch.zeros(size=(len(insample_y), self.h, 1)).to(insample_y.device)
         x_dec = torch.cat([insample_y[:, -self.label_len :, :], x_dec], dim=1)
 
         enc_out = self.enc_embedding(insample_y, x_mark_enc)
         enc_out, _ = self.encoder(enc_out, attn_mask=None)  # attns visualization
 
         dec_out = self.dec_embedding(x_dec, x_mark_dec)
         dec_out = self.decoder(dec_out, enc_out, x_mask=None, cross_mask=None)
```

### Comparing `neuralforecast-1.5.0/neuralforecast/tsdataset.py` & `neuralforecast-1.6.0/neuralforecast/tsdataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         static=None,
         static_cols=None,
         sorted=False,
     ):
         super().__init__()
 
         self.temporal = torch.tensor(temporal, dtype=torch.float)
-        self.temporal_cols = pd.Index(list(temporal_cols) + ["available_mask"])
+        self.temporal_cols = pd.Index(list(temporal_cols))
+
         if static is not None:
             self.static = torch.tensor(static, dtype=torch.float)
             self.static_cols = static_cols
         else:
             self.static = static
             self.static_cols = static_cols
 
@@ -103,18 +104,15 @@
     def __getitem__(self, idx):
         if isinstance(idx, int):
             # Parse temporal data and pad its left
             temporal = torch.zeros(
                 size=(len(self.temporal_cols), self.max_size), dtype=torch.float32
             )
             ts = self.temporal[self.indptr[idx] : self.indptr[idx + 1], :]
-            temporal[: len(self.temporal_cols) - 1, -len(ts) :] = ts.permute(1, 0)
-
-            # Add available_mask
-            temporal[len(self.temporal_cols) - 1, -len(ts) :] = 1
+            temporal[: len(self.temporal_cols), -len(ts) :] = ts.permute(1, 0)
 
             # Add static data if available
             static = None if self.static is None else self.static[idx, :]
 
             item = dict(
                 temporal=temporal,
                 temporal_cols=self.temporal_cols,
@@ -140,28 +138,30 @@
             self.indptr, other.indptr
         )
 
     @staticmethod
     def update_dataset(dataset, future_df):
         """Add future observations to the dataset."""
 
+        # Protect consistency
+        future_df = future_df.copy()
+
         # Add Nones to missing columns (without available_mask)
         temporal_cols = dataset.temporal_cols.copy()
-        temporal_cols = temporal_cols.delete(len(temporal_cols) - 1)
         for col in temporal_cols:
             if col not in future_df.columns:
                 future_df[col] = None
+            if col == "available_mask":
+                future_df[col] = 1
 
-        # Sort columns to match self.temporal_cols
+        # Sort columns to match self.temporal_cols (without available_mask)
         future_df = future_df[["unique_id", "ds"] + temporal_cols.tolist()]
 
         # Process future_df
-        futr_dataset, indices, futr_dates, futr_index = dataset.from_df(
-            df=future_df, sort_df=dataset.sorted
-        )
+        futr_dataset, *_ = dataset.from_df(df=future_df, sort_df=dataset.sorted)
 
         # Define and fill new temporal with updated information
         len_temporal, col_temporal = dataset.temporal.shape
         new_temporal = torch.zeros(size=(len_temporal + len(future_df), col_temporal))
         new_indptr = [0]
         new_max_size = 0
 
@@ -184,15 +184,15 @@
             new_indptr.append(acum)
             if new_length > new_max_size:
                 new_max_size = new_length
 
         # Define new dataset
         updated_dataset = TimeSeriesDataset(
             temporal=new_temporal,
-            temporal_cols=temporal_cols,
+            temporal_cols=dataset.temporal_cols.copy(),
             indptr=np.array(new_indptr).astype(np.int32),
             max_size=new_max_size,
             min_size=dataset.min_size,
             static=dataset.static,
             static_cols=dataset.static_cols,
             sorted=dataset.sorted,
         )
@@ -207,18 +207,14 @@
         """
         if dataset.min_size <= left_trim + right_trim:
             raise Exception(
                 f"left_trim + right_trim ({left_trim} + {right_trim}) \
                                 must be lower than the shorter time series ({dataset.min_size})"
             )
 
-        # Remove available mask from temporal_cols
-        temporal_cols = dataset.temporal_cols.copy()
-        temporal_cols = temporal_cols.delete(len(temporal_cols) - 1)
-
         # Define and fill new temporal with trimmed information
         len_temporal, col_temporal = dataset.temporal.shape
         total_trim = (left_trim + right_trim) * dataset.n_groups
         new_temporal = torch.zeros(size=(len_temporal - total_trim, col_temporal))
         new_indptr = [0]
 
         acum = 0
@@ -233,28 +229,29 @@
 
         new_max_size = dataset.max_size - left_trim - right_trim
         new_min_size = dataset.min_size - left_trim - right_trim
 
         # Define new dataset
         updated_dataset = TimeSeriesDataset(
             temporal=new_temporal,
-            temporal_cols=temporal_cols,
+            temporal_cols=dataset.temporal_cols.copy(),
             indptr=np.array(new_indptr).astype(np.int32),
             max_size=new_max_size,
             min_size=new_min_size,
             static=dataset.static,
             static_cols=dataset.static_cols,
             sorted=dataset.sorted,
         )
 
         return updated_dataset
 
     @staticmethod
     def from_df(df, static_df=None, sort_df=False):
         # TODO: protect on equality of static_df + df indexes
+
         # Define indexes if not given
         if df.index.name != "unique_id":
             df = df.set_index("unique_id")
             if static_df is not None:
                 static_df = static_df.set_index("unique_id")
 
         df = df.set_index("ds", append=True)
@@ -274,14 +271,20 @@
         sizes = indices_sizes.values
         max_size = max(sizes)
         min_size = min(sizes)
         cum_sizes = sizes.cumsum()
         dates = df.index.get_level_values("ds")[cum_sizes - 1]
         indptr = np.append(0, cum_sizes).astype(np.int32)
 
+        # Add Available mask efficiently (without adding column to df)
+        if "available_mask" not in df.columns:
+            available_mask = np.ones((len(temporal), 1), dtype=np.float32)
+            temporal = np.append(temporal, available_mask, axis=1)
+            temporal_cols = temporal_cols.append(pd.Index(["available_mask"]))
+
         # Static features
         if static_df is not None:
             static = static_df.values
             static_cols = static_df.columns
         else:
             static = None
             static_cols = None
```

### Comparing `neuralforecast-1.5.0/neuralforecast/utils.py` & `neuralforecast-1.6.0/neuralforecast/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
                 DayOfWeek,
                 DayOfMonth,
                 DayOfYear,
             ]
         ]
 
 
-def augment_calendar_df(df, freq="h"):
+def augment_calendar_df(df, freq="H"):
     """
     > * Q - [month]
     > * M - [month]
     > * W - [Day of month, week of year]
     > * D - [Day of week, day of month, day of year]
     > * B - [Day of week, day of month, day of year]
     > * H - [Hour of day, day of week, day of month, day of year]
```

### Comparing `neuralforecast-1.5.0/neuralforecast.egg-info/PKG-INFO` & `neuralforecast-1.6.0/neuralforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.5.0
+Version: 1.6.0
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neuralforecast-1.5.0/neuralforecast.egg-info/SOURCES.txt` & `neuralforecast-1.6.0/neuralforecast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 neuralforecast/common/_scalers.py
 neuralforecast/losses/__init__.py
 neuralforecast/losses/numpy.py
 neuralforecast/losses/pytorch.py
 neuralforecast/models/__init__.py
 neuralforecast/models/autoformer.py
 neuralforecast/models/dilated_rnn.py
+neuralforecast/models/fedformer.py
 neuralforecast/models/gru.py
 neuralforecast/models/hint.py
 neuralforecast/models/informer.py
 neuralforecast/models/lstm.py
 neuralforecast/models/mlp.py
 neuralforecast/models/nbeats.py
 neuralforecast/models/nbeatsx.py
```

### Comparing `neuralforecast-1.5.0/settings.ini` & `neuralforecast-1.6.0/settings.ini`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Time series forecasting suite using deep learning models
 keywords = time-series forecasting deep-learning 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.5.0
+version = 1.6.0
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 requirements = numpy>=1.21.6 pandas>=1.3.5 torch>=2.0.0 pytorch-lightning>=2.0.0 ray[tune]>=2.2.0
```

### Comparing `neuralforecast-1.5.0/setup.py` & `neuralforecast-1.6.0/setup.py`

 * *Files identical despite different names*

