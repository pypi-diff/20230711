# Comparing `tmp/dequeai-0.810.tar.gz` & `tmp/dequeai-0.812.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.810.tar", last modified: Mon Jul 10 23:08:25 2023, max compression
+gzip compressed data, was "dequeai-0.812.tar", last modified: Mon Jul 10 23:15:29 2023, max compression
```

## Comparing `dequeai-0.810.tar` & `dequeai-0.812.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:08:25.843838 dequeai-0.810/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.810/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.810/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.810/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.810/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.810/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    14904 2023-07-10 23:07:35.000000 dequeai-0.810/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.810/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.810/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.810/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.810/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.810/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:08:25.843838 dequeai-0.810/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      514 2023-07-10 23:08:09.000000 dequeai-0.810/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:15:29.911181 dequeai-0.812/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.812/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.812/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.812/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.812/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.812/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    14904 2023-07-10 23:15:06.000000 dequeai-0.812/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.812/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.812/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.812/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.812/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.812/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:15:29.911181 dequeai-0.812/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:15:29.000000 dequeai-0.812/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:15:29.911181 dequeai-0.812/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      514 2023-07-10 23:15:16.000000 dequeai-0.812/setup.py
```

### Comparing `dequeai-0.810/dequeai/datatypes.py` & `dequeai-0.812/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/dequeai/dequeai.py` & `dequeai-0.812/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/dequeai/dequeai_model.py` & `dequeai-0.812/dequeai/dequeai_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         except ImportError:
             raise ImportError("PyTorch is required for creating model.")
 
             # Check if the model is a PyTorch model
         if not isinstance(model, torch.nn.Module):
             raise Exception('Model should be an instance of a PyTorch nn.Module.')
 
-        p2 = multiprocessing.Process(target=self._create_task, args=(model, model_card))
+        p2 = multiprocessing.Process(target=self._create_task, args=(model, model_card.to_dict()))
         p2.start()
 
     def _create_task(self, model, model_card):
 
         file_name = f"{self._project_name}.pt"
         try:
             import torch
@@ -326,15 +326,15 @@
                 headers = {'Content-type': "application/octet-stream"}
                 http_response = requests.put(url=res['url'], data=object_text, headers=headers)
             print(http_response)
 
         req_data = {"user_name": self.user_name,
                     "model_name": self._project_name, "file_url": dest_path, "bucket_name": res['bucket_name'],
                     "bucket_region": res['bucket_region'],
-                    "project_name": self._project_name, "run_id": self._run_id, "model_card": model_card.to_dict()}
+                    "project_name": self._project_name, "run_id": self._run_id, "model_card": model_card}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/appstore/model/create/",
                              json=req_data)
         res = resp.json()
         print(res)
         # we record the meta data
 
     def load(self, model_name, run_id=None):
```

### Comparing `dequeai-0.810/dequeai/dequeai_run.py` & `dequeai-0.812/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/dequeai/parsing_service.py` & `dequeai-0.812/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/dequeai/rest_connect.py` & `dequeai-0.812/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/dequeai/util.py` & `dequeai-0.812/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.810/setup.py` & `dequeai-0.812/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000810',
+    version='0.00000812',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

