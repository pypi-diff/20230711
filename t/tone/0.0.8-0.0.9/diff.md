# Comparing `tmp/tone-0.0.8.tar.gz` & `tmp/tone-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tone-0.0.8.tar", last modified: Tue Jul 11 03:30:39 2023, max compression
+gzip compressed data, was "tone-0.0.9.tar", last modified: Tue Jul 11 03:56:50 2023, max compression
```

## Comparing `tone-0.0.8.tar` & `tone-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/
--rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.8/LICENSE
--rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.8/MANIFEST.in
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:30:39.390932 tone-0.0.8/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.8/README
--rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-11 03:30:39.390932 tone-0.0.8/setup.cfg
--rw-r--r--   0 steven    (1000) root         (0)     1205 2023-07-10 22:23:33.000000 tone-0.0.8/setup.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.387598 tone-0.0.8/tests/
--rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_all.py
--rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_base.py
--rw-r--r--   0 steven    (1000) root         (0)      437 2023-07-11 03:29:57.000000 tone-0.0.8/tests/test_learning.py
--rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_tone.py
--rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_utils_attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_utils_logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone/
--rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-11 03:30:22.000000 tone-0.0.8/tone/__init__.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone/utils/
--rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.8/tone/utils/__init__.py
--rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.8/tone/utils/attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      700 2023-07-10 23:06:01.000000 tone-0.0.8/tone/utils/ipython.py
--rw-r--r--   0 steven    (1000) root         (0)     1453 2023-07-11 03:29:24.000000 tone-0.0.8/tone/utils/learning.py
--rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.8/tone/utils/logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone.egg-info/
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      434 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/top_level.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/zip-safe
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:56:50.120859 tone-0.0.9/
+-rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.9/LICENSE
+-rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.9/MANIFEST.in
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:56:50.120859 tone-0.0.9/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.9/README
+-rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-11 03:56:50.120859 tone-0.0.9/setup.cfg
+-rw-r--r--   0 steven    (1000) root         (0)     1205 2023-07-10 22:23:33.000000 tone-0.0.9/setup.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:56:50.117526 tone-0.0.9/tests/
+-rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.9/tests/test_all.py
+-rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.9/tests/test_base.py
+-rw-r--r--   0 steven    (1000) root         (0)     1008 2023-07-11 03:56:24.000000 tone-0.0.9/tests/test_learning.py
+-rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.9/tests/test_tone.py
+-rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.9/tests/test_utils_attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.9/tests/test_utils_logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:56:50.117526 tone-0.0.9/tone/
+-rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-11 03:56:40.000000 tone-0.0.9/tone/__init__.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:56:50.120859 tone-0.0.9/tone/utils/
+-rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.9/tone/utils/__init__.py
+-rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.9/tone/utils/attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      700 2023-07-10 23:06:01.000000 tone-0.0.9/tone/utils/ipython.py
+-rw-r--r--   0 steven    (1000) root         (0)     2071 2023-07-11 03:50:10.000000 tone-0.0.9/tone/utils/learning.py
+-rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.9/tone/utils/logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:56:50.117526 tone-0.0.9/tone.egg-info/
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:56:50.000000 tone-0.0.9/tone.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)      434 2023-07-11 03:56:50.000000 tone-0.0.9/tone.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:56:50.000000 tone-0.0.9/tone.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-11 03:56:50.000000 tone-0.0.9/tone.egg-info/top_level.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:56:50.000000 tone-0.0.9/tone.egg-info/zip-safe
```

### Comparing `tone-0.0.8/LICENSE` & `tone-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/setup.py` & `tone-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/tests/test_utils_attrdict.py` & `tone-0.0.9/tests/test_utils_attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/tests/test_utils_logger.py` & `tone-0.0.9/tests/test_utils_logger.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/tone/utils/attrdict.py` & `tone-0.0.9/tone/utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/tone/utils/ipython.py` & `tone-0.0.9/tone/utils/ipython.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.8/tone/utils/learning.py` & `tone-0.0.9/tone/utils/learning.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,14 +39,41 @@
     dirname = os.path.dirname(filename)
     if not os.path.exists(dirname):
         os.makedirs(dirname)
 
     torch.save(model.state_dict(), filename)
 
 
+def save_module(model, filename):
+    from .attrdict import attrdict
+    import pickle
+    import os
+    attr = attrdict()
+    attr.classname = type(model)
+    attr.state_dict = model.state_dict()
+
+    dirname = os.path.dirname(filename)
+    if not os.path.exists(dirname):
+        os.makedirs(dirname)
+
+    with open(filename, 'wb') as file:
+        file.write(pickle.dumps(attr))
+
+
+def load_module(filename):
+    import pickle
+    with open(filename, 'rb') as file:
+        attr = pickle.loads(file.read())
+
+    model = attr.classname()
+    model.load_state_dict(attr.state_dict)
+    model.eval()
+    return model
+
+
 def metrics(y_true, y_pred):
     from .attrdict import attrdict
     from sklearn import metrics as m
     import math
 
     scores = attrdict()
     scores.mape = m.mean_absolute_percentage_error(y_true, y_pred)
```

### Comparing `tone-0.0.8/tone/utils/logger.py` & `tone-0.0.9/tone/utils/logger.py`

 * *Files identical despite different names*

