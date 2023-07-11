# Comparing `tmp/aitomatic-1.2.9.tar.gz` & `tmp/aitomatic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitomatic-1.2.9.tar", last modified: Tue Jun 27 03:07:08 2023, max compression
+gzip compressed data, was "aitomatic-1.3.0.tar", last modified: Tue Jul 11 02:29:39 2023, max compression
```

## Comparing `aitomatic-1.2.9.tar` & `aitomatic-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.819754 aitomatic-1.2.9/
--rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.9/LICENSE
--rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.9/MANIFEST.in
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-27 03:07:08.819897 aitomatic-1.2.9/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.9/README.md
--rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.9/pyproject.toml
--rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.9/requirements.txt
--rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-06-27 03:07:08.820703 aitomatic-1.2.9/setup.cfg
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.801855 aitomatic-1.2.9/src/
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.806798 aitomatic-1.2.9/src/aitomatic/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/__init__.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.813218 aitomatic-1.2.9/src/aitomatic/api/
--rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8843 2023-06-26 07:24:53.000000 aitomatic-1.2.9/src/aitomatic/api/build.py
--rw-r--r--   0 hungvo     (501) staff       (20)     6890 2023-06-27 03:06:50.000000 aitomatic-1.2.9/src/aitomatic/api/client.py
--rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/api/exceptions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/model_params.py
--rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/tuning_utils.py
--rw-r--r--   0 hungvo     (501) staff       (20)    15820 2023-06-26 07:24:20.000000 aitomatic-1.2.9/src/aitomatic/api/web_model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.817371 aitomatic-1.2.9/src/aitomatic/dsl/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_conclusions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_features.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_handler.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_rules.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.9/src/aitomatic/dsl/utils.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.819238 aitomatic-1.2.9/src/aitomatic/objects/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.9/src/aitomatic/objects/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/objects/dataset.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/objects/model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.809302 aitomatic-1.2.9/src/aitomatic.egg-info/
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/SOURCES.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/dependency_links.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/requires.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/top_level.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-06-27 03:06:53.000000 aitomatic-1.2.9/version.txt
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.869127 aitomatic-1.3.0/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.3.0/LICENSE
+-rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.3.0/MANIFEST.in
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 02:29:39.869315 aitomatic-1.3.0/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.3.0/README.md
+-rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.3.0/pyproject.toml
+-rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.3.0/requirements.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-07-11 02:29:39.870600 aitomatic-1.3.0/setup.cfg
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.822116 aitomatic-1.3.0/src/
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.848249 aitomatic-1.3.0/src/aitomatic/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/__init__.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.857881 aitomatic-1.3.0/src/aitomatic/api/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    10935 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/build.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7441 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/client.py
+-rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/api/exceptions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/model_params.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/tuning_utils.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    16606 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/web_model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.864030 aitomatic-1.3.0/src/aitomatic/dsl/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_conclusions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_features.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_handler.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_rules.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.3.0/src/aitomatic/dsl/utils.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.868234 aitomatic-1.3.0/src/aitomatic/objects/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.3.0/src/aitomatic/objects/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-07-03 03:38:53.000000 aitomatic-1.3.0/src/aitomatic/objects/dataset.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/objects/model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.851384 aitomatic-1.3.0/src/aitomatic.egg-info/
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/requires.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/top_level.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-07-11 02:28:57.000000 aitomatic-1.3.0/version.txt
```

### Comparing `aitomatic-1.2.9/LICENSE` & `aitomatic-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/PKG-INFO` & `aitomatic-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.9
+Version: 1.3.0
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.9/README.md` & `aitomatic-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/setup.cfg` & `aitomatic-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/api/__init__.py` & `aitomatic-1.3.0/src/aitomatic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/api/build.py` & `aitomatic-1.3.0/src/aitomatic/api/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import time
 import pandas as pd
+import json
 from aitomatic.api.client import get_api_root, ProjectManager
 from aitomatic.api import model_params as mp
 from aitomatic.dsl.arl_handler import ARLHandler
 from typing import List, Any, Dict, Optional
 from aitomatic.objects.dataset import Dataset
 
 API_TOKEN = os.getenv("AITOMATIC_API_TOKEN")
@@ -119,75 +120,121 @@
         conclusions = knowledge.conclusions.get("conclusions", {}).keys()
         conclusion_threshold_hyperparms = [
             {k: value for k in conclusions} for value in threshold_ranges
         ]
 
         return conclusion_threshold_hyperparms
 
+    def update_training_job_status(self, training_jobs: dict) -> dict:
+        for model_name in list(training_jobs.keys):
+            status, model = self.check_model_status(model_name=model_name)
+            if (status != 'training'):
+                training_jobs.pop(model_name)
+        return training_jobs
+
+    
     def tune_model_with_hyperparams(
         self,
         tuning_params: List[Any],
         base_name: str,
         model_type: str,
         knowledge_name: str,
         data_name: str,
         mapping_data: Any,
         label_columns: Any,
         metadata: Any,
     ) -> pd.DataFrame:
         model_log = []
-        print("Creating training jobs")
-        for i, item in enumerate(tuning_params):
-            test_params = {**item}
-            model_name = f"{base_name} {i}"
-            resp = self.build_model(
-                model_type,
-                model_name,
-                knowledge_name,
-                data_name,
-                mapping_data=mapping_data,
-                label_columns=label_columns,
-                metadata=metadata,
-                **item,
-            )
-            print(f'Training model {model_name}: {resp["id"]}')
-            test_params["id"] = resp["id"]
-            test_params["model_name"] = model_name
-            model_log.append(test_params)
+        # print(f"Creating training jobs, {tuning_params}")
+        max_training_tasks = 16
+        current_training_tasks = {}
+        num_executed_jobs = 0
+        while num_executed_jobs < max_training_tasks:
+            if len(current_training_tasks) < max_training_tasks:
+                item = tuning_params[num_executed_jobs]
+                test_params = {**item}
+                model_name = f'{base_name} {num_executed_jobs}'
+                resp = self.build_model(
+                    model_type,
+                    model_name,
+                    knowledge_name,
+                    data_name,
+                    mapping_data=mapping_data,
+                    label_columns=label_columns,
+                    metadata=metadata,
+                    **item,
+                )
+                print(f'Training model {model_name}: {resp["id"]}')
+                test_params['id'] = resp['id']
+                test_params['model_name'] = model_name
+                test_params['status'] = 'training'
+                model_log.append(test_params)
+                current_training_tasks[model_name] = 'training'
+                num_executed_jobs += 1
+            else:
+                current_training_tasks = self.update_training_job_status(current_training_tasks)
+                time.sleep(5)
+                
+        # print(f'Creating training {len(tuning_params)} jobs')
+        # for i, item in enumerate(tuning_params):
+        #     test_params = {**item}
+        #     model_name = f"{base_name} {i}"
+        #     resp = self.build_model(
+        #         model_type,
+        #         model_name,
+        #         knowledge_name,
+        #         data_name,
+        #         mapping_data=mapping_data,
+        #         label_columns=label_columns,
+        #         metadata=metadata,
+        #         **item,
+        #     )
+        #     print(f'Training model {model_name}: {resp["id"]}')
+        #     test_params["id"] = resp["id"]
+        #     print(f'Creating training job for {model_name}: {test_params}')
+        #     test_params["model_name"] = model_name
+        #     model_log.append(test_params)
         model_df = pd.DataFrame(model_log)
         model_df["status"] = "training"
+        model_df["output"] = {}
+
         return model_df
 
     def check_model_status(self, model_name):
         try:
             model_info = self.project.get_model_info(model_name)
-            return model_info.status.lower()
+            return model_info.status.lower(), model_info.model_output
         except Exception as e:
             print("Checking model status, e =", e)
             return "training"
 
     def wait_for_tuning_to_complete(
         self,
         model_df: pd.DataFrame,
         file_path: str = "tuning.parquet",
         sleep_time: int = 30,
     ):
         print("Waiting for training jobs to complete")
         while True:
             for i, row in model_df.iterrows():
                 model_name = row["model_name"]
-                status = self.check_model_status(model_name)
+                status, output = self.check_model_status(model_name)
                 model_df.loc[i, "status"] = status
+                if output:
+                    model_df.at[i, "output"] = json.dumps(output)
+                else:
+                    model_df.at[i, "output"] = None
 
             success_length = len(model_df[model_df["status"] == "success"])
             error_length = len(model_df[model_df["status"] == "error"])
             df_length = len(model_df)
             print(
                 f"Waiting for training jobs to complete: [{success_length} success, {error_length} error, {df_length} total]"
             )
+            # print(f"MODEL_DF: {model_df.to_string()}")
             model_df.to_parquet(file_path)
             if model_df["status"].isin(["training"]).any():
                 time.sleep(sleep_time)
             else:
                 break
         return model_df
 
@@ -216,23 +263,24 @@
                 "max_depth": max_depth,
                 "eta": eta,
             },
         }
 
     def builld_logistic_regression_param(
         self,
+        # **kwargs
         # threshold: float = 0.5,
-        # C: float = 1.0,
+        C: float = 1.0,
         # penalty: str = 'l2'
     ):
         return {
             "type": "LogisticRegression",
             "hyperparams": {
                 # 'threshold': threshold,
-                # 'C': C,
+                'C': C,
                 # 'penalty': penalty,
             },
         }
 
     def build_random_forest_param(
         self,
         # n_estimators: int = 3,
```

### Comparing `aitomatic-1.2.9/src/aitomatic/api/client.py` & `aitomatic-1.3.0/src/aitomatic/api/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,192 +4,207 @@
 from tqdm import tqdm
 from aitomatic.dsl.arl_handler import ARLHandler
 from aitomatic.objects.model import Model
 from aitomatic.objects.dataset import Dataset
 
 
 MODEL_API_ROOT = {
-    'local': 'http://localhost:8000/',
-    'dev': 'https://model-api-dev.platform.aitomatic.com',
-    'staging': 'https://model-api-stg.platform.aitomatic.com',
-    'production': 'https://model-api-prod.platform.aitomatic.com',
+    "local": "http://localhost:8000/",
+    "dev": "https://model-api-dev.platform.aitomatic.com",
+    "staging": "https://model-api-stg.platform.aitomatic.com",
+    "production": "https://model-api-prod.platform.aitomatic.com",
 }
 
 CLIENT_API_ROOT = {
-    'local': 'http://localhost:8000/api/client',
-    'dev': 'https://dev.platform.aitomatic.com/api/client',
-    'staging': 'https://staging.platform.aitomatic.com/api/client',
-    'production': 'https://production.platform.aitomatic.com/api/client',
+    "local": "http://localhost:8000/api/client",
+    "dev": "https://dev.platform.aitomatic.com/api/client",
+    "staging": "https://staging.platform.aitomatic.com/api/client",
+    "production": "https://production.platform.aitomatic.com/api/client",
 }
 
 
 def get_api_root(aitomatic_environment=None):
     if aitomatic_environment is None:
-        aitomatic_environment = os.getenv('AITOMATIC_ENVIRONMENT')
+        aitomatic_environment = os.getenv("AITOMATIC_ENVIRONMENT")
 
     model_api_root = MODEL_API_ROOT.get(aitomatic_environment)
     client_api_root = CLIENT_API_ROOT.get(aitomatic_environment)
     return model_api_root, client_api_root
 
 
 def get_project_id(project_name: str, api_token: str = None):
     if api_token is None:
-        api_token = os.getenv('AITOMATIC_API_TOKEN')
+        api_token = os.getenv("AITOMATIC_API_TOKEN")
 
     _, api_root = get_api_root()
-    url = f'{api_root}/project'
+    url = f"{api_root}/project"
     headers = {
-        'authorization': api_token,
-        'Content-Type': 'application/json',
-        'accept': 'application/json',
+        "authorization": api_token,
+        "Content-Type": "application/json",
+        "accept": "application/json",
     }
-    data = {'project_name': project_name}
+    data = {"project_name": project_name}
     resp = requests.post(url, headers=headers, json=data)
     # Handle request errors
     if resp.status_code != 200:
-        err = f'{resp.status_code}: {resp.content}'
+        err = f"{resp.status_code}: {resp.content}"
         raise ConnectionError(err)
 
     resp_content = json.loads(resp.content)
-    id_ = resp_content['id']
+    id_ = resp_content["id"]
     return id_
 
 
 class ProjectManager:
     def __init__(self, project_name: str = None, api_token: str = None):
         if api_token is None:
-            api_token = os.getenv('AITOMATIC_API_TOKEN')
+            api_token = os.getenv("AITOMATIC_API_TOKEN")
 
         if project_name is None:
-            project_name = os.getenv('AITOMATIC_PROJECT_NAME')
-            project_id = os.getenv('AITOMATIC_PROJECT_ID')
+            project_name = os.getenv("AITOMATIC_PROJECT_NAME")
+            project_id = os.getenv("AITOMATIC_PROJECT_ID")
         else:
             project_id = get_project_id(project_name, api_token=api_token)
 
         self.project_name = project_name
         self.project_id = project_id
+        self.api_token = api_token
         self.headers = {
-            'accept': 'application/json',
-            'authorization': api_token,
-            'Content-Type': 'application/json',
+            "accept": "application/json",
+            "authorization": api_token,
+            "Content-Type": "application/json",
         }
         self.init_endpoints()
 
     def init_endpoints(self):
         _, self.API_ROOT = get_api_root()
-        self.KNOWLEDGE_LIST = f'{self.API_ROOT}/{self.project_id}/knowledges'
-        self.KNOWLEDGE_DETAIL = lambda id_: f'{self.API_ROOT}/knowledges/' + id_
-        self.MODELS_LIST = f'{self.API_ROOT}/{self.project_id}/models'
-        self.MODEL_DETAIL = lambda id_: f'{self.API_ROOT}/models/' + id_
-        self.MODEL_DELETE = f'{self.API_ROOT}/models/delete'
-        self.MODEL_BUILD = f'{self.API_ROOT}/models'
-        self.DATA_LIST = f'{self.API_ROOT}/{self.project_id}/data'
-        self.DATA_DETAIL = lambda id_: f'{self.API_ROOT}/data/' + id_
+        self.KNOWLEDGE_LIST = f"{self.API_ROOT}/{self.project_id}/knowledges"
+        self.KNOWLEDGE_DETAIL = lambda id_: f"{self.API_ROOT}/knowledges/" + id_
+        self.MODELS_LIST = f"{self.API_ROOT}/{self.project_id}/models"
+        self.MODEL_DETAIL = lambda id_: f"{self.API_ROOT}/models/" + id_
+        self.MODEL_DELETE = f"{self.API_ROOT}/models/delete"
+        self.MODEL_BUILD = f"{self.API_ROOT}/models"
+        self.DATA_LIST = f"{self.API_ROOT}/{self.project_id}/data"
+        self.DATA_DETAIL = lambda id_: f"{self.API_ROOT}/data/" + id_
+        self.DATA_UPLOAD = f"{self.API_ROOT}/data/upload"
 
     def get_model_list(self):
-        resp = self.make_request('get', self.MODELS_LIST)
+        resp = self.make_request("get", self.MODELS_LIST)
         if resp:
             models = []
             for m in resp:
                 models.append(Model(m))
             return models
 
     def get_model_info(self, model_name: str):
         id_ = self.get_model_id(model_name)
-        resp = self.make_request('get', self.MODEL_DETAIL(id_))
+        resp = self.make_request("get", self.MODEL_DETAIL(id_))
         if resp:
             model = Model(resp)
             return model
 
     def get_model_id(self, model_name: str):
-        model_list = self.make_request('get', self.MODELS_LIST)
-        id_ = [x['id'] for x in model_list if x['name'].lower() == model_name.lower()]
+        model_list = self.make_request("get", self.MODELS_LIST)
+        id_ = [x["id"] for x in model_list if x["name"].lower() == model_name.lower()]
         if len(id_) == 0:
-            raise ValueError(f'model {model_name} not found.')
+            raise ValueError(f"model {model_name} not found.")
 
         return id_[0]
 
     def get_data_info(self, data_name: str):
         id_ = self.get_data_id(data_name)
-        resp = self.make_request('get', self.DATA_DETAIL(id_))
+        resp = self.make_request("get", self.DATA_DETAIL(id_))
         if resp:
             return Dataset(resp)
 
     def get_data_id(self, data_name: str):
-        data_list = self.make_request('get', self.DATA_LIST)
-        id_ = [x['id'] for x in data_list if x['name'].lower() == data_name.lower()]
+        data_list = self.make_request("get", self.DATA_LIST)
+        id_ = [x["id"] for x in data_list if x["name"].lower() == data_name.lower()]
         if len(id_) == 0:
-            raise ValueError(f'Dataset {data_name} not found.')
+            raise ValueError(f"Dataset {data_name} not found.")
 
         return id_[0]
 
     def make_request(self, request_type: str, url: str, headers=None, **kwargs):
         if headers is None:
             headers = self.headers
 
         return make_request(request_type, url, headers=headers, **kwargs)
 
     def get_knowledge_info(self, knowledge_set_name: str) -> dict:
         id_ = self.get_knowledge_id(knowledge_set_name)
-        data = make_request('get', self.KNOWLEDGE_DETAIL(id_), headers=self.headers)
+        data = make_request("get", self.KNOWLEDGE_DETAIL(id_), headers=self.headers)
         return data
 
     def get_knowledge(self, knowledge_set_name: str) -> ARLHandler:
-        knowledge = self.get_knowledge_info(knowledge_set_name)['structured']
+        knowledge = self.get_knowledge_info(knowledge_set_name)["structured"]
         return ARLHandler(knowledge)
 
     def get_knowledge_id(self, knowledge_set_name: str):
-        knowledges = make_request('get', self.KNOWLEDGE_LIST, headers=self.headers)
+        knowledges = make_request("get", self.KNOWLEDGE_LIST, headers=self.headers)
         id_ = [
-            x['id']
+            x["id"]
             for x in knowledges
-            if x['name'].lower() == knowledge_set_name.lower()
+            if x["name"].lower() == knowledge_set_name.lower()
         ]
         if len(id_) == 0:
-            raise ValueError(f'knowledge set {knowledge_set_name} not found.')
+            raise ValueError(f"knowledge set {knowledge_set_name} not found.")
 
         return id_[0]
 
     # TODO: Move to model builder class
 
     def get_base_conclusion_mapping(self, knowledge: ARLHandler):
-        return {k: None for k in knowledge.conclusions.get('conclusions', {}).keys()}
+        return {k: None for k in knowledge.conclusions.get("conclusions", {}).keys()}
 
     def get_base_metadata(self, dataset: Dataset, model: Model):
         schema_mapping = model.schema_mapping
 
         result = {}
         dataset_metadata = dataset.metadata
         for key in schema_mapping:
             if dataset_metadata.get(schema_mapping.get(key)):
                 result[key] = dataset_metadata.get(schema_mapping.get(key))
 
         return result
 
     def delete_model_by_model_name(self, model_name):
-        data = {
-            'project': self.project_name,
-            'model_name': model_name
-        }
+        data = {"project": self.project_name, "model_name": model_name}
         self.headers["Accept-Language"] = "en-US,en;q=0.9,vi;q=0.8,es;q=0.7"
-        make_request('post', self.MODEL_DELETE, headers=self.headers, json=data)
+        make_request("post", self.MODEL_DELETE, headers=self.headers, json=data)
 
     def delete_models(self, model_names):
         for model_name in tqdm(model_names):
             self.delete_model_by_model_name(model_name)
 
+    def upload_data(self, dataset_name: str, file_name: str, file):
+        data = {
+            "project_name": self.project_name,
+            "dataset_name": dataset_name,
+        }
+        make_request(
+            "post",
+            self.DATA_UPLOAD,
+            headers={
+                "accept": "application/json",
+                "authorization": self.api_token,
+            },
+            data=data,
+            files={"file": (file_name, file, "application/parquet")},
+        )
+
 
 def make_request(request_type: str, url: str, **kwargs):
     func = getattr(requests, request_type)
     if func is None:
         raise ValueError(
-            f'Invalid request type {request_type}. ' f'Must be get, post or put'
+            f"Invalid request type {request_type}. " f"Must be get, post or put"
         )
 
     resp = func(url, **kwargs)
     # Handle request errors
     if resp.status_code != 200:
-        err = f'{resp.status_code}: {resp.content}'
+        err = f"{resp.status_code}: {resp.content}"
         raise ConnectionError(err)
 
     resp_content = json.loads(resp.content)
     return resp_content
```

### Comparing `aitomatic-1.2.9/src/aitomatic/api/model_params.py` & `aitomatic-1.3.0/src/aitomatic/api/model_params.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/api/tuning_utils.py` & `aitomatic-1.3.0/src/aitomatic/api/tuning_utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/api/web_model.py` & `aitomatic-1.3.0/src/aitomatic/api/web_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 from typing import Dict, Tuple, Union, List, Any
 from itertools import product
+from multiprocessing.pool import ThreadPool
 
 from tqdm import tqdm
 from itertools import chain
 import requests
 import json
 import pandas as pd
 import numpy as np
@@ -92,17 +93,34 @@
         N = int(chunk_max / spi) - 1
         total_batches = int(np.ceil(items / N))
         logger.info(
             f"data size too large. Running inference in chunks of "
             f"{chunk_max /1024} kb or {N} data points"
         )
         out = []
-        for Xi in tqdm(self.slice_data(X, N), total=total_batches):
+        sliced_data = self.slice_data(X, N)
+        for Xi in tqdm(sliced_data, total=total_batches):
             pred = self.predict({self.data_key: Xi, **Xother})[self.output_key]
             out.append(pred)
+        
+        # num_threads = 4
+        # pools = ThreadPool(num_threads)
+        # thread_results = []
+        # # for Xi in tqdm(sliced_data, total=total_batches):
+
+        # for i, Xi in enumerate(sliced_data):
+        #     print(f"chunkId: {i}")
+        #     thread_results.append(pools.apply_async(self.predict, args=({self.data_key: Xi, **Xother}, i)))
+        
+        # print("before out")
+        # out1 = [res.get() for res in thread_results]
+        # print(f"after out1: {out1}")
+        # # print(f"OUT1: {out1}")
+        # out = [o[0][self.output_key] for o in out1]
+        # print(f"Out: {out}")
 
         predictions = self.merge_items(out, type(X))
         return {self.output_key: predictions}
 
     def merge_items(self, items, dtype):
         """
         Merge multiple inference outputs
@@ -152,15 +170,15 @@
                 yield tmp.to_dict()
             else:
                 yield tmp
 
             Nj = Ni
             Ni = Ni + N
 
-    def predict(self, input_data: Dict) -> Dict:
+    def predict(self, input_data: Dict, chunk_id: int = None) -> Dict:
         """
         Logic to generate prediction from data
 
         :params input_data: input data for prediction, dictionary with data under key 'X'
         :return: a dictionary with key `predictions` containing the predictions
         """
         if sys.getsizeof(input_data[self.data_key]) > self.chunk_size + 1:
@@ -203,15 +221,16 @@
         # resp_data = resp_content['result']
         resp_data = resp_content
         result_file_path = resp_content["result_file_path"]
 
         # Convert response back to correct types
         # predictions format to match input_data['X'] format/types
         predictions = convert_json_to_data(resp_data["result"], types_dict)
-
+        if chunk_id != None:
+            return predictions, chunk_id
         return predictions
 
     def process(self, input_data: Dict) -> Dict:
         """
         Implement logic to generate prediction from data
         """
         return self.predict(input_data=input_data)
```

### Comparing `aitomatic-1.2.9/src/aitomatic/dsl/arl_conclusions.py` & `aitomatic-1.3.0/src/aitomatic/dsl/arl_conclusions.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/dsl/arl_features.py` & `aitomatic-1.3.0/src/aitomatic/dsl/arl_features.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/dsl/arl_handler.py` & `aitomatic-1.3.0/src/aitomatic/dsl/arl_handler.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/dsl/arl_rules.py` & `aitomatic-1.3.0/src/aitomatic/dsl/arl_rules.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/dsl/utils.py` & `aitomatic-1.3.0/src/aitomatic/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic/objects/dataset.py` & `aitomatic-1.3.0/src/aitomatic/objects/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
     raw_data: dict
 
     def __init__(self, raw_data) -> None:
         self.raw_data = raw_data
 
     @property
     def type(self) -> str:
-        return self.raw_data.get('type', '')
+        return self.raw_data.get("type", "")
 
     @property
     def metadata(self) -> dict:
-        if self.type == 'DATA':
-            return self.raw_data.get('dataset_metadata', {}).get('metadata', {})
-        if self.type == 'DESCRIBE':
+        if self.type == "DATA":
+            return self.raw_data.get("dataset_metadata", {}).get("metadata", {})
+        if self.type == "DESCRIBE":
             obj = {}
-            for var in self.raw_data.get('variables'):
-                obj[var['name']] = var
+            for var in self.raw_data.get("variables"):
+                obj[var["name"]] = var
             return obj
```

### Comparing `aitomatic-1.2.9/src/aitomatic/objects/model.py` & `aitomatic-1.3.0/src/aitomatic/objects/model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.9/src/aitomatic.egg-info/PKG-INFO` & `aitomatic-1.3.0/src/aitomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.9
+Version: 1.3.0
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.9/src/aitomatic.egg-info/SOURCES.txt` & `aitomatic-1.3.0/src/aitomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

