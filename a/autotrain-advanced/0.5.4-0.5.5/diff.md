# Comparing `tmp/autotrain-advanced-0.5.4.tar.gz` & `tmp/autotrain-advanced-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.5.4.tar", last modified: Mon Jul 10 11:44:51 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.5.5.tar", last modified: Tue Jul 11 12:12:53 2023, max compression
```

## Comparing `autotrain-advanced-0.5.4.tar` & `autotrain-advanced-0.5.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.4/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.4/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.4/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.007328 autotrain-advanced-0.5.4/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.007328 autotrain-advanced-0.5.4/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-10 11:44:46.000000 autotrain-advanced-0.5.4/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38472 2023-06-21 11:15:37.000000 autotrain-advanced-0.5.4/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.007328 autotrain-advanced-0.5.4/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.4/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.4/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.4/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13520 2023-07-10 11:41:35.000000 autotrain-advanced-0.5.4/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.4/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.4/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.4/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.4/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.4/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.4/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.4/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.4/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.4/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.4/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.4/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.4/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.4/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7921 2023-07-10 11:41:41.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-06-20 15:50:18.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5118 2023-07-10 11:40:14.000000 autotrain-advanced-0.5.4/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.4/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:44:51.011328 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1187 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3069 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-10 11:44:50.000000 autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.5/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.5/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.5/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-11 12:12:45.000000 autotrain-advanced-0.5.5/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38472 2023-06-21 11:15:37.000000 autotrain-advanced-0.5.5/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.5/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.5/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.5/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14109 2023-07-11 10:08:31.000000 autotrain-advanced-0.5.5/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.5/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.5/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.5/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.5/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.5/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.5/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9966 2023-07-11 12:12:06.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-06-20 15:50:18.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5525 2023-07-11 12:12:21.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.5/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1187 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3057 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.5.4/LICENSE` & `autotrain-advanced-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/PKG-INFO` & `autotrain-advanced-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.4/setup.py` & `autotrain-advanced-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/__init__.py` & `autotrain-advanced-0.5.5/src/autotrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Lint as: python3
 # pylint: enable=line-too-long
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
```

### Comparing `autotrain-advanced-0.5.4/src/autotrain/app.py` & `autotrain-advanced-0.5.5/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.5.5/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.5.5/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.5.5/src/autotrain/cli/run_llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         args.save_strategy,
         args.auto_find_batch_size,
         args.fp16,
         args.push_to_hub,
         args.use_int8,
         args.model_max_length,
         args.repo_id,
+        args.use_int4,
+        args.trainer,
     )
 
 
 class RunAutoTrainLLMCommand(BaseAutoTrainCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         run_llm_parser = parser.add_parser(
@@ -305,14 +307,27 @@
         )
         run_llm_parser.add_argument(
             "--repo_id",
             help="Repo id for hugging face hub",
             required=False,
             type=str,
         )
+        run_llm_parser.add_argument(
+            "--use_int4",
+            help="Use int4 True/False",
+            required=False,
+            action="store_true",
+        )
+        run_llm_parser.add_argument(
+            "--trainer",
+            help="Trainer type to use",
+            required=False,
+            type=str,
+            default="default",
+        )
 
         run_llm_parser.set_defaults(func=run_llm_command_factory)
 
     def __init__(
         self,
         train,
         deploy,
@@ -348,14 +363,16 @@
         save_strategy,
         auto_find_batch_size,
         fp16,
         push_to_hub,
         use_int8,
         model_max_length,
         repo_id,
+        use_int4,
+        trainer,
     ):
         self.train = train
         self.deploy = deploy
         self.inference = inference
         self.data_path = data_path
         self.train_split = train_split
         self.valid_split = valid_split
@@ -387,14 +404,16 @@
         self.save_strategy = save_strategy
         self.auto_find_batch_size = auto_find_batch_size
         self.fp16 = fp16
         self.push_to_hub = push_to_hub
         self.use_int8 = use_int8
         self.model_max_length = model_max_length
         self.repo_id = repo_id
+        self.use_int4 = use_int4
+        self.trainer = trainer
 
         if self.train:
             if self.project_name is None:
                 raise ValueError("Project name must be specified")
             if self.data_path is None:
                 raise ValueError("Data path must be specified")
             if self.model is None:
@@ -439,9 +458,11 @@
                 save_strategy=self.save_strategy,
                 auto_find_batch_size=self.auto_find_batch_size,
                 fp16=self.fp16,
                 push_to_hub=self.push_to_hub,
                 use_int8=self.use_int8,
                 model_max_length=self.model_max_length,
                 repo_id=self.repo_id,
+                use_int4=self.use_int4,
+                trainer=self.trainer,
             )
             train_llm(params)
```

### Comparing `autotrain-advanced-0.5.4/src/autotrain/dataset.py` & `autotrain-advanced-0.5.5/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/help.py` & `autotrain-advanced-0.5.5/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/params.py` & `autotrain-advanced-0.5.5/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.5.5/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.5.5/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.5.5/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.5.5/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/project.py` & `autotrain-advanced-0.5.5/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/tasks.py` & `autotrain-advanced-0.5.5/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/clm.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from huggingface_hub import HfApi
 from loguru import logger
 from peft import LoraConfig, get_peft_model, prepare_model_for_int8_training
 from transformers import (
     AutoConfig,
     AutoModelForCausalLM,
     AutoTokenizer,
+    BitsAndBytesConfig,
     Trainer,
     TrainingArguments,
     default_data_collator,
 )
+from trl import SFTTrainer
 
 from autotrain.trainers import utils
 from autotrain.trainers.callbacks import LoadBestPeftModelCallback, SavePeftModelCallback
 
 
 def train(config):
     if isinstance(config, dict):
@@ -40,55 +42,71 @@
         use_auth_token=config.huggingface_token,
         trust_remote_code=True,
     )
 
     if tokenizer.model_max_length > 2048:
         tokenizer.model_max_length = config.model_max_length
 
-    train_data = utils.process_data(
-        data=train_data,
-        tokenizer=tokenizer,
-        config=config,
-    )
-    if config.valid_split is not None:
-        valid_data = utils.process_data(
-            data=valid_data,
+    if getattr(tokenizer, "pad_token", None) is None:
+        tokenizer.pad_token = tokenizer.eos_token
+
+    if config.trainer == "default":
+        train_data = utils.process_data(
+            data=train_data,
             tokenizer=tokenizer,
             config=config,
         )
+        if config.valid_split is not None:
+            valid_data = utils.process_data(
+                data=valid_data,
+                tokenizer=tokenizer,
+                config=config,
+            )
 
     model_config = AutoConfig.from_pretrained(
         config.model_name,
         use_auth_token=config.huggingface_token,
         trust_remote_code=True,
     )
     logger.info(model_config)
 
     if config.use_peft:
+        if config.use_int4:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=config.use_int4,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_compute_dtype=torch.float16,
+                bnb_4bit_use_double_quant=False,
+            )
+        elif config.use_int8:
+            bnb_config = BitsAndBytesConfig(load_in_8bit=config.use_int8)
+        else:
+            bnb_config = BitsAndBytesConfig()
+
         model = AutoModelForCausalLM.from_pretrained(
             config.model_name,
             config=model_config,
             use_auth_token=config.huggingface_token,
+            quantization_config=bnb_config,
             torch_dtype=torch.float16,
-            load_in_8bit=config.use_int8,
             device_map="auto",
             trust_remote_code=True,
         )
     else:
         model = AutoModelForCausalLM.from_pretrained(
             config.model_name,
             config=model_config,
             use_auth_token=config.huggingface_token,
             trust_remote_code=True,
         )
 
     model.resize_token_embeddings(len(tokenizer))
 
     if config.use_peft:
-        if config.use_int8:
+        if config.use_int8 or config.use_int4:
             model = prepare_model_for_int8_training(model)
         peft_config = LoraConfig(
             r=config.lora_r,
             lora_alpha=config.lora_alpha,
             lora_dropout=config.lora_dropout,
             bias="none",
             task_type="CAUSAL_LM",
@@ -116,49 +134,50 @@
             )
         block_size = min(config.block_size, tokenizer.model_max_length)
 
     config.block_size = block_size
 
     logger.info(model)
 
-    tokenize_fn = partial(utils.tokenize, tokenizer=tokenizer, config=config)
-    group_texts_fn = partial(utils.group_texts, config=config)
-
-    train_data = train_data.map(
-        tokenize_fn,
-        batched=True,
-        num_proc=1,
-        remove_columns=list(train_data.features),
-        desc="Running tokenizer on train dataset",
-    )
+    if config.trainer == "default":
+        tokenize_fn = partial(utils.tokenize, tokenizer=tokenizer, config=config)
+        group_texts_fn = partial(utils.group_texts, config=config)
 
-    if config.valid_split is not None:
-        valid_data = valid_data.map(
+        train_data = train_data.map(
             tokenize_fn,
             batched=True,
             num_proc=1,
-            remove_columns=list(valid_data.features),
-            desc="Running tokenizer on validation dataset",
+            remove_columns=list(train_data.features),
+            desc="Running tokenizer on train dataset",
         )
 
-    train_data = train_data.map(
-        group_texts_fn,
-        batched=True,
-        num_proc=4,
-        desc=f"Grouping texts in chunks of {block_size}",
-    )
+        if config.valid_split is not None:
+            valid_data = valid_data.map(
+                tokenize_fn,
+                batched=True,
+                num_proc=1,
+                remove_columns=list(valid_data.features),
+                desc="Running tokenizer on validation dataset",
+            )
 
-    if config.valid_split is not None:
-        valid_data = valid_data.map(
+        train_data = train_data.map(
             group_texts_fn,
             batched=True,
             num_proc=4,
             desc=f"Grouping texts in chunks of {block_size}",
         )
 
+        if config.valid_split is not None:
+            valid_data = valid_data.map(
+                group_texts_fn,
+                batched=True,
+                num_proc=4,
+                desc=f"Grouping texts in chunks of {block_size}",
+            )
+
     logger.info("creating trainer")
     # trainer specific
     if config.logging_steps == -1:
         if config.valid_split is not None:
             logging_steps = int(0.2 * len(valid_data) / config.train_batch_size)
         else:
             logging_steps = int(0.2 * len(train_data) / config.train_batch_size)
@@ -200,32 +219,61 @@
             callbacks.append(LoadBestPeftModelCallback)
 
     trainer_args = dict(
         args=args,
         model=model,
     )
 
-    trainer = Trainer(
-        **trainer_args,
-        train_dataset=train_data,
-        eval_dataset=valid_data if config.valid_split is not None else None,
-        tokenizer=tokenizer,
-        data_collator=default_data_collator,
-        callbacks=callbacks,
-    )
+    if config.trainer == "default":
+        trainer = Trainer(
+            **trainer_args,
+            train_dataset=train_data,
+            eval_dataset=valid_data if config.valid_split is not None else None,
+            tokenizer=tokenizer,
+            data_collator=default_data_collator,
+            callbacks=callbacks,
+        )
+    elif config.trainer == "sft":
+        trainer = SFTTrainer(
+            **trainer_args,
+            train_dataset=train_data,
+            eval_dataset=valid_data if config.valid_split is not None else None,
+            peft_config=peft_config if config.use_peft else None,
+            dataset_text_field="text",
+            max_seq_length=config.block_size,
+            tokenizer=tokenizer,
+            packing=True,
+        )
     model.config.use_cache = False
 
     if torch.__version__ >= "2" and sys.platform != "win32":
         model = torch.compile(model)
 
+    for name, module in trainer.model.named_modules():
+        # if isinstance(module, LoraLayer):
+        #     if script_args.bf16:
+        #         module = module.to(torch.bfloat16)
+        if "norm" in name:
+            module = module.to(torch.float32)
+        # if "lm_head" in name or "embed_tokens" in name:
+        #     if hasattr(module, "weight"):
+        #         if script_args.bf16 and module.weight.dtype == torch.float32:
+        #             module = module.to(torch.bfloat16)
+
     trainer.train()
 
     logger.info("Finished training, saving model...")
     trainer.save_model(config.project_name)
 
+    model_card = utils.create_model_card()
+
+    # save model card to output directory as README.md
+    with open(f"{config.project_name}/README.md", "w") as f:
+        f.write(model_card)
+
     if config.use_peft:
         logger.info("Merging adapter weights...")
         utils.merge_adapter(
             base_model_path=config.model_name,
             target_model_path=config.project_name,
             adapter_path=config.project_name,
         )
```

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.5.5/src/autotrain/trainers/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,29 @@
 
 
 IGNORE_INDEX = -100
 DEFAULT_PAD_TOKEN = "[PAD]"
 DEFAULT_EOS_TOKEN = "</s>"
 DEFAULT_BOS_TOKEN = "</s>"
 DEFAULT_UNK_TOKEN = "</s>"
-TARGET_MODULES = {}
+TARGET_MODULES = {
+    "Salesforce/codegen25-7b-multi": "q_proj,k_proj,v_proj,o_proj,down_proj,up_proj,gate_proj",
+}
+
+MODEL_CARD = """
+---
+tags:
+- autotrain
+- text-generation
+widget:
+- text: "I love AutoTrain because "
+---
+
+# Model Trained Using AutoTrain
+"""
 
 
 class LLMTrainingParams(BaseModel):
     model_name: str = Field("gpt2", title="Model name")
     data_path: str = Field("data", title="Data path")
     train_split: str = Field("train", title="Train data config")
     valid_split: str = Field(None, title="Validation data config")
@@ -49,14 +63,16 @@
     save_strategy: str = Field("epoch", title="Save strategy")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     fp16: bool = Field(False, title="FP16")
     push_to_hub: bool = Field(False, title="Push to hub")
     use_int8: bool = Field(False, title="Use int8")
     model_max_length: int = Field(1024, title="Model max length")
     repo_id: str = Field(None, title="Repo id")
+    use_int4: bool = Field(False, title="Use int4")
+    trainer: str = Field("default", title="Trainer type")
 
 
 def process_data(data, tokenizer, config):
     data = data.to_pandas()
     data = data.fillna("")
 
     data = data[[config.text_column]]
@@ -126,7 +142,11 @@
         trust_remote_code=True,
     )
     model = model.merge_and_unload()
 
     logger.info("Saving target model...")
     model.save_pretrained(target_model_path)
     tokenizer.save_pretrained(target_model_path)
+
+
+def create_model_card():
+    return MODEL_CARD.strip()
```

### Comparing `autotrain-advanced-0.5.4/src/autotrain/utils.py` & `autotrain-advanced-0.5.5/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.4/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 python-slugify==8.0.1
 requests==2.28.2
 tensorboard
 pycocotools==2.0.6
 gradio==3.35.2
 streamlit
 einops==0.6.1
-peft==0.3.0
+peft
+trl
 
 [dev]
 albumentations==1.3.0
 boto3==1.16.49
 codecarbon==2.2.3
 datasets[vision]~=2.13.0
 evaluate==0.3.0
@@ -81,15 +82,16 @@
 python-slugify==8.0.1
 requests==2.28.2
 tensorboard
 pycocotools==2.0.6
 gradio==3.35.2
 streamlit
 einops==0.6.1
-peft==0.3.0
+peft
+trl
 black
 isort
 flake8==3.7.9
 pytest
 
 [docs]
 albumentations==1.3.0
@@ -130,15 +132,16 @@
 python-slugify==8.0.1
 requests==2.28.2
 tensorboard
 pycocotools==2.0.6
 gradio==3.35.2
 streamlit
 einops==0.6.1
-peft==0.3.0
+peft
+trl
 recommonmark
 sphinx==3.1.2
 sphinx-markdown-tables
 sphinx-rtd-theme==0.4.3
 sphinx-copybutton
 
 [quality]
@@ -180,11 +183,12 @@
 python-slugify==8.0.1
 requests==2.28.2
 tensorboard
 pycocotools==2.0.6
 gradio==3.35.2
 streamlit
 einops==0.6.1
-peft==0.3.0
+peft
+trl
 black
 isort
 flake8==3.7.9
```

