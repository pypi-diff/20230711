# Comparing `tmp/dequeai-0.812.tar.gz` & `tmp/dequeai-0.8124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.812.tar", last modified: Mon Jul 10 23:15:29 2023, max compression
+gzip compressed data, was "dequeai-0.8124.tar", last modified: Mon Jul 10 23:22:26 2023, max compression
```

## Comparing `dequeai-0.812.tar` & `dequeai-0.8124.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:15:29.911181 dequeai-0.812/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.812/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.812/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.812/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.812/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.812/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    14904 2023-07-10 23:15:06.000000 dequeai-0.812/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.812/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.812/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.812/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.812/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.812/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:15:29.911181 dequeai-0.812/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      514 2023-07-10 23:15:16.000000 dequeai-0.812/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:22:26.497412 dequeai-0.8124/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-10 23:22:26.497412 dequeai-0.8124/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:22:26.497412 dequeai-0.8124/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8124/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.8124/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8124/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8124/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8124/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    15175 2023-07-10 23:21:44.000000 dequeai-0.8124/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8124/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8124/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8124/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8124/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8124/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:22:26.497412 dequeai-0.8124/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-10 23:22:26.000000 dequeai-0.8124/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:22:26.000000 dequeai-0.8124/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:22:26.000000 dequeai-0.8124/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:22:26.000000 dequeai-0.8124/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:22:26.000000 dequeai-0.8124/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:22:26.497412 dequeai-0.8124/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-10 23:22:13.000000 dequeai-0.8124/setup.py
```

### Comparing `dequeai-0.812/dequeai/datatypes.py` & `dequeai-0.8124/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/dequeai/dequeai.py` & `dequeai-0.8124/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/dequeai/dequeai_model.py` & `dequeai-0.8124/dequeai/dequeai_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -279,26 +279,32 @@
     def init(self, user_name, api_key, run_id, project_name=None):
         self.user_name = user_name
         self.api_key = api_key
         self._project_name = project_name
         self._run_id = run_id
 
     def create(self, model, model_card: ModelCard):
+
         if self.user_name is None:
             raise Exception("Please call dequeai.init(user_name, api_key, project_name) before creating model")
         if model is None:
             raise Exception("Please provide a valid model")
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for creating model.")
+        if model_card is None:
+            raise Exception("Please provide a valid model card")
 
-            # Check if the model is a PyTorch model
+        if not isinstance(model_card, ModelCard):
+            raise Exception("Please create a ModelCard object and pass it as an argument")
+        # Check if the model is a PyTorch model
         if not isinstance(model, torch.nn.Module):
             raise Exception('Model should be an instance of a PyTorch nn.Module.')
+        self.model_card = model_card
 
         p2 = multiprocessing.Process(target=self._create_task, args=(model, model_card.to_dict()))
         p2.start()
 
     def _create_task(self, model, model_card):
 
         file_name = f"{self._project_name}.pt"
```

### Comparing `dequeai-0.812/dequeai/dequeai_run.py` & `dequeai-0.8124/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/dequeai/parsing_service.py` & `dequeai-0.8124/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/dequeai/rest_connect.py` & `dequeai-0.8124/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/dequeai/util.py` & `dequeai-0.8124/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.812/setup.py` & `dequeai-0.8124/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000812',
+    version='0.000008124',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

