# Comparing `tmp/dequeai-0.80888.tar.gz` & `tmp/dequeai-0.810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.80888.tar", last modified: Mon Jul 10 21:01:19 2023, max compression
+gzip compressed data, was "dequeai-0.810.tar", last modified: Mon Jul 10 23:08:25 2023, max compression
```

## Comparing `dequeai-0.80888.tar` & `dequeai-0.810.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:01:19.004895 dequeai-0.80888/
--rw-r--r--   0 root         (0) root         (0)      384 2023-07-10 21:01:19.004895 dequeai-0.80888/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:01:19.004895 dequeai-0.80888/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.80888/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.80888/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.80888/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.80888/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.80888/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    14893 2023-07-10 21:00:16.000000 dequeai-0.80888/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.80888/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.80888/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.80888/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.80888/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.80888/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:01:19.004895 dequeai-0.80888/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      384 2023-07-10 21:01:18.000000 dequeai-0.80888/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 21:01:18.000000 dequeai-0.80888/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:01:18.000000 dequeai-0.80888/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 21:01:18.000000 dequeai-0.80888/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 21:01:18.000000 dequeai-0.80888/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:01:19.004895 dequeai-0.80888/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-10 21:01:01.000000 dequeai-0.80888/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:08:25.843838 dequeai-0.810/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.810/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.810/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.810/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.810/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.810/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    14904 2023-07-10 23:07:35.000000 dequeai-0.810/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.810/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.810/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.810/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.810/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.810/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:08:25.843838 dequeai-0.810/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:08:25.000000 dequeai-0.810/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:08:25.843838 dequeai-0.810/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      514 2023-07-10 23:08:09.000000 dequeai-0.810/setup.py
```

### Comparing `dequeai-0.80888/dequeai/datatypes.py` & `dequeai-0.810/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/dequeai/dequeai.py` & `dequeai-0.810/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/dequeai/dequeai_model.py` & `dequeai-0.810/dequeai/dequeai_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,30 +311,30 @@
 
         dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/model/" + file_name
 
         req_data = {"user_name": self.user_name, "destination_path": dest_path}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/appstore/model/upload/presigned_url/read/",
                              json=req_data)
         res = resp.json()
-        print(res)
+        #print(res)
         with open(file_name, 'rb') as f:
             files = {'file': (file_name, f)}
             if "fields" in res:
                 http_response = requests.post(url=res['url'], data=res['fields'], files=files)
             else:
                 # TODO: for google we need a different way to save data
                 object_text = f.read()
                 headers = {'Content-type': "application/octet-stream"}
                 http_response = requests.put(url=res['url'], data=object_text, headers=headers)
             print(http_response)
 
         req_data = {"user_name": self.user_name,
                     "model_name": self._project_name, "file_url": dest_path, "bucket_name": res['bucket_name'],
                     "bucket_region": res['bucket_region'],
-                    "project_name": self._project_name, "run_id": self._run_id, "model_card": model_card}
+                    "project_name": self._project_name, "run_id": self._run_id, "model_card": model_card.to_dict()}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/appstore/model/create/",
                              json=req_data)
         res = resp.json()
         print(res)
         # we record the meta data
 
     def load(self, model_name, run_id=None):
```

### Comparing `dequeai-0.80888/dequeai/dequeai_run.py` & `dequeai-0.810/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/dequeai/parsing_service.py` & `dequeai-0.810/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/dequeai/rest_connect.py` & `dequeai-0.810/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/dequeai/util.py` & `dequeai-0.810/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.80888/setup.py` & `dequeai-0.810/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.0000080888',
+    version='0.00000810',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
-    keywords='deque client for experiment tracking, sweep and other deep learning tooling',
+    keywords='dequeai client for deep learning',
     install_requires=[
           "coolname","requests","numpy","pillow","psutil","GPUtil","ipython","tabulate"
       ],
 )
```

