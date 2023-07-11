# Comparing `tmp/hpcom-0.1.5.tar.gz` & `tmp/hpcom-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpcom-0.1.5.tar", last modified: Fri Jul  7 14:43:47 2023, max compression
+gzip compressed data, was "hpcom-0.1.6.tar", last modified: Tue Jul 11 13:13:42 2023, max compression
```

## Comparing `hpcom-0.1.5.tar` & `hpcom-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-07 14:43:47.171224 hpcom-0.1.5/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.5/LICENSE
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-07 14:43:47.171224 hpcom-0.1.5/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.5/README.md
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-07 14:43:47.167224 hpcom-0.1.5/hpcom/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      239 2022-12-14 10:00:50.000000 hpcom-0.1.5/hpcom/__init__.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    46513 2023-07-07 14:33:56.000000 hpcom-0.1.5/hpcom/channel.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.5/hpcom/decorators.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.5/hpcom/hpcom_old.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     4996 2023-04-13 16:56:44.000000 hpcom-0.1.5/hpcom/metrics.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     7485 2022-11-23 13:22:15.000000 hpcom-0.1.5/hpcom/modulation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      452 2023-04-12 17:22:11.000000 hpcom-0.1.5/hpcom/plot.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    23220 2023-07-07 13:21:09.000000 hpcom-0.1.5/hpcom/signal.py
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-07 14:43:47.171224 hpcom-0.1.5/hpcom.egg-info/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-07 14:43:47.000000 hpcom-0.1.5/hpcom.egg-info/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      425 2023-07-07 14:43:47.000000 hpcom-0.1.5/hpcom.egg-info/SOURCES.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-07 14:43:47.000000 hpcom-0.1.5/hpcom.egg-info/dependency_links.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-07 14:43:47.000000 hpcom-0.1.5/hpcom.egg-info/top_level.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-07 14:40:42.000000 hpcom-0.1.5/pyproject.toml
--rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-07 14:43:47.171224 hpcom-0.1.5/setup.cfg
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-07 14:43:47.171224 hpcom-0.1.5/tests/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.5/tests/test_back_to_back.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.5/tests/test_channel_model.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.5/tests/test_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.5/tests/test_ofdm_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.5/tests/test_propagation.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:13:42.116401 hpcom-0.1.6/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.6/LICENSE
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-11 13:13:42.116401 hpcom-0.1.6/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.6/README.md
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:13:42.116401 hpcom-0.1.6/hpcom/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      239 2022-12-14 10:00:50.000000 hpcom-0.1.6/hpcom/__init__.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    46901 2023-07-11 13:09:50.000000 hpcom-0.1.6/hpcom/channel.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.6/hpcom/decorators.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.6/hpcom/hpcom_old.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     4996 2023-04-13 16:56:44.000000 hpcom-0.1.6/hpcom/metrics.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     7485 2022-11-23 13:22:15.000000 hpcom-0.1.6/hpcom/modulation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      452 2023-04-12 17:22:11.000000 hpcom-0.1.6/hpcom/plot.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    23588 2023-07-11 13:13:22.000000 hpcom-0.1.6/hpcom/signal.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:13:42.116401 hpcom-0.1.6/hpcom.egg-info/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-11 13:13:42.000000 hpcom-0.1.6/hpcom.egg-info/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      425 2023-07-11 13:13:42.000000 hpcom-0.1.6/hpcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-11 13:13:42.000000 hpcom-0.1.6/hpcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-11 13:13:42.000000 hpcom-0.1.6/hpcom.egg-info/top_level.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-11 13:13:22.000000 hpcom-0.1.6/pyproject.toml
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-11 13:13:42.116401 hpcom-0.1.6/setup.cfg
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:13:42.116401 hpcom-0.1.6/tests/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.6/tests/test_back_to_back.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.6/tests/test_channel_model.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.6/tests/test_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.6/tests/test_ofdm_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.6/tests/test_propagation.py
```

### Comparing `hpcom-0.1.5/LICENSE` & `hpcom-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/PKG-INFO` & `hpcom-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.5
+Version: 0.1.6
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.5/README.md` & `hpcom-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/hpcom/channel.py` & `hpcom-0.1.6/hpcom/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import scipy as sp
+import json
 
 from datetime import datetime
 
 from .signal import create_wdm_parameters, generate_wdm, generate_wdm_optimise, receiver, receiver_wdm,\
     nonlinear_shift, dbm_to_mw, get_default_wdm_parameters, get_points_wdm
 from .modulation import get_modulation_type_from_order, get_scale_coef_constellation, \
     get_nearest_constellation_points_unscaled
@@ -59,14 +60,28 @@
     channel['nz'] = int(channel['z_span'] / channel['dz'])  # number of steps per each span
     channel['noise_density'] = channel['h_planck'] * channel['fc'] * (channel['gain'] - 1) * channel['noise_figure']
     channel['seed'] = 'fixed'
 
     return channel
 
 
+def update_channel_parameters_from_json(json_file):
+    # Load the JSON file as a dictionary
+    with open(json_file, 'r') as f:
+        update_params = json.load(f)
+
+    # Get the default channel parameters
+    channel = get_default_channel_parameters()
+
+    # Update the default parameters with the ones from the JSON
+    channel.update(update_params)
+
+    return channel
+
+
 def create_channel_parameters(n_spans, z_span, alpha_db, gamma, noise_figure_db, dispersion_parameter, dz, seed='fixed'):
     """
     This function creates a dictionary containing the parameters of a communication channel.
 
     Args:
         n_spans: The number of spans in the channel.
         z_span: The length of each span in kilometers.
```

### Comparing `hpcom-0.1.5/hpcom/hpcom_old.py` & `hpcom-0.1.6/hpcom/hpcom_old.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/hpcom/metrics.py` & `hpcom-0.1.6/hpcom/metrics.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/hpcom/modulation.py` & `hpcom-0.1.6/hpcom/modulation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/hpcom/signal.py` & `hpcom-0.1.6/hpcom/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+import json
 
 import numpy as np
 import tensorflow as tf
 
 from datetime import datetime
 
 # from hpcom.modulation import get_n_bits, get_constellation_point, get_modulation_type_from_order, \
@@ -110,14 +111,28 @@
     wdm['modulation_type'] = get_modulation_type_from_order(wdm['m_order'])
     wdm['n_bits_symbol'] = get_n_bits(wdm['modulation_type'])
     wdm['seed'] = 'fixed'
 
     return wdm
 
 
+def update_wdm_parameters_from_json(json_file):
+    # Load the JSON file as a dictionary
+    with open(json_file, 'r') as f:
+        update_params = json.load(f)
+
+    # Get the default channel parameters
+    wdm = get_default_wdm_parameters()
+
+    # Update the default parameters with the ones from the JSON
+    wdm.update(update_params)
+
+    return wdm
+
+
 def check_wdm_parameters(wdm):
 
     if not (wdm['n_polarisations'] == 1 or wdm['n_polarisations'] == 2):
         print('[check_wdm_parameters] Error: wrong number of polarisations')
         return -1
 
     if wdm['n_channels'] % 2 == 0:
```

### Comparing `hpcom-0.1.5/hpcom.egg-info/PKG-INFO` & `hpcom-0.1.6/hpcom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.5
+Version: 0.1.6
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.5/pyproject.toml` & `hpcom-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hpcom"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Egor Sedov", email="e.sedov@g.nsu.ru" },
 ]
 description = "High performance optical communication library"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hpcom-0.1.5/tests/test_back_to_back.py` & `hpcom-0.1.6/tests/test_back_to_back.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/tests/test_channel_model.py` & `hpcom-0.1.6/tests/test_channel_model.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/tests/test_generation.py` & `hpcom-0.1.6/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/tests/test_ofdm_generation.py` & `hpcom-0.1.6/tests/test_ofdm_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.5/tests/test_propagation.py` & `hpcom-0.1.6/tests/test_propagation.py`

 * *Files identical despite different names*

