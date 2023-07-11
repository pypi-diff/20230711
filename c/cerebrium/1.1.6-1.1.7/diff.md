# Comparing `tmp/cerebrium-1.1.6.tar.gz` & `tmp/cerebrium-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.6.tar", max compression
+gzip compressed data, was "cerebrium-1.1.7.tar", max compression
```

## Comparing `cerebrium-1.1.6.tar` & `cerebrium-1.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      371 2023-07-04 21:43:42.070319 cerebrium-1.1.6/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-04 21:43:42.070319 cerebrium-1.1.6/LICENSE
--rw-r--r--   0        0        0      381 2023-07-04 21:47:35.642349 cerebrium-1.1.6/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    21838 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/cli.py
--rw-r--r--   0        0        0    31606 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/conduit.py
--rw-r--r--   0        0        0     5050 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/errors.py
--rw-r--r--   0        0        0    11300 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/flow.py
--rw-r--r--   0        0        0     2777 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3798 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      914 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/base.py
--rw-r--r--   0        0        0      447 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      419 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1118 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      150 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      344 2023-07-04 21:43:42.070319 cerebrium-1.1.6/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8753 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/requests.py
--rw-r--r--   0        0        0     5297 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/README.md
--rw-r--r--   0        0        0        0 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     9047 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1520 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/__init__.py
--rw-r--r--   0        0        0     2703 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/base_dataset.py
--rw-r--r--   0        0        0     3750 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/data_validator.py
--rw-r--r--   0        0        0     2007 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/templates/README.md
--rw-r--r--   0        0        0      530 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/templates/alpaca.json
--rw-r--r--   0        0        0      269 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/templates/alpaca_short.json
--rw-r--r--   0        0        0      597 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/trainer/userDataset/templates/vigogne.json
--rw-r--r--   0        0        0      466 2023-07-04 21:43:42.074319 cerebrium-1.1.6/cerebrium/utils.py
--rw-r--r--   0        0        0     2656 2023-07-04 21:47:35.642349 cerebrium-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 cerebrium-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      371 2023-07-11 17:11:12.024782 cerebrium-1.1.7/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-11 17:11:12.024782 cerebrium-1.1.7/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-11 17:13:42.066247 cerebrium-1.1.7/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    25081 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/cli.py
+-rw-r--r--   0        0        0    33936 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      411 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/requests.py
+-rw-r--r--   0        0        0    11285 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-11 17:11:12.024782 cerebrium-1.1.7/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     2174 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/diffuser_config.yaml
+-rw-r--r--   0        0        0    14933 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     9079 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     3909 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1614 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/trainer/transformer_config.yaml
+-rw-r--r--   0        0        0     1048 2023-07-11 17:11:12.028782 cerebrium-1.1.7/cerebrium/utils.py
+-rw-r--r--   0        0        0     2378 2023-07-11 17:13:42.066247 cerebrium-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 cerebrium-1.1.7/PKG-INFO
```

### Comparing `cerebrium-1.1.6/LICENSE` & `cerebrium-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.6/cerebrium/cli.py` & `cerebrium-1.1.7/cerebrium/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import json
 import os
 import re
 import sys
 import tempfile
 import time
 import zipfile
-from typing import List
+from typing import Union
 
 import requests
 import typer
 import yaml
 import yaspin
 from termcolor import colored
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
-from cerebrium import FineTuner
+from cerebrium import trainer
 from cerebrium import __version__ as cerebrium_version
 
 app = typer.Typer()
 env = os.getenv("ENV", "prod")
 
 dashboard_url = (
     "https://dashboard.cerebrium.ai"
@@ -177,23 +177,40 @@
     project_id = upload_url_response.json()["projectId"]
     zip_file_name = upload_url_response.json()["keyName"]
     endpoint = upload_url_response.json()["internalEndpoint"]
     build_id = upload_url_response.json()["buildId"]
 
     print(f"🆔 Build ID: {build_id}")
 
+    def ensure_pattern_format(pattern):
+        if not pattern.startswith("./"):
+            pattern = f"./{pattern}"
+        elif pattern.startswith("/"):
+            raise ValueError(
+                "Pattern cannot start with a forward slash. Please use a relative path."
+            )
+        if pattern.endswith("/"):
+            pattern = f"{pattern}*"
+        elif os.path.isdir(pattern) and not pattern.endswith("/"):
+            pattern = f"{pattern}/*"
+        return pattern
+
     # Zip all files in the current directory and upload to S3
     with tempfile.TemporaryDirectory() as temp_dir:
         zip_path = os.path.join(temp_dir, zip_file_name)
         dir_name = os.path.dirname(zip_path)
         os.makedirs(dir_name, exist_ok=True)
         with zipfile.ZipFile(zip_path, "w") as zip_file:
             # include files
-            include_set = set(include.strip("[]").split(","))
-            exclude_set = set(exclude.strip("[]").split(","))
+            include_set = include.strip("[]").split(",")
+            # Force include main.py, requirements.txt, pkglist.txt and conda_pkglist.txt
+            include_set.extend(["./main.py", "./requirements.txt", "./pkglist.txt", "./conda_pkglist.txt"])
+            include_set = set(ensure_pattern_format(pattern) for pattern in include_set)
+            exclude_set = exclude.strip("[]").split(",")
+            exclude_set = set(ensure_pattern_format(pattern) for pattern in exclude_set)
             file_list = []
             for root, _, files in os.walk("./"):
                 for file in files:
                     full_path = os.path.join(root, file)
                     if any(
                         fnmatch.fnmatch(full_path, pattern) for pattern in include_set
                     ) and not any(
@@ -285,19 +302,18 @@
                     ):  # If the regex matches the beginning of the string
                         created = match[1]
                         message = message[len(created) + 2 :]
                     if spinner:
                         spinner.write(f"{message}")
                     else:
                         print(message)
+                elif spinner:
+                    spinner.write("\n")
                 else:
-                    if spinner:
-                        spinner.write("\n")
-                    else:
-                        print()
+                    print()
             seen_index = len(logs)
             if spinner:
                 spinner.text = f"🔨 Building... Status: {build_status}"
             time.sleep(1)
         if time.time() - t1 > 600:
             msg = "⏲️ Build timed out."
             if spinner:
@@ -369,24 +385,24 @@
 
 @app.command()
 def get_training_logs(
     job_id: str = typer.Argument(
         ..., help="Job ID returned for your training instance."
     ),
     api_key: str = typer.Option("", help="Private API key for the user."),
-    polling_duration: int = typer.Argument(
+    max_polling_duration: int = typer.Option(
         6000, help="Number of seconds to poll the training. Maximum of 15min."
     ),
 ):
     print(f"Retrieving training logs for {job_id}...")
     if not api_key:
         api_key = get_api_key()
 
     interval = 5  # seconds between polling.
-    polling_duration = min(polling_duration, 60 * 15)
+    max_polling_duration = min(max_polling_duration, 60 * 15)
 
     # Poll the trainingLogs and make the output pretty
     seen_index = 0
     t_start = time.time()
     with yaspin.yaspin(text="CHECKING...", color="green") as spinner:
         train_status = "CHECKING..."
         while train_status != "succeeded":
@@ -403,29 +419,46 @@
                 )
                 spinner.fail(
                     f"❌ Error fetching training job logs: {train_status_response.text}"
                 )
                 train_status_response.raise_for_status()
                 sys.exit(1)
             else:
-                train_status = train_status_response.json()["status"]
-                if train_status == "pending":
+                training_response = train_status_response.json()
+                train_status = training_response["status"]
+                if (
+                    train_status == "pending"
+                ):  # pending containers have no logs. Update status and continue.
                     spinner.text = f"🏋️ Training... Status: {train_status}"
                     time.sleep(interval)
                     continue
 
-                if not (
-                    response_logs := train_status_response.json().get(
-                        "trainingLogs", None
-                    )
+                if not (  # If no logs, continue
+                    response_logs := training_response.get("trainingLogs", None)
                 ):
                     continue
 
                 concat_logs = "".join(response_logs)
                 logs = concat_logs.split("\n")[:-1]
+
+                # If the logs are unavailible and the training has succeeded, the instance has been recycled.
+                # Notify the user.
+                fail_phrase = "Unfortunately live logs are not available for this job at the moment."  # hardcoded but corresponds to dashboard backend.
+                if (
+                    train_status == "succeeded"
+                    and response_logs[0].find(fail_phrase) != -1
+                ):
+                    spinner.write(f"🏋️ Training... Status: {train_status}")
+                    spinner.write(
+                        f"❌ Could not retrieve logs for job: `{job_id}`. Logs are deleted 12hrs after a job has ended."
+                    )
+                    spinner.text = ""
+                    time.sleep(0.2)  # to allow the spinner text time to update
+                    break
+
                 for message in logs[seen_index:]:
                     if message:
                         match = re.match(
                             r"^(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{9})Z ", message
                         )
                         if (
                             match is not None
@@ -433,51 +466,54 @@
                             created = match[1]
                             message = message[len(created) + 2 :]
                         spinner.write(f"{message}")
                     else:
                         spinner.write("\n")
 
                 seen_index = len(logs)
+
                 spinner.text = f"🏋️ Training... Status: {train_status}"
+                if train_status == "succeeded":
+                    break
                 time.sleep(interval)
-            if time.time() - t_start > polling_duration:
+            if time.time() - t_start > max_polling_duration:
                 spinner.fail("⏲️ Training polling timed out.")
                 sys.exit(1)
             elif train_status == "failed":
                 spinner.fail("❌ Training failed.")
                 sys.exit(1)
         spinner.ok("🚀 Training complete!")
 
 
 @app.command()
 def get_training_jobs(
     api_key: str = typer.Option("", help="Private API key for the user."),
     last_n: int = typer.Option(
-        0, help="Number of last training jobs to fetch. Defaults to all"
+        10, help="Number of last training jobs to fetch. Defaults to all"
     ),
 ):
     print("Getting status of recent training jobs...")
     if not api_key:
         api_key = get_api_key()
     status_response = requests.post(
         f"{api_url}/jobs",
         # f"{api_url}/training-jobs",
         headers={"Authorization": api_key},
         json={},
     )
 
     if status_response.status_code != 200:
-        print("API request failed with status code:", status_response.status_code)
+        print("❌ API request failed with status code:", status_response.status_code)
         print("Error: ", status_response.text)
         status_response.raise_for_status()
 
     trainingJobArr = status_response.json()["trainingJobArr"]
 
     if last_n > 0:
-        trainingJobArr = trainingJobArr[:last_n]  # get the last n jobs
+        trainingJobArr = trainingJobArr[-last_n:]  # get the last n jobs
 
     # make the printing pretty using panels and boxes using rich. Not for MVP
     if len(trainingJobArr):
         print(
             f"\n{'-' * 60}\n✅Found the following training jobs:\n{'-' * 60}\n{'=' * 60}"
         )
         for trainingJob in trainingJobArr:
@@ -492,66 +528,109 @@
             )
     else:
         print("❌ Found no training jobs")  # redundant catch in case.
 
 
 @app.command()
 def train(
-    name: str = typer.Argument(..., help="Name for your training instance."),
-    api_key: str = typer.Option("", help="Private API key for the user."),
-    hf_model_path: str = typer.Argument(..., help="Huggingface model path to use."),
-    local_dataset_path: str = typer.Argument(
-        ..., help="Path to your local dataset JSON file."
-    ),
-    training_args: str = typer.Option(
-        "",
-        help='Json training arguments for the model. Example: \'{"num_train_epochs": 5, "learning_rate": 1e-4}\'',
-    ),
-    hardware: str = typer.Option(
-        "A10",
-        help="Hardware to use for the builder deployment. Can be one of 'CPU', 'GPU' or 'A10'. !!! NOT IN USE !!!",
-    ),
-    model_type: str = typer.Option(
-        "AutoModelForCausalLM",
-        help="Huggingface model type used to load in pretrained weights.",
+    # Command line takes priority. All can be set in config.
+    config_file: str = typer.Option(
+        None,
+        help="Path to your config YAML file containing your args for training. Will be overridden by command line args.",
+    ),
+    training_type: Union[str, None] = typer.Option(
+        None,
+        help='Type of training to run if not provided in the config. Can be either "diffuser" or "transformer".',
+    ),
+    name: str = typer.Option(
+        None, help="Name for your training instance. Overrides config file."
+    ),
+    api_key: Union[str, None] = typer.Option(
+        None, help="Private API key for the user. Overrides the config file"
+    ),
+    config_string: str = typer.Option(
+        None,
+        help="Config JSON string to use for training. Overrides the config file if the file is provided.",
     ),
     init_debug: bool = typer.Option(
         False,
         help="Stops the container after initialization.",
     ),
     pre_init_debug: bool = typer.Option(
         False,
         help="Stops the container before initialization.",
     ),
-    log_level: str = typer.Option(
-        "INFO",
-        help="Log level for the builder deployment. Can be one of 'DEBUG' or 'INFO'",
+    log_level: Union[str, None] = typer.Option(
+        None,
+        help="Log level for the builder deployment. Can be one of 'DEBUG', 'INFO', 'WARNING' or 'ERROR'. Overrides the config file.",
     ),
 ):
     """
     Deploy a fine tuning to Cerebrium
     """
-    print(f"Fine tuning {name} with {hardware} hardware to Cerebrium...")
+    # check only a config file or a config string is specified
+    assert (
+        config_file or config_string
+    ), "At least one of --config-file or --config-string must be specified."
+
+    # if config file or json, load in
+    if config_file:
+        with open(config_file, "r") as f:
+            config = yaml.safe_load(f)
+    else:
+        config = {}
+
+    if config_string:
+        config_json = json.loads(config_string)
+        config.update(config_json)
+
+    # check if training type is specified in config
+    training_type = (
+        training_type or config.get("training_type")
+    )
+    assert (
+        training_type is not None
+    ), "Training type must be specified in config or command line args."
+
+    # overwrite with command line args if present
+    name = name or config["name"]
+    if not api_key:
+        api_key = config.get("api_key")  # default to config from either the file or the string
+
+    # If api key is not provided in any parameter or config, check if it is in the login config file
     if not api_key:
         api_key = get_api_key()
-    # Creating the training object
 
-    user_training_args = json.loads(training_args) if training_args else {}
+    # get log level
+    log_level = log_level or config.get("log_level", "INFO")
 
-    finetuning = FineTuner(
-        experiment_name=name,
-        hf_model_path=hf_model_path,
-        dataset_path=local_dataset_path,
-        model_type=model_type,
-        api_key=api_key,
-        training_kwargs=user_training_args,
-    )
-    finetuning._upload(
-        init_debug=init_debug, pre_init_debug=pre_init_debug, log_level=log_level
-    )
+    # check which training
+    if training_type == "diffuser":
+        diffuser_tuning = trainer.DiffuserTuner(
+            name=name, config=config, log_level=log_level
+        )
+        # upload
+        diffuser_tuning._upload(
+            api_key=api_key,
+            init_debug=init_debug,
+            pre_init_debug=pre_init_debug,
+            log_level=log_level,
+        )
+    elif training_type == "transformer":
+        finetuning = trainer.FineTuner(
+            name=name,
+            config=config,
+            log_level=log_level,
+        )
+        finetuning._upload(
+            api_key=api_key,
+            init_debug=init_debug,
+            pre_init_debug=pre_init_debug,
+            log_level=log_level,
+        )
 
 
 @app.command()
 def download_model(
     job_id: str = typer.Argument(..., help="Job ID of your trained model."),
     api_key: str = typer.Option("", help="Private API key for the user."),
     download_path: str = typer.Option(
```

### Comparing `cerebrium-1.1.6/cerebrium/conduit.py` & `cerebrium-1.1.7/cerebrium/conduit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import enum
 import json
 import os
 import re
 import tempfile
 import zipfile
+import requests
 from copy import deepcopy
 from inspect import getsource, signature
 from types import FunctionType
 from typing import Any, Dict, Literal, Union
-
-import requests
+from typing_extensions import Self
 from cloudpickle import load as pickle_load
-from numpy import atleast_2d, ndarray
-from torch.cuda import is_available
-from torch.jit import load as torchscript_load  # type: ignore
-from torch.nn import Module as TorchModule
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from cerebrium import __version__
 from cerebrium.flow import CerebriumFlow, _check_flow_type, _flow_string
 from cerebrium.logging.base import LoggingPlatform
 from cerebrium.models.base import ModelType
@@ -56,18 +52,15 @@
         name: str = "",
         api_key: str = "",
         flow: CerebriumFlow = [],
         hardware: Union[Hardware, None] = None,
         from_json: str = "",
     ):
         if not from_json:
-            if api_key != "":
-                self.api_key = api_key
-            else:
-                self.api_key = os.environ.get("CEREBRIUM_API_KEY", "")
+            self.api_key = api_key or os.environ.get("CEREBRIUM_API_KEY", "")
             assert name != "" and self.api_key != ""
             # Check that the flow name is valid
             if len(name) > 20:
                 raise ValueError("Conduit name must be less than 20 characters")
             if not bool(re.match(REGEX_NAME_PATTERN, name)):
                 raise ValueError(
                     "Conduit name can only contain lowercase alphanumeric characters and hyphens"
@@ -95,79 +88,90 @@
                         processors,
                     )
                 hardware = Hardware(config["hardware"])
         _set_api_key(self.api_key)
         self.graph = []
         self.ready = False
         self.loggers = {}
-        if hardware:
-            self.hardware = hardware
-        else:
-            self.hardware = self._determine_hardware()
-        self.device = (
-            "cuda" if self.hardware == Hardware.GPU and is_available() else "cpu"
-        )
+        self.hardware = hardware or self._determine_hardware()
+        try:
+            from torch.cuda import is_available
+
+            self.device = (
+                "cuda" if self.hardware == Hardware.GPU and is_available() else "cpu"
+            )
+        except ImportError:
+            self.device = "cpu"
+        self.contains_torch_model = False
 
     def _determine_hardware(self):
         # Set the default hardware to GPU if the flow contains a Torch, ONNX or HuggingFace model
         if any(
-            [
-                model_type
-                in [ModelType.TORCH, ModelType.ONNX, ModelType.HUGGINGFACE_PIPELINE]
-                for model_type, _, _ in self.flow  # type: ignore
-            ]
+            model_type
+            in [ModelType.TORCH, ModelType.ONNX, ModelType.HUGGINGFACE_PIPELINE]
+            for model_type, _, _ in self.flow
         ):
             return Hardware.GPU
         else:
             return Hardware.CPU
 
     def load(self, directory: str = "/cache/", direct_from_flow: bool = False):
         """
         Load the Conduit components from the stored Model Flow into the computation graph.
 
         Args:
             directory (str): The directory to load the Conduit components from.
         """
-        from sklearn.base import ClassifierMixin, RegressorMixin, BaseEstimator
-
         if self.flow == []:
             raise ValueError("Conduit is empty. Please add models to the Conduit flow.")
-        else:
+        if not self.ready:
             for model_type, model_initialization, _ in self.flow:  # type: ignore
-                # Use correct path
+                # run correct path
                 if direct_from_flow:
                     model_initialization: str = os.path.abspath(model_initialization)
-                elif (
-                    model_type != ModelType.PREBUILT
-                    and model_type != ModelType.HUGGINGFACE_PIPELINE
-                ):
+                elif model_type not in [
+                    ModelType.PREBUILT,
+                    ModelType.HUGGINGFACE_PIPELINE,
+                ]:
                     model_initialization: str = (
                         directory + model_initialization.split("/")[-1]
                     )
-                else:
-                    pass
-
                 # Torch
                 if model_type == ModelType.TORCH:
                     from cerebrium.models.torch import TorchModel
 
+                    try:
+                        from torch.nn import Module as TorchModule
+                        from torch.jit import load as torchscript_load
+                    except ImportError as e:
+                        raise ImportError(
+                            "PyTorch not installed. Please install `torch` with pip or conda to run this model type."
+                        ) from e
+                    self.contains_torch_model = True
+
                     if model_initialization.endswith(".pt"):
                         torch_model: TorchModule = torchscript_load(
                             model_initialization
                         )
                     else:
                         with open(model_initialization, "rb") as f:
                             torch_model: TorchModule = pickle_load(f)
                     torch_model.to(self.device)
                     self.graph.append(TorchModel(torch_model))
 
                 # ONNX
                 elif model_type == ModelType.ONNX:
                     from cerebrium.models.onnx import OnnxModel
-                    from onnxruntime import InferenceSession
+
+                    try:
+                        from onnxruntime import InferenceSession
+                    except ImportError as e:
+                        raise ImportError(
+                            "ONNX not installed. Please install `onnxruntime` with pip or conda to run this model type."
+                        ) from e
 
                     providers = (
                         ["CUDAExecutionProvider", "CPUExecutionProvider"]
                         if self.device == "cuda"
                         else ["CPUExecutionProvider"]
                     )
                     onnx_model = InferenceSession(
@@ -177,250 +181,310 @@
                     self.graph.append(OnnxModel(onnx_model))
 
                 # Spacy
                 elif model_type == ModelType.SPACY:
                     from cerebrium.models.spacy import SpacyModel
                     from spacy import load as spacy_load
 
+                    try:
+                        from spacy import load as spacy_load
+                    except ImportError as e:
+                        raise ImportError(
+                            "SpaCy not installed. Please install `spacy` with pip or conda to run this model type."
+                        ) from e
+
                     spacy_model = spacy_load(model_initialization)
                     self.graph.append(SpacyModel(spacy_model))
 
                 # XGBoost
                 elif model_type == ModelType.XGBOOST_CLASSIFIER:
                     from cerebrium.models.sklearn import SKClassifierModel
-                    from xgboost import XGBClassifier
+
+                    try:
+                        from xgboost import XGBClassifier
+                    except ImportError as e:
+                        raise ImportError(
+                            "XGBoost not installed. Please install `xgboost` with pip or conda to run this model type."
+                        ) from e
 
                     if model_initialization.endswith("json"):
                         xgb_classifier = XGBClassifier()
                         xgb_classifier.load_model(model_initialization)
                     else:
                         with open(model_initialization, "rb") as f:
                             xgb_classifier: XGBClassifier = pickle_load(f)
                     self.graph.append(SKClassifierModel(xgb_classifier))
 
                 elif model_type == ModelType.XGBOOST_REGRESSOR:
                     from cerebrium.models.sklearn import SKRegressorModel
-                    from xgboost import XGBRegressor
+
+                    try:
+                        from xgboost import XGBRegressor
+                    except ImportError as e:
+                        raise ImportError(
+                            "XGBoost not installed. Please install `xgboost` with pip or conda to run this model type."
+                        ) from e
 
                     if model_initialization.endswith("json"):
                         xgb_regressor = XGBRegressor()
                         xgb_regressor.load_model(model_initialization)
                     else:
                         with open(model_initialization, "rb") as f:
                             xgb_regressor: XGBRegressor = pickle_load(f)
                     self.graph.append(SKRegressorModel(xgb_regressor))
 
                 # Scikit-Learn Interface
                 elif model_type == ModelType.SKLEARN_CLASSIFIER:
                     from cerebrium.models.sklearn import SKClassifierModel
 
+                    try:
+                        from sklearn.base import ClassifierMixin
+                    except ImportError as e:
+                        raise ImportError(
+                            "SciKit-Learn not installed. Please install `scikit-learn` with pip or conda to run this model type."
+                        ) from e
+
                     with open(model_initialization, "rb") as f:
                         sk_classifier: ClassifierMixin = pickle_load(f)
                     self.graph.append(SKClassifierModel(sk_classifier))
 
                 elif model_type == ModelType.SKLEARN:
                     from cerebrium.models.sklearn import SKRegressorModel
 
+                    try:
+                        from sklearn.base import RegressorMixin
+                    except ImportError as e:
+                        raise ImportError(
+                            "SciKit-Learn not installed. Please install `scikit-learn` with pip or conda to run this model type."
+                        ) from e
+
                     with open(model_initialization, "rb") as f:
                         sk_regressor: RegressorMixin = pickle_load(f)
                     self.graph.append(SKRegressorModel(sk_regressor))
 
                 elif model_type == ModelType.SKLEARN_PREPROCESSOR:
                     from cerebrium.models.sklearn import SKPreprocessorModel
 
+                    try:
+                        from sklearn.base import BaseEstimator
+                    except ImportError as e:
+                        raise ImportError(
+                            "SciKit-Learn not installed. Please install `scikit-learn` with pip or conda to run this model type."
+                        ) from e
+
                     with open(model_initialization, "rb") as f:
                         sk_preprocessor: BaseEstimator = pickle_load(f)
                     self.graph.append(SKPreprocessorModel(sk_preprocessor))
 
                 # HuggingFace Pipeline
                 elif model_type == ModelType.HUGGINGFACE_PIPELINE:
                     from cerebrium.models.hf_pipeline import HFPipeline
-                    from transformers.pipelines import pipeline
 
-                    hf_pipeline = HFPipeline(pipeline(**model_initialization))  # type: ignore
+                    try:
+                        from transformers.pipelines import pipeline
+                    except ImportError as e:
+                        raise ImportError(
+                            "Transformers not installed. Please install `transformers` with pip or conda to run this model type."
+                        ) from e
+
+                    hf_pipeline: pipeline = HFPipeline(pipeline(**model_initialization))  # type: ignore
                     self.graph.append(hf_pipeline)
 
             # If there are processors, create a processors.py file with the respective processors
-            # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
-            if self._processors:
-                app_name = os.getenv("APP_NAME", "")
-                assert app_name != "", "APP_NAME environment variable not set"
-                processor_path = (
-                    f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
-                )
-                os.makedirs(processor_path, exist_ok=True)
-                # Create the processors.py file
-                with open(
-                    f"{processor_path}/processors.py",
-                    "w",
-                ) as f:
-                    f.write(
-                        "from cerebrium import save, get, delete, upload\n"
-                        "import numpy as np\n"
-                        "import pandas as pd\n"
-                        "import torch\n"
-                    )
-                    for processors in self._processors:
-                        if processors["pre"]:
-                            source = processors["pre"]
-                            f.write(source)
-                        if processors["post"]:
-                            source = processors["post"]
-                            f.write(source)
-                # Create the __init__.py file
-                with open(
-                    f"{processor_path}/__init__.py",
-                    "w",
-                ) as f:
-                    f.write("from .processors import *\n")
+            # Save the processors.py file in the /usr/local/lib/python3.11/dist-packages/conduit_processors directory
 
+            self.write_processors()
             self.ready = True
 
+    def write_processors(self):
+        if not self._processors:
+            return
+        app_name = os.getenv("APP_NAME", "")
+        assert app_name != "", "APP_NAME environment variable not set"
+        # get python version from the runtime
+        processor_path = f"/miniconda/envs/{app_name}/lib/python3.11/conduit_processors"
+        os.makedirs(processor_path, exist_ok=True)
+        # Create the processors.py file
+        with open(
+            f"{processor_path}/processors.py",
+            "w",
+        ) as f:
+            f.write(
+                "from cerebrium import save, get, delete, upload\n"
+                "import numpy as np\n"
+                "import pandas as pd\n"
+                "import torch\n"
+            )
+            for processors in self._processors:
+                if processors["pre"]:
+                    source = processors["pre"]
+                    f.write(source)
+                if processors["post"]:
+                    source = processors["post"]
+                    f.write(source)
+        # Create the __init__.py file
+        with open(
+            f"{processor_path}/__init__.py",
+            "w",
+        ) as f:
+            f.write("from .processors import *\n")
+
     def run(self, data: Any, files: list = []):
+        # sourcery skip: default-mutable-arg
         """
         Run the Conduit on the given input with the stored computational graph.
 
         Args:
             data (list): The input data to run the Conduit on.
         """
-        from torch import Tensor
+        self.load()
+        try:
+            from numpy import atleast_2d, ndarray
+        except ImportError as e:
+            raise ImportError(
+                "NumPy not installed. Please install `numpy` with pip or conda to run Conduit."
+            ) from e
+        if self.contains_torch_model:
+            try:
+                from torch import Tensor
+            except ImportError as e:
+                raise ImportError(
+                    "PyTorch not installed. Please install `torch` with pip or conda to run Conduit."
+                ) from e
 
         if self._processors:
             # List files in working directory
             files = os.listdir()
             import conduit_processors  # type: ignore
 
         if not self.ready:
             return "Conduit not ready. Conduit components have not been loaded."
-        else:
             # If there is no initial pre-processor, convert the data accordingly
-            if not self.flow[0][2].get("pre", False):
-                if self.flow[0][0] == ModelType.TORCH:
-                    data = Tensor(atleast_2d(data)).to(self.device)
-                elif self.flow[0][0] == ModelType.ONNX:
-                    if isinstance(data, list):
-                        data = data[0]
-                    else:
-                        pass
-                elif self.flow[0][0] == ModelType.HUGGINGFACE_PIPELINE:
-                    pass
-                elif self.flow[0][0] == ModelType.SPACY:
+        if not self.flow[0][2].get("pre", False):
+            if self.flow[0][0] == ModelType.TORCH:
+                # attempt to import Tensor from Torch if it exists
+                data = Tensor(atleast_2d(data)).to(self.device)  # type: ignore
+            elif self.flow[0][0] == ModelType.ONNX:
+                if isinstance(data, list):
                     data = data[0]
-                elif any([isinstance(d, bytes) for d in data]):
-                    pass
+            elif self.flow[0][0] == ModelType.HUGGINGFACE_PIPELINE:
+                pass
+            elif self.flow[0][0] == ModelType.SPACY:
+                data = data[0]
+            elif not any(isinstance(d, bytes) for d in data):
+                data = atleast_2d(data)
+
+        # Set input data
+        input_data = data
+
+        for (model_type, _, processors), (model) in zip(self.flow, self.graph):
+            # Run the preprocessor
+            preprocessor: Union[FunctionType, str] = processors.get("pre", "")
+            postprocessor: Union[FunctionType, str] = processors.get("post", "")
+            if preprocessor:
+                if self._processors:
+                    assert isinstance(preprocessor, str)
+                    preprocessor_function: FunctionType = getattr(conduit_processors, preprocessor)  # type: ignore
                 else:
-                    data = atleast_2d(data)
-
-            # Set input data
-            input_data = data
-
-            for (model_type, _, processors), (model) in zip(self.flow, self.graph):
-                # Run the preprocessor
-                preprocessor: Union[FunctionType, str] = processors.get("pre", "")
-                postprocessor: Union[FunctionType, str] = processors.get("post", "")
-                if preprocessor:
-                    if self._processors:
-                        assert isinstance(preprocessor, str)
-                        preprocessor_function: FunctionType = getattr(conduit_processors, preprocessor)  # type: ignore
-                    else:
-                        assert isinstance(preprocessor, FunctionType)
-                        preprocessor_function: FunctionType = preprocessor
-                    sig = signature(preprocessor_function)
-                    if len(sig.parameters) == 1:
-                        data = preprocessor_function(data)
-                    elif len(sig.parameters) == 2:
-                        data = preprocessor_function(data, files)
-
-                # Ensure that the input data is the correct type
-                if model_type == ModelType.TORCH and not isinstance(data, Tensor):
-                    data = Tensor(data).to(self.device)
-                elif model_type != ModelType.TORCH and isinstance(data, Tensor):
+                    assert isinstance(preprocessor, FunctionType)
+                    preprocessor_function: FunctionType = preprocessor
+                sig = signature(preprocessor_function)
+                if len(sig.parameters) == 1:
+                    data = preprocessor_function(data)
+                elif len(sig.parameters) == 2:
+                    data = preprocessor_function(data, files)
+
+            # Ensure that the input data is the correct type
+            if self.contains_torch_model:
+                if model_type == ModelType.TORCH and not isinstance(data, Tensor):  # type: ignore
+                    data = Tensor(data).to(self.device)  # type: ignore
+                elif model_type != ModelType.TORCH and isinstance(data, Tensor):  # type: ignore
                     data = data.detach().to("cpu").numpy()
 
-                # Run the model
-                data = model.predict(data)
+            # Run the model
+            data = model.predict(data)
 
-                # Run the postprocessor
-                if postprocessor:
-                    if self._processors:
-                        assert isinstance(postprocessor, str)
-                        postprocessor_function = getattr(conduit_processors, postprocessor)  # type: ignore
-                    else:
-                        assert isinstance(postprocessor, FunctionType)
-                        postprocessor_function: FunctionType = postprocessor
-                    sig = signature(postprocessor_function)
-                    if len(sig.parameters) == 1:
-                        data = postprocessor_function(data)
-                    elif len(sig.parameters) == 2:
-                        data = postprocessor_function(data, input_data)
-                    else:
-                        data = postprocessor_function(data, input_data, files)
+            # Run the postprocessor
+            if postprocessor:
+                if self._processors:
+                    assert isinstance(postprocessor, str)
+                    postprocessor_function = getattr(conduit_processors, postprocessor)  # type: ignore
+                else:
+                    assert isinstance(postprocessor, FunctionType)
+                    postprocessor_function: FunctionType = postprocessor
+                sig = signature(postprocessor_function)
+                if len(sig.parameters) == 1:
+                    data = postprocessor_function(data)
+                elif len(sig.parameters) == 2:
+                    data = postprocessor_function(data, input_data)
+                else:
+                    data = postprocessor_function(data, input_data, files)
 
-            # Ensure that final output is a list
-            if isinstance(data, Tensor):
+        # Ensure that final output is a list
+        if self.contains_torch_model:
+            if isinstance(data, Tensor):  # type: ignore
                 data = data.detach().to("cpu").numpy().tolist()
-            elif isinstance(data, ndarray):
-                data = data.tolist()
-            elif not isinstance(data, list) and not isinstance(data, dict):
-                data = [data]
-            return data
+        elif isinstance(data, ndarray):
+            data = data.tolist()
+        elif not isinstance(data, list) and not isinstance(data, dict):
+            data = [data]
+        return data
 
     def add_model(
         self,
         model_type: ModelType,
         model_initialization: Union[str, dict],
         postprocessor: Union[
             Dict[Union[Literal["pre"], Literal["post"]], FunctionType], None
         ] = None,
     ):
         """
         Add a model to the Conduit's computational flow.
         """
         temp_flow = self.flow
-        temp_flow.append((model_type, model_initialization, postprocessor))
+        model = (model_type, model_initialization, postprocessor or {})
+        temp_flow.append(model)  # type: ignore
         self.flow = _check_flow_type(temp_flow)
         self._determine_hardware()
 
     def add_logger(
         self,
         platform: LoggingPlatform,
         platform_authentication: dict,
         features: list,
         targets: list,
         platform_args: dict = {},
         log_ms: bool = False,
-    ):
+    ):  # sourcery skip: default-mutable-arg
         """
         Add a logger to the Conduit's computational flow.
 
         Args:
             platform (LoggingPlatform): The logging platform to use.
             platform_authentication (dict): The authentication credentials for the logging platform.
             features (list): The features to log.
             targets (list): The targets to log.
             platform_args (dict, optional): Any additional arguments to pass to the logger. Defaults to {}.
             log_ms (bool, optional): Whether to log the milliseconds of the input data. Defaults to False.
         """
-        platform = platform.value
-        self.logger_configs[platform] = {
+        self.logger_configs[platform.value] = {
             "platform_authentication": platform_authentication,
             "features": features,
             "targets": targets,
             "platform_args": platform_args,
             "log_ms": log_ms,
         }
 
     def setup_loggers(self):
         """
         Setup the loggers for the Conduit.
         """
         for platform, config in self.logger_configs.items():
             if platform == "Censius":
                 from cerebrium.logging.censius import CensiusLogger
-                from censius import ModelType
 
                 # If there are processors, set the model type to the last model in the flow
                 if self._processors:
                     self.logger_configs[platform]["platform_args"]["model_type"] = eval(
                         config[platform]["platform_args"]["model_type"]
                     )
                 self.loggers["Censius"] = CensiusLogger(
@@ -459,15 +523,15 @@
                                 data=config[platform]["platform_args"]["embedding"][
                                     feature
                                 ]["data"],
                                 vector=Series(
                                     config[platform]["platform_args"]["embedding"][
                                         feature
                                     ]["vector"]
-                                ),
+                                ).to_list(),
                             )
                 self.loggers["Arize"] = ArizeLogger(
                     config["platform_authentication"],
                     self.name,
                     config["features"],
                     config["targets"],
                     config["platform_args"],
@@ -476,30 +540,15 @@
 
     def _jsonify_loggers(self):
         """
         Serialize the loggers to JSON for the Conduit.
         """
         logger_configs = {}
         for platform, config in self.logger_configs.items():
-            if platform == "Censius":
-                from censius import ModelType
-
-                logger_configs[platform] = deepcopy(config)
-                if (
-                    config["platform_args"]["model_type"]
-                    == ModelType.BINARY_CLASSIFICATION
-                ):
-                    logger_configs[platform]["platform_args"][
-                        "model_type"
-                    ] = "ModelType.BINARY_CLASSIFICATION"
-                else:
-                    logger_configs[platform]["platform_args"][
-                        "model_type"
-                    ] = "ModelType.REGRESSION"
-            elif platform == "Arize":
+            if platform == "Arize":
                 logger_configs[platform] = deepcopy(config)
                 logger_configs[platform]["platform_args"]["model_type"] = str(
                     config["platform_args"]["model_type"]
                 )
                 logger_configs[platform]["platform_args"]["metric"] = [
                     str(x) for x in config["platform_args"]["metric"]
                 ]
@@ -531,36 +580,44 @@
                                 "embedding_features"
                             ][feature]["data"],
                             "vector": logger_configs[platform]["platform_args"][
                                 "embedding_features"
                             ][feature]["vector"].tolist(),
                         }
 
+            elif platform == "Censius":
+                from censius import ModelType
+
+                logger_configs[platform] = deepcopy(config)
+                logger_configs[platform]["platform_args"]["model_type"] = (
+                    "ModelType.BINARY_CLASSIFICATION"
+                    if (
+                        config["platform_args"]["model_type"]
+                        == ModelType.BINARY_CLASSIFICATION
+                    )
+                    else "ModelType.REGRESSION"
+                )
         return logger_configs
 
     def create_json_config(self, filename: str):
         """
         Return the Conduit's configuration as a JSON string.
 
         Returns:
             str: The Conduit's configuration as a JSON string.
         """
 
         def get_function_names(
             processors: Dict[Union[Literal["pre"], Literal["post"]], FunctionType]
         ):
             names = {}
-            if "pre" in processors:
-                names["pre"] = processors["pre"].__name__
-            else:
-                names["pre"] = None
-            if "post" in processors:
-                names["post"] = processors["post"].__name__
-            else:
-                names["post"] = None
+            names["pre"] = processors["pre"].__name__ if "pre" in processors else None
+            names["post"] = (
+                processors["post"].__name__ if "post" in processors else None
+            )
             return names
 
         json_flow = [
             (model_type.value, model_initialization, get_function_names(processors))  # type: ignore
             for model_type, model_initialization, processors in self.flow
         ]
         with open(filename, "w") as f:
@@ -571,18 +628,18 @@
                     "api_key": self.api_key,
                     "logger_configs": self._jsonify_loggers(),
                     "version": __version__,
                     "processors": [
                         {
                             "pre": None
                             if p[2].get("pre", None) is None
-                            else getsource(p[2]["pre"]),
+                            else getsource(p[2]["pre"]),  # type: ignore
                             "post": None
                             if p[2].get("post", None) is None
-                            else getsource(p[2]["post"]),
+                            else getsource(p[2]["post"]),  # type: ignore
                         }
                         for p in self.flow
                     ],
                     "hardware": self.hardware.value,
                 },
                 f,
                 indent=2,
@@ -596,139 +653,139 @@
             url (str): The upload URL.
 
         Returns:
             dict ('status_code': int, 'data': dict): The response code and data. 'data' contains the flow token if successful.
         """
         if self.flow == []:
             raise ValueError("Conduit is empty. Please add models to the Conduit.")
-        else:
-            # Clear the graph
-            if self.ready:
-                print("Clearing the Conduit graph...")
-                self.graph = []
-                self.ready = False
-            # Clear the loggers
-            if self.loggers:
-                print("Clearing the Conduit loggers...")
-                self.loggers = {}
+        # Clear the graph
+        if self.ready:
+            print("Clearing the Conduit graph...")
             self.graph = []
             self.ready = False
-            # Create a temporary directory to store the Conduit zip
-            with tempfile.TemporaryDirectory() as tmpdir:
-                # Create a zip file of the Conduit, writing the model files and Conduit object to the zip
-                with zipfile.ZipFile(tmpdir + f"/{self.name}.zip", "w") as zip:
-                    for model_type, model_initialization, _ in self.flow:
-                        if model_type != ModelType.HUGGINGFACE_PIPELINE:
-                            assert isinstance(model_initialization, str)
-                            true_path: str = os.path.abspath(model_initialization)
-                            zip.write(true_path, os.path.basename(true_path))
-                            ## If the model is a spaCy model, write all the folder contents to the zip
-                            ## This is necessary because spaCy models are directories
-                            if model_type == ModelType.SPACY:
-                                for root, _, files in os.walk(true_path):
-                                    for file in files:
-                                        directory = os.path.basename(root)
-                                        if root == true_path:
-                                            directory = ""
-                                        else:
-                                            directory = "/" + os.path.basename(root)
-                                        zip.write(
-                                            os.path.join(root, file),
-                                            os.path.join(
-                                                f"{os.path.basename(true_path)}{directory}",
-                                                file,
-                                            ),
-                                        )
-                    self.create_json_config("conduit.json")
-                    zip.write("conduit.json")
+        # Clear the loggers
+        if self.loggers:
+            print("Clearing the Conduit loggers...")
+            self.loggers = {}
+        self.graph = []
+        self.ready = False
+        # Create a temporary directory to store the Conduit zip
+        with tempfile.TemporaryDirectory() as tmpdir:
+            # Create a zip file of the Conduit, writing the model files and Conduit object to the zip
+            with zipfile.ZipFile(f"{tmpdir}/{self.name}.zip", "w") as zip:
+                for model_type, model_initialization, _ in self.flow:
+                    if model_type != ModelType.HUGGINGFACE_PIPELINE:
+                        assert isinstance(model_initialization, str)
+                        true_path: str = os.path.abspath(model_initialization)
+                        zip.write(true_path, os.path.basename(true_path))
+                        ## If the model is a spaCy model, write all the folder contents to the zip
+                        ## This is necessary because spaCy models are directories
+                        if model_type == ModelType.SPACY:
+                            for root, _, files in os.walk(true_path):
+                                for file in files:
+                                    directory = os.path.basename(root)
+                                    directory = (
+                                        ""
+                                        if root == true_path
+                                        else f"/{os.path.basename(root)}"
+                                    )
+                                    zip.write(
+                                        os.path.join(root, file),
+                                        os.path.join(
+                                            f"{os.path.basename(true_path)}{directory}",
+                                            file,
+                                        ),
+                                    )
+                self.create_json_config("conduit.json")
+                zip.write("conduit.json")
                 # Upload the Conduit zip, chunking with tqdm for progress bar
-                with open(tmpdir + f"/{self.name}.zip", "rb") as f:
-                    headers = {
-                        "Content-Type": "application/zip",
-                    }
-                    with tqdm(
-                        total=os.path.getsize(tmpdir + f"/{self.name}.zip"),
-                        unit="B",
-                        unit_scale=True,
-                        unit_divisor=1024,
-                        colour="#EB3A6F",
-                    ) as pbar:
-                        wrapped_f = CallbackIOWrapper(pbar.update, f, "read")
-                        response = requests.put(
-                            url,
-                            headers=headers,
-                            data=wrapped_f,  # type: ignore
-                            timeout=60,
-                            stream=True,
-                        )
-                    data = {} if not response.text else json.loads(response.text)
-                    return {"status_code": response.status_code, "data": data}
+            with open(f"{tmpdir}/{self.name}.zip", "rb") as f:
+                headers = {
+                    "Content-Type": "application/zip",
+                }
+                with tqdm(
+                    total=os.path.getsize(f"{tmpdir}/{self.name}.zip"),
+                    unit="B",
+                    unit_scale=True,
+                    unit_divisor=1024,
+                    colour="#EB3A6F",
+                ) as pbar:
+                    wrapped_f = CallbackIOWrapper(pbar.update, f, "read")
+                    response = requests.put(
+                        url,
+                        headers=headers,
+                        data=wrapped_f,  # type: ignore
+                        timeout=60,
+                        stream=True,
+                    )
+                data = json.loads(response.text) if response.text else {}
+                return {"status_code": response.status_code, "data": data}
 
-    def deploy(self, dry_run=False) -> str:
+    def deploy(self, dry_run=False) -> Union[str, Self]:
         """
         Deploy the Conduit to Cerebrium.
 
         Returns:
             dict ('status_code': int, 'data': dict): The response code and data. 'data' contains the flow token if successful.
         """
-        # Deploy the conduit
         if not dry_run:
-            # Check that the user is authenticated
-            env = os.getenv("DEVELOPMENT_ENV", "prod")
-            upload_url_response = _cerebrium_request(
-                "deploy",
+            return self.register()
+        if self.flow[0][0] == ModelType.PREBUILT:
+            raise NotImplementedError("Dry run not supported for prebuilt models")
+        self.load(direct_from_flow=True)
+        return self
+
+    def register(self):
+        # Check that the user is authenticated
+        env = os.getenv("DEVELOPMENT_ENV", "prod")
+        upload_url_response = _cerebrium_request(
+            "deploy",
+            "POST",
+            self.api_key,
+            payload={
+                "name": self.name,
+                "cerebrium_version": __version__ if env == "prod" else "0.1.1_dev",
+                "hardware": self.hardware.value.upper(),
+                "source": "conduit",
+            },
+            enable_spinner=(
+                True,
+                ("Authenticating...", "Authenticated with Cerebrium!"),
+            ),
+        )
+        upload_url = upload_url_response["data"]["uploadUrl"]
+        project_id = upload_url_response["data"]["projectId"]
+        build_id = upload_url_response["data"]["buildId"]
+        endpoint = upload_url_response["data"]["internalEndpoint"]
+
+        print(f"🚀 Deploying {self.name}:{build_id} to Cerebrium...")
+
+        # If Prebuilt model, register with modal
+        if self.flow[0][0] == ModelType.PREBUILT:
+            print("Registering with Cerebrium...")
+            prebuilt_model_response = _cerebrium_request(
+                "pre-built-model",
                 "POST",
                 self.api_key,
                 payload={
-                    "name": self.name,
-                    "cerebrium_version": __version__ if env == "prod" else "0.1.1_dev",
-                    "hardware": self.hardware.value.upper(),
-                    "source": "conduit",
+                    "arguments": {
+                        "name": self.name,
+                        "externalId": self.flow[0][1],
+                        "modelType": _flow_string(self.flow),
+                    }
                 },
                 enable_spinner=(
                     True,
-                    ("Authenticating...", "Authenticated with Cerebrium!"),
+                    ("Registering with Cerebrium...", "Registered with Cerebrium!"),
                 ),
             )
-            upload_url = upload_url_response["data"]["uploadUrl"]
-            project_id = upload_url_response["data"]["projectId"]
-            build_id = upload_url_response["data"]["buildId"]
-            endpoint = upload_url_response["data"]["internalEndpoint"]
-
-            print(f"🚀 Deploying {self.name}:{build_id} to Cerebrium...")
-
-            # If Prebuilt model, register with modal
-            if self.flow[0][0] == ModelType.PREBUILT:
-                print("Registering with Cerebrium...")
-                prebuilt_model_response = _cerebrium_request(
-                    "pre-built-model",
-                    "POST",
-                    self.api_key,
-                    payload={
-                        "arguments": {
-                            "name": self.name,
-                            "externalId": self.flow[0][1],
-                            "modelType": _flow_string(self.flow),
-                        }
-                    },
-                    enable_spinner=(
-                        True,
-                        ("Registering with Cerebrium...", "Registered with Cerebrium!"),
-                    ),
-                )
-                endpoint = prebuilt_model_response["data"]["internalEndpoint"]
-                print("🌍 Endpoint:", endpoint)
-                return endpoint
-            else:
-                # Upload the conduit artefacts to Cerebrium
-                print("⬆️  Uploading conduit resources...")
-                self._upload(upload_url)
-                print("✅ Conduit resources uploaded successfully.")
-                _poll_deployment_status(
-                    self.api_key, build_id, self.name, project_id, endpoint
-                )
-                return endpoint
+            endpoint = prebuilt_model_response["data"]["internalEndpoint"]
+            print("🌍 Endpoint:", endpoint)
         else:
-            if self.flow[0][0] == ModelType.PREBUILT:
-                raise NotImplementedError("Dry run not supported for prebuilt models")
-            self.load(direct_from_flow=True)
-            return self
+            # Upload the conduit artefacts to Cerebrium
+            print("⬆️  Uploading conduit resources...")
+            self._upload(upload_url)
+            print("✅ Conduit resources uploaded successfully.")
+            _poll_deployment_status(
+                self.api_key, build_id, self.name, project_id, endpoint
+            )
+        return endpoint
```

### Comparing `cerebrium-1.1.6/cerebrium/core.py` & `cerebrium-1.1.7/cerebrium/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 import json
 import os
-from typing import Union, List
-from uuid import uuid4
-
-import boto3
 import requests
 import yaml
-from numpy import ndarray
-from torch import Tensor
+from typing import Union, List
+from uuid import uuid4
 
 from cerebrium.conduit import Conduit
 from cerebrium.flow import CerebriumFlow
 from cerebrium.requests import _cerebrium_request, ENV
 from cerebrium.utils import _convert_input_data
+from cerebrium.errors import CerebriumError
 
 IS_SERVER = os.getenv("IS_SERVER", "false")
 _objects = {}
 if os.path.exists("secrets.json"):
     with open("secrets.json") as f:
         SECRETS = json.load(f)
 elif os.path.exists("secrets.yaml"):
     with open("secrets.yaml") as f:
         SECRETS = yaml.load(f, Loader=yaml.FullLoader)
 else:
     SECRETS = {}
 
 
 def get_secret(key):
-    if SECRETS:
-        secret = SECRETS.get(key, "")
-    else:
-        secret = os.getenv(key, "")
+    secret = SECRETS.get(key, "") if SECRETS else os.getenv(key, "")
     if secret == "":
-        raise Exception(
+        raise CerebriumError(
             f"Secret not found for key: {key}, please check set your environment variable"
         )
     else:
         return secret
 
 
 def upload(file_name):
     # Upload a file to Cerebrium S3 and return a URL to the file
     from cerebrium.conduit import API_KEY
+    from boto3 import client
 
     if API_KEY and IS_SERVER == "true":
-        s3_client = boto3.client("s3")
-        id = str(uuid4())
+        s3_client = client("s3")
+        file_id = str(uuid4())
         s3_client.upload_file(file_name, f"cerebrium-file-storage-{ENV}", id)
-        # Generate presigned URL to the file
-        url = _cerebrium_request(
+        return _cerebrium_request(
             method="getFileUrl",
             http_method="POST",
             api_key=API_KEY,
-            payload={"file_name": id},
+            payload={"file_name": file_id},
         )
-        return url
     else:
         return file_name
 
 
 def save(name: str, obj: object) -> None:
     """
     Save a Python objec from the current scope to persistent memory so that it can be accessed by processing functions.
@@ -94,17 +87,17 @@
         del _objects[name]
     except KeyError as error:
         raise NameError(f"Object '{name}' not found in persistent memory.") from error
 
 
 def model_api_request(
     model_endpoint: str,
-    data: Union[list, ndarray, Tensor],
+    data: list,
     api_key: str,
-    files: List[bytes] = None,
+    files: Union[List[bytes], None] = None,
 ) -> dict:
     """
     Make a request to the Cerebrium model API.
 
     Args:
         model_endpoint (str): The endpoint of the model to make a request to.
         data (list): The data to send to the model.
@@ -114,17 +107,17 @@
     """
     payload = _convert_input_data(data)
     headers = {
         "Authorization": api_key,
     }
     if files is not None:
         byte_files = {f"file{i}": (f, open(f, "rb")) for i, f in enumerate(files)}
-        byte_files["data"] = (None, json.dumps(payload), "application/json")
+        byte_files["data"] = (None, json.dumps(payload), "application/json")  # type: ignore
         response = requests.request(
-            "POST", model_endpoint, headers=headers, timeout=30, files=byte_files
+            "POST", model_endpoint, headers=headers, timeout=30, files=byte_files  # type: ignore
         )
     else:
         payload = json.dumps(payload)
         headers["Content-Type"] = "application/json"
         response = requests.request(
             "POST", model_endpoint, headers=headers, data=payload, timeout=30
         )
@@ -134,15 +127,15 @@
 def deploy(
     model_flow: CerebriumFlow,
     name: str,
     api_key: str,
     dry_run=False,
     loggers=[],
     hardware=None,
-) -> str:
+) -> Union[str, Conduit]:  # sourcery skip: default-mutable-arg
     """
     Deploy a model to Cerebrium.
 
     Args:
         model_flow (CerebriumFlow): The flow to deploy. This is a list of ModelType, model path and postprocessor tuples, as such:
             [(ModelType.TORCH, "model.pt", postprocess_f)]
         name (str): The name to deploy the flow under.
```

### Comparing `cerebrium-1.1.6/cerebrium/errors.py` & `cerebrium-1.1.7/cerebrium/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
     Args:
         status_code (int): The status code returned from the Cerebrium API.
         endpoint (str): The endpoint that was called.
     """
 
     def __init__(self, status_code, endpoint, data={}):
+        # sourcery skip: default-mutable-arg
         self.status_code = status_code
         self.endpoint = endpoint
         self.data = data
         super().__init__(self.status_code)
 
     def __str__(self):
         msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed.\n{self.data}."
 
         if self.status_code == 401:
             msg = f"{self.status_code}\n`{self.endpoint} API key does not exist or is incorrect. If your key is correct, please contact the Cerebrium team."
         elif self.status_code == 403:
-            plan_limits = self.data.get("planLimits")
-            if plan_limits:
+            if plan_limits := self.data.get("planLimits"):
                 can_deploy_model = plan_limits.get("canDeployModel")
                 number_of_plan_models = plan_limits.get("numberOfPlanModels")
                 upgrade_link = plan_limits.get("upgradeLink")
                 if not can_deploy_model:
                     msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. You have exceeded your model deployment limit of {number_of_plan_models}."
                     if upgrade_link:
                         msg += f" Please upgrade your plan to continue using Cerebrium at `{upgrade_link}`"
@@ -39,15 +39,15 @@
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Internal Server Error: {self.data}."
         elif self.status_code == 502:
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Bad Gateway."
 
         return msg
 
 
-class CerebriumDeploymentError(Exception):
+class CerebriumError(Exception):
     """
     Class to handle the error code messages from the Cerebrium API.
 
     Args:
         status_code (int): The status code returned from the Cerebrium API.
         endpoint (str): The endpoint that was called.
     """
```

### Comparing `cerebrium-1.1.6/cerebrium/flow.py` & `cerebrium-1.1.7/cerebrium/flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Tuple, List, Dict, Literal, Union
 
 from cerebrium.models.base import ModelType
 
 CerebriumModel = Tuple[
     ModelType,
     Union[str, dict],
-    Union[Dict[Union[Literal["pre"], Literal["post"]], FunctionType], None],
+    Dict[Union[Literal["pre"], Literal["post"]], Union[FunctionType, str]],
 ]
 CerebriumFlow = List[CerebriumModel]
 
 
 def _flow_string(flow: CerebriumFlow):
     """
     Convert a flow to a string.
@@ -81,19 +81,18 @@
 
     Args:
         model_flow: The model flow to check.
 
     Returns:
         A boolean indicating whether the model flow is a special model.
     """
-    if model_flow[0][0] == ModelType.PREBUILT:
-        if len(model_flow) != 1:
-            raise TypeError(
-                f"Prebuilt models must be a tuple or list of length 1, but is {len(model_flow)}"
-            )
+    if model_flow[0][0] == ModelType.PREBUILT and len(model_flow) != 1:
+        raise TypeError(
+            f"Prebuilt models must be a tuple or list of length 1, but is {len(model_flow)}"
+        )
 
 
 def _check_valid_model(
     model_type: ModelType,
     model_initialization: Union[str, dict],
     pipeline_position: int,
 ):
@@ -108,121 +107,99 @@
     # Check typing
     if not isinstance(model_type, ModelType):
         raise TypeError(
             f"Model {pipeline_position}: model_type must be of type ModelType, but is {type(model_type)}. Please ensure you use a valid Cerebrium typing."
         )
 
     # Check the length of the prebuilt model flow is 1
-    if pipeline_position > 0:
-        if model_type == ModelType.PREBUILT:
-            raise TypeError(
-                f"Model {pipeline_position}: Prebuilt models can only be used as the first model in a pipeline."
-            )
+    if pipeline_position > 0 and model_type == ModelType.PREBUILT:
+        raise TypeError(
+            f"Model {pipeline_position}: Prebuilt models can only be used as the first model in a pipeline."
+        )
 
     # Check valid model params
     if (
         model_type == ModelType.HUGGINGFACE_PIPELINE
         and not isinstance(model_initialization, dict)
         and ("task" not in model_initialization or "model" not in model_initialization)
     ):
         raise TypeError(
             f"Model {pipeline_position}: For {model_type}, `model_initialization` must be a dictionary and contain at least one of the keys 'task' or 'model', but is {model_initialization}"
         )
     elif model_type == ModelType.PREBUILT and not isinstance(model_initialization, str):
         raise TypeError(
             f"Model {pipeline_position}: For {model_type}, model_initialization must be a valid Cerebrium pre-built model string, but is {model_initialization}"
         )
+    elif model_type == ModelType.ONNX:
+        assert isinstance(model_initialization, str)
+        if not model_initialization.endswith(".onnx"):
+            raise TypeError(
+                f"Model {pipeline_position}: {model_type} `model_initialization` file type must be `.onnx`, but is {model_initialization.split('.')[-1]}"
+            )
     elif model_type != ModelType.HUGGINGFACE_PIPELINE and not isinstance(
         model_initialization, str
     ):
         raise TypeError(
             f"Model {pipeline_position}: For {model_type}, model_initialization must be a file path of type `str`, but is {type(model_initialization)}"
         )
-    elif (
-        model_type != ModelType.HUGGINGFACE_PIPELINE
-        and not Path(model_initialization).exists()
-    ):
-        raise TypeError(
-            f"Model {pipeline_position}: For {model_type}, `model_initialization` must be be a valid file path, but is {model_initialization}"
-        )
-    elif (
-        model_type == ModelType.TORCH
-        and not model_initialization.endswith(".pt")
-        and not model_initialization.endswith(".pkl")
-    ):
-        raise TypeError(
-            f"Model {pipeline_position}: For {model_type}, `model_initialization` file type must be either `.pt` for Torchscript models or `pkl` for pickled models, but is {model_initialization.split('.')[-1]}"
-        )
-    elif model_type == ModelType.ONNX and not model_initialization.endswith(".onnx"):
-        raise TypeError(
-            f"Model {pipeline_position}: {model_type} `model_initialization` file type must be `.onnx`, but is {model_initialization.split('.')[-1]}"
-        )
-    elif (
-        model_type == ModelType.SKLEARN_CLASSIFIER or model_type == ModelType.SKLEARN
-    ) and not model_initialization.endswith(".pkl"):
-        raise TypeError(
-            f"Model {pipeline_position}: {model_type} `model_initialization` file type must be `.pkl`, but is {model_initialization.split('.')[-1]}"
-        )
-    elif (
-        (
-            model_type == ModelType.XGBOOST_CLASSIFIER
-            or model_type == ModelType.XGBOOST_REGRESSOR
-        )
-        and not model_initialization.endswith(".pkl")
-        and not model_initialization.endswith(".json")
-    ):
-        raise TypeError(
-            f"Model {pipeline_position}: {model_type} `model_initialization` file type must be either `.pkl` or `.json`, but is {model_initialization.split('.')[-1]}"
-        )
-    elif model_type == ModelType.SPACY:
-        if model_initialization.endswith("/"):
-            model_initialization = model_initialization[:-1]
-        if (
-            Path(model_initialization + "/ner").exists()
-            and not Path(model_initialization + "/tok2vec").exists()
-            and not Path(model_initialization + "/vocab").exists()
-            and not Path(model_initialization + "/config.cfg").exists()
-            and not Path(model_initialization + "/meta.json").exists()
-            and not Path(model_initialization + "/tokenizer").exists()
-        ):
+    elif model_type != ModelType.HUGGINGFACE_PIPELINE:
+        assert isinstance(model_initialization, str)
+        if not Path(model_initialization).exists():
             raise TypeError(
-                f"Model {pipeline_position}: model_initialization must be be a valid spaCy folder. Make sure the folder contains the following folders/files: ner, tok2vec, vocab, config.cfg, meta.json, tokenizer."
+                f"Model {pipeline_position}: For {model_type}, `model_initialization` must be be a valid file path, but is {model_initialization}"
+            )
+    elif model_type in [
+        ModelType.SKLEARN_CLASSIFIER,
+        ModelType.SKLEARN,
+    ]:
+        assert isinstance(model_initialization, str)
+        if not model_initialization.endswith(".pkl"):
+            raise TypeError(
+                f"Model {pipeline_position}: {model_type} `model_initialization` file type must be `.pkl`, but is {model_initialization.split('.')[-1]}"
+            )
+    elif model_type in [ModelType.XGBOOST_CLASSIFIER, ModelType.XGBOOST_REGRESSOR]:
+        assert isinstance(model_initialization, str)
+        if not model_initialization.endswith(
+            ".pkl"
+        ) and not model_initialization.endswith(".json"):
+            raise TypeError(
+                f"Model {pipeline_position}: {model_type} `model_initialization` file type must be either `.pkl` or `.json`, but is {model_initialization.split('.')[-1]}"
             )
-
     return model_type, model_initialization
 
 
-def _check_processor(processor: FunctionType, pipeline_position: int, stage: str):
+def _check_processor(
+    processor: Union[FunctionType, str], pipeline_position: int, stage: str
+):
     """
     Check that the postprocessor is valid, raising an error if not.
 
     Args:
         processor: The processor function.
         pipeline_position: The position of the post-processor in the pipeline.
     """
     if not isinstance(processor, FunctionType) and processor is not None:
         raise TypeError(
             f"Model {pipeline_position}: The post-processing function must be of type FunctionType, but is {type(processor)}"
         )
-    else:
-        if processor is not None:
-            processor_str = getsource(processor).replace("\t", "    ").split("\n")
-            processor_args = _get_function_arg(processor_str[0])
-            if processor_args[0] == "":
-                processor_args = []
-            if len(processor_args) == 0 or len(processor_args) >= 4:
-                raise NotImplementedError(
-                    f"Model {processor}: The {stage}-processing function must have between 1 and 3 arguments, but has {len(processor_args)}"
-                )
+    if processor is not None:
+        processor_str = getsource(processor).replace("\t", "    ").split("\n")
+        processor_args = _get_function_arg(processor_str[0])
+        if processor_args[0] == "":
+            processor_args = []
+        if len(processor_args) == 0 or len(processor_args) >= 4:
+            raise NotImplementedError(
+                f"Model {processor}: The {stage}-processing function must have between 1 and 3 arguments, but has {len(processor_args)}"
+            )
 
-            contains_return = [s.strip()[:6] == "return" for s in processor_str]
-            if not any(contains_return):
-                raise NotImplementedError(
-                    f"Model {processor}: The {stage}-processing function must return a value, but does not."
-                )
+        contains_return = [s.strip()[:6] == "return" for s in processor_str]
+        if not any(contains_return):
+            raise NotImplementedError(
+                f"Model {processor}: The {stage}-processing function must return a value, but does not."
+            )
 
 
 def _check_flow_type(model_flow: Union[CerebriumFlow, CerebriumModel]) -> CerebriumFlow:
     """
     Check if the given model_flow is a valid CerebriumFlow.
 
     Args:
@@ -252,15 +229,15 @@
         model_type, model_initialization = _check_valid_model(
             flow_component[0], flow_component[1], i
         )
         if len(flow_component) == 3:
             if not isinstance(flow_component[2], dict):
                 # Assume a post-process function, backwards compatibility
                 _check_processor(flow_component[2], i, "post")
-                model_flow[i] = (
+                model_flow[i] = (  # type: ignore
                     model_type,
                     model_initialization,
                     {"post": flow_component[2]},
                 )
             else:
                 # Check if the processing functions are valid
                 keys = set(flow_component[2].keys())
```

### Comparing `cerebrium-1.1.6/cerebrium/logging/arize.py` & `cerebrium-1.1.7/cerebrium/logging/arize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import numpy as np
-import pandas as pd
-from arize.pandas.logger import Client
-from arize.utils.types import ModelTypes, Environments
 from tenacity import retry, stop_after_attempt, wait_fixed
+from typing import Tuple
 
 from cerebrium.logging.base import ConduitLogger
 
 
 class ArizeLogger(ConduitLogger):
     def __init__(
         self,
@@ -21,35 +18,44 @@
             platform_authentication,
             platform_model_id,
             features,
             targets,
             platform_args,
             log_ms,
         )
-
+        try:
+            from arize.pandas.logger import Client
+            from arize.utils.types import Environments
+        except ImportError as e:
+            raise ImportError(
+                "Arize is not installed. Please install `arize` with pip or conda to use this logger."
+            ) from e
         self.space_key = platform_authentication["space_key"]
         self.api_key = platform_args["api_key"]
         self.model_type = platform_args["model_type"]
         self.features = platform_args["features"]
         self.schema = platform_args["schema"]
         self.metrics_validation = platform_args.get("metrics_validation", [])
         self.environment = platform_args.get("environment", Environments.PRODUCTION)
         self.platform_args = platform_args
         self.client = Client(space_key=self.space_key, api_key=self.api_key)
 
-    def check_ready(self, model_version: str, model_name: str) -> str:
+    def check_ready(self, model_version: str, model_name: str) -> Tuple[str, bool]:
         self.model_name = model_name
         self.model_version = model_version
 
         return "", True
 
     @retry(wait=wait_fixed(60), stop=stop_after_attempt(5))
     async def log(self, data: list, predictions: list, prediction_id: str):
         df = {label: data[i] for i, label in enumerate(self.features)}
         df["prediction_id"] = prediction_id
+        import numpy as np
+        import pandas as pd
+        from arize.utils.types import ModelTypes
 
         if self.model_type == ModelTypes.BINARY_CLASSIFICATION:
             df["prediction"] = np.argmax(predictions)
 
         elif self.model_type == ModelTypes.REGRESSION:
             df["prediction"] = predictions[0]
 
@@ -59,18 +65,17 @@
                 df["prediction"] = self.platform_args["class_labels"][
                     np.argmax(predictions)
                 ]
 
             if "embedding_features" in self.platform_args:
                 df["embedding_features"] = self.platform_args["embedding_features"]
 
-        response = self.client.log(
+        return self.client.log(
             model_id=self.model_name,
             model_version=self.model_version,
             model_type=self.model_type,
             metrics_validation=self.metrics_validation,
             environment=self.environment,
-            dataframe=pd.DataFrame([df], columns=df.keys()),
+            dataframe=pd.DataFrame([df], columns=list(df.keys())),
             schema=self.schema,
             sync=True,
         )
-        return response
```

### Comparing `cerebrium-1.1.6/cerebrium/logging/base.py` & `cerebrium-1.1.7/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.6/cerebrium/logging/censius.py` & `cerebrium-1.1.7/cerebrium/logging/censius.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from time import time
-
-import numpy as np
 from tenacity import retry, stop_after_attempt, wait_fixed
+from typing import Tuple
 
-from censius import CensiusClient, ModelType
 from cerebrium.logging.base import ConduitLogger
 
 
 class CensiusLogger(ConduitLogger):
     def __init__(
         self,
         platform_authentication: dict,
@@ -21,22 +19,27 @@
             platform_authentication,
             platform_model_id,
             features,
             targets,
             platform_args,
             log_ms,
         )
-
+        try:
+            from censius import CensiusClient
+        except ImportError as e:
+            raise ImportError(
+                "Censius is not installed. Please install `censius` with pip or conda to use this logger."
+            ) from e
         self.tenant_id = platform_authentication["tenant_id"]
         self.project_id = platform_args["project_id"]
         self.training_info = platform_args["training_info"]
         self.model_type = platform_args["model_type"]
         self.client = CensiusClient(api_key=self.api_key, tenant_id=self.tenant_id)
 
-    def check_ready(self, model_version: str, model_name: str) -> str:
+    def check_ready(self, model_version: str, model_name: str) -> Tuple[str, bool]:
         self.model_name = model_name
         self.model_version = model_version
         response = self.client.register_new_model_version(
             model_id=model_name,
             model_version=model_version,
             targets=self.targets,
             features=self.features,
@@ -71,29 +74,31 @@
             response_msg = f"Registered new model version {model_name}@{model_version} with Censius@{self.project_id}."
         else:
             response_msg = f"Unable to register new model version for {model_name} with Censius@{self.project_id}."
         return response_msg, self.ready
 
     @retry(wait=wait_fixed(60), stop=stop_after_attempt(5))
     async def log(self, data: list, predictions: list, prediction_id: str):
+        import numpy as np
+        from censius import ModelType
+
         timestamp = round(time()) if self.log_ms else round(time() * 1000)
         feature_dict = {label: data[i] for i, label in enumerate(self.features)}
-        prediction_dict = {}
-        for i, t in enumerate(self.targets):
-            if self.model_type == ModelType.BINARY_CLASSIFICATION:
-                prediction_dict[t] = {
-                    "label": int(np.argmax(predictions[i])),
-                    "confidence": float(np.max(predictions[i])),
-                }
-            else:
-                prediction_dict[t] = {
-                    "value": predictions[i],
-                }
-        response = self.client.log(
+        prediction_dict = {
+            t: {
+                "label": int(np.argmax(predictions[i])),
+                "confidence": float(np.max(predictions[i])),
+            }
+            if self.model_type == ModelType.BINARY_CLASSIFICATION
+            else {
+                "value": predictions[i],
+            }
+            for i, t in enumerate(self.targets)
+        }
+        return self.client.log(
             model_id=self.model_name,
             model_version=self.model_version,
             features=feature_dict,
             prediction=prediction_dict,
             timestamp=timestamp,
             prediction_id=prediction_id,
         )
-        return response
```

### Comparing `cerebrium-1.1.6/cerebrium/requests.py` & `cerebrium-1.1.7/cerebrium/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import os
 import re
 import time
-from typing import Tuple, Union
-
 import requests
+from typing import Tuple, Union
 from tenacity import retry, stop_after_delay, wait_fixed
 from termcolor import colored
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
-from cerebrium.errors import CerebriumRequestError, CerebriumDeploymentError
+from cerebrium.errors import CerebriumRequestError, CerebriumError
 
 ENV = os.getenv("ENV", "prod")
 if ENV == "dev":
     print("Using development environment")
     BASE_CEREBRIUM_URL = "https://dev-rest-api.cerebrium.ai"
     DASHBOARD_URL = "https://dev-dashboard.cerebrium.ai"
     TRAINING_URL = "http://dev-training-api.cerebrium.ai/"
@@ -127,52 +126,48 @@
                 headers={"Authorization": api_key},
             )
             if build_status_response.status_code != 200:
                 print(
                     "API request failed with status code:",
                     build_status_response.status_code,
                 )
-                raise CerebriumDeploymentError(
+                raise CerebriumError(
                     build_status_response.text,
                 )
             else:
                 build_status = build_status_response.json()["status"]
-                response_logs = build_status_response.json()["logs"]
-                if response_logs:
-                    concat_logs = "".join(response_logs)
-                    logs = concat_logs.split("\n")[:-1]
-                else:
+                if not (response_logs := build_status_response.json()["logs"]):
                     continue
 
+                concat_logs = "".join(response_logs)
+                logs = concat_logs.split("\n")[:-1]
                 for message in logs[seen_index:]:
                     if message:
                         match = re.match(
                             r"^(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{9})Z ", message
                         )
                         if (
                             match is not None
                         ):  # If the regex matches the beginning of the string
-                            created = match.group(
-                                1
-                            )  # The first group is the creation time
+                            created = match[1]
                             message = message[len(created) + 2 :]
                         spinner.write(f"{message}")
                     else:
                         spinner.write("\n")
                 seen_index = len(logs)
                 spinner.text = f"🔨 Building... Status: {build_status}"
                 time.sleep(1)
             if time.time() - t1 > 600:
                 spinner.fail("Build timed out.")
-                raise CerebriumDeploymentError(
+                raise CerebriumError(
                     "Deployment Timed Out. Your conduit might be large and take longer to deploy. Please try again later."
                 )
             elif build_status == "failed":
                 spinner.fail("Build failed.")
-                raise CerebriumDeploymentError(
+                raise CerebriumError(
                     "Deployment Failed. Please check your conduit and try again."
                 )
         spinner.text = f"Status: {build_status}"
         spinner.ok("🚀 Build complete!")
         print("\n🌍 Endpoint:", endpoint)
         print("💡 You can call the endpoint with the following curl command:")
         print(
@@ -204,25 +199,26 @@
 
     Returns:
         str: The endpoint of the deployed model.
     """
     # Check the status of the deployment by polling the Cerebrium API for deployment status
     with yaspin(
         spinner=Spinners.arc, text="Checking deployment status...", color="magenta"
-    ) as spinner:
+    ) as _:
         response = _cerebrium_request(
             "checkDeploymentStatus",
+            "POST",
             api_key,
             payload={"arguments": {"name": training_name}},
         )
     if response["data"]["status"] == "deployed":
         endpoint = response["data"]["endpoint"]
         print("✅ FineTuning deployed!")
         return endpoint
     elif response["data"]["status"] == "failed":
         print("❌ FineTuning deployment failed.")
-        raise CerebriumDeploymentError(response["data"]["failureMessage"])
+        raise CerebriumError(response["data"]["failureMessage"])
     else:
         print("⏳ FineTuning deployment in progress...")
-        raise CerebriumDeploymentError(
+        raise CerebriumError(
             "Deployment Not Complete. Your conduit might be large and take longer to deploy. Please try again later."
         )
```

### Comparing `cerebrium-1.1.6/cerebrium/trainer/README.md` & `cerebrium-1.1.7/cerebrium/trainer/README_Transformers.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # Contents
 
 - [Contents](#contents)
 - [Introduction](#introduction)
 - [Using the fine-tuner](#using-the-fine-tuner)
   - [Curating a dataset](#curating-a-dataset)
   - [Deploying a finetuning job](#deploying-a-finetuning-job)
@@ -83,34 +84,39 @@
 cerebrium download-model <<JOB_ID>> <<API_KEY>>
 ```
 
 This will return a zip file which contains your **adapter** and **adapter config** which should be in the order of 10MB for your 7B parameter model due to the extreme efficiency of PEFT fine-tuning.
 
 
 # Using your Fine-tuned Adaptor
-Using your adapter can be done simply with:
+Using your adapter can be done simply by adding two lines as shown here:
 
 ```python
-  from transformers import AutoModelForSeq2SeqLM
-+ from peft import PeftModel, PeftConfig
+  from transformers import AutoModelForCausalLM
+  from peft import PeftModel, PeftConfig # Add the peft libraries we need for the adapter
 
   peft_model_id = "path/toYourAdapter"
   config = PeftConfig.from_pretrained(peft_model_id)
-  model = AutoModelForSeq2SeqLM.from_pretrained(config.base_model_name_or_path)
-+ model = PeftModel.from_pretrained(model, peft_model_id)
+  model = AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path)
+  model = PeftModel.from_pretrained(model, peft_model_id) # Add the adapter to the model
   tokenizer = AutoTokenizer.from_pretrained(config.base_model_name_or_path)
 
-  # Now just inference your model as you normally would.
-  model = model.to(device)
-  model.eval()
-  inputs = tokenizer("Insert your prompt matching the training template here:", return_tensors="pt")
+  model = model.to("cuda")
+  model.eval() # set the model to inference mode
+
+```
+
+Now for inference, you just need to place the prompt into the template used for training. In this example we do it as follows
+``` python
+  template =  "### Instruction:\n{instruction}\n\n### Response:\n"
+  question = template.format(instruction=prompt) 
+  inputs = tokenizer(question, return_tensors="pt")
 
   with torch.no_grad():
     outputs = model.generate(input_ids=inputs["input_ids"].to("cuda"), max_new_tokens=10)
     print(tokenizer.batch_decode(outputs.detach().cpu().numpy(), skip_special_tokens=True)[0])
 
-
 ```
 
 These adapters can be combined with others when using your model at inference time.  
 For more information, see
 [Using Adapter Transformers at Hugging Face](https://huggingface.co/docs/hub/adapter-transformers#exploring-adaptertransformers-in-the-hub)
```

### Comparing `cerebrium-1.1.6/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.1.7/cerebrium/trainer/fine_tuner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,81 @@
 import hashlib
-import json
 import os
 import sys
 import tempfile
+import yaml
 import zipfile
 from copy import copy
-
+from typing import Optional
 import requests
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
-from transformers import (
-    TrainingArguments,
-)
 
 from cerebrium import __version__
 from cerebrium.requests import _cerebrium_request
-from cerebrium.trainer.finetuning_model import FineTuningModel
-from cerebrium.trainer.userDataset.base_dataset import FineTuningDataset
+from cerebrium.trainer.finetune_LLM.finetuning_model import FineTuningModel
+from cerebrium.trainer.finetune_LLM.userDataset.base_dataset import FineTuningDataset
 
 
 class FineTuner:
     def __init__(
         self,
-        api_key: str,
-        experiment_name: str,
-        hf_model_path: str,
-        dataset_path: str,
-        model_type: str = "AutoModelForCausalLM",
-        custom_tokenizer: str = "",
-        base_model_kwargs: dict = {},
-        peft_lora_kwargs: dict = {},
-        training_kwargs: dict = {},
-        dataset_kwargs: dict = {},
-        seed: int = 42,
-        verbose=False,
+        name: str,
+        config: dict = {},
+        config_yaml_path: Optional[str] = None,
+        log_level: str = "INFO",
     ):
-        """An object for finetuning transformers on Cerebrium to improve the perfromance of Large Language Models towards your task.
+        """An object for finetuning transformers on Cerebrium to improve the perfromance of Large Language Models towards your task."""
+        # check either config or config_yaml_path is provided
+        assert (
+            config or config_yaml_path
+        ), "Either config or config_yaml_path must be provided."
+        # load config
+        if config_yaml_path:
+            with open(config_yaml_path, "r") as f:
+                self.config = yaml.safe_load(f).update(config)
+        else:
+            self.config = config
 
+        self.config["training_type"] = "transformer"
+        self.config["name"] = name
 
-        Args:
-            experiment_name (str): The unique name you would like to use to refer to your training. Will be used as the model name for deploying to cerebrium.
-            hf_model_path (str): The path to the model on huggingface.
-            dataset_path (str): Path of your local dataset.json file.
-            model_type (str, optional): Type of model to use. Defaults to "AutoModelForCausalLM".
-            custom_tokenizer (str, optional): If you need something other than "AutoTokenizer for your model. Defaults to "".
-            base_model_kwargs (dict, optional): Any kwargs you need to send to from_pretrained(). Defaults to {}.
-            peft_lora_kwargs (dict, optional): Kwargs to be fed into LoraConfig(), eg. lora rank. Defaults to {}.
-            training_kwargs (dict, optional): Any custom training args you have. Defaults to {}.
-            dataset_kwargs (dict, optional): Additional kwargs to be parsed into the FineTuningDataset. Defaults to {}.
-            seed (int, optional): Pytorch seed. Defaults to 42.
-            verbose (bool, optional): _description_. Defaults to False.
-        """
+        # override with log_level from params
+        self.config["log_level"] = log_level or self.config["log_level"]
+        if (
+            str.find(self.config["hf_model_path"], "llama") != -1
+        ):  # if llama model, use llama tokenizer. This seems to have broken in the latest huggingface release
+            self.config["custom_tokenizer"] = "LlamaTokenizer"
 
-        self.name = experiment_name
-        self.api_key = api_key
-        self.seed = seed
-        self.verbose = verbose
-        self.dataset_path = dataset_path
-        self.hf_model_path = hf_model_path
-        self.user_base_model_kwargs = copy(base_model_kwargs)
-        self.user_peft_kwargs = copy(peft_lora_kwargs)
+        # backup for user to see what they sent
+        self.config["user_base_model_kwargs"] = copy(self.config["base_model_args"])
+        self.config["user_peft_kwargs"] = copy(self.config["peft_lora_args"])
 
         # will set to our defaults. Easier for beginners.
         # Calling here so that a user can access the defaults and check them before training.
-        self.user_training_kwargs = training_kwargs
 
-        self.finetuning_model = FineTuningModel(
-            hf_base_model_path=hf_model_path,
-            model_type=model_type,
-            base_model_kwargs=base_model_kwargs,
-            lora_kwargs=peft_lora_kwargs,
-            verbose=self.verbose,
+        if self.config["log_level"].upper() == "DEBUG":
+            print("Training args set to:")
+            args = self.get_training_arguments(self.config["training_args"])
+            print(args.to_json_string())
+
+        self.config["finetuning_model"] = FineTuningModel(
+            hf_base_model_path=self.config["hf_model_path"],
+            model_type=self.config["model_type"],
+            base_model_kwargs=self.config["base_model_args"],
+            lora_kwargs=self.config["peft_lora_args"],
         )
-        self.custom_tokenizer = custom_tokenizer
-        if (
-            str.find(self.hf_model_path, "llama") != -1
-        ):  # if llama model, use llama tokenizer. This seems to have broken in the latest huggingface release
-            self.custom_tokenizer = "LlamaTokenizer"
 
-        self.dataset = FineTuningDataset(
-            dataset_path=dataset_path, verbose=self.verbose, **dataset_kwargs
+        self.config["dataset"] = FineTuningDataset(
+            dataset_path=self.config["dataset_path"],
+            verbose=self.config["log_level"],
+            **self.config["dataset_args"],
         )
 
-    def TrainingArguments(self, training_kwargs: dict = {}) -> TrainingArguments:
+    def get_training_arguments(self, training_kwargs: dict = {}):
         """A utility function to create training arguments for user inspection.
         A set of default training arguments is used if none are provided
 
         Args:
             logging_steps (int, optional): Steps between logging. Defaults to 10.
             per_device_batch_size (int, optional): Batch size. Defaults to 15.
             warmup_steps (int, optional): Warmup before beginning training. Defaults to 50.
@@ -95,15 +84,22 @@
             learning_rate (float, optional): Initial learning rate. Defaults to 3e-4.
             group_by_length (bool, optional): Defaults to False.
 
 
         Returns:
             TrainingArguments: _description_
         """
-
+        try:
+            from transformers import (
+                TrainingArguments,
+            )
+        except ImportError as e:
+            raise ImportError(
+                "Transformers not installed. Please install `transformers` with pip or conda to run this model type."
+            ) from e
         defaults = {
             "logging_steps": 10,
             "per_device_train_batch_size": 15,
             "per_device_eval_batch_size": 15,
             "warmup_steps": 0,
             "gradient_accumulation_steps": 4,
             "num_train_epochs": 3,
@@ -116,74 +112,80 @@
             if k not in training_kwargs:
                 training_kwargs[k] = v
 
         return TrainingArguments(
             **training_kwargs,
         )
 
-    def create_json_config(self, filename="finetune.json"):
+    def create_yaml_config(self, filename="finetune.yaml"):
         # Quick json serialiser. Dumps all the variables as a config
-        config_dict = self.__dict__.copy()
+        config_dict = self.config.copy()
         config_dict["finetuning_model"] = config_dict["finetuning_model"].to_dict()
         config_dict["dataset"] = config_dict["dataset"].to_dict()
 
         with open(filename, "w") as f:
-            json.dump(config_dict, fp=f, indent=2, sort_keys=True)
+            # json.dump(config_dict, fp=f, indent=2, sort_keys=True)
+            yaml.dump(config_dict, f, sort_keys=False, version=(1, 2))
 
-    def _upload(self, init_debug=False, pre_init_debug=False, log_level="INFO"):
+    def _upload(
+        self, api_key, init_debug=False, pre_init_debug=False, log_level="INFO"
+    ):  # sourcery skip: extract-method
         dataset_hash = "DATASET_FILE_DOESNT_EXIST"
 
         # Calc MD5 hash of user's dataset
         assert os.path.exists(
-            self.dataset_path
+            self.config["dataset_path"]
         ), "Dataset file cannot be found. Please check the path you have entered!"
-        with open(self.dataset_path, "rb") as f:
+        with open(self.config["dataset_path"], "rb") as f:
             dataset_hash = hashlib.md5(f.read()).hexdigest()
         # Hit the deploy endpoint to get the upload URL
         upload_url_response = _cerebrium_request(
             method="train",
             http_method="POST",
-            api_key=self.api_key,
+            api_key=api_key,
             payload={
-                "name": self.name,
-                "hf_model_path": self.hf_model_path,
+                "name": self.config["name"],
+                "hf_model_path": self.config["hf_model_path"],
                 "hardware": "A10",
                 "init_debug": init_debug,
                 "pre_init_debug": pre_init_debug,
                 "log_level": log_level,
                 "cerebrium_version": __version__,
                 "dataset_hash": dataset_hash,
             },
         )
         if upload_url_response["status_code"] != 200 or (
             upload_url_response["data"].get("uploadUrl", None) is None
         ):
             print(
-                "API request failed with status code:",
+                "❌ API request failed with status code:",
                 upload_url_response["status_code"],
             )
             print("Error getting upload URL:", upload_url_response["data"]["message"])
             sys.exit(1)
         upload_url = upload_url_response["data"]["uploadUrl"]
         job_id = upload_url_response["data"]["jobId"]
 
-        print(f"Job ID: {job_id}")
+        print(f"⚙️ Job ID: {job_id}")
         # Zip all files in the current directory and upload to S3
-        print("Zipping files...")
+        print("📦 Zipping files...")
         with tempfile.TemporaryDirectory() as temp_dir:
-            zip_path = os.path.join(temp_dir, f"{self.name}.zip")
+            zip_path = os.path.join(temp_dir, f"{self.config['name']}.zip")
             dir_name = os.path.dirname(zip_path)
             os.makedirs(dir_name, exist_ok=True)
             # Create a zip file containing the config files and upload them.
             with zipfile.ZipFile(
-                os.path.join(temp_dir, f"{self.name}.zip"), "w"
+                os.path.join(temp_dir, f"{self.config['name']}.zip"), "w"
             ) as zip:
-                self.create_json_config("finetune_config.json")
-                zip.write("finetune_config.json")
-                zip.write(self.dataset_path, "dataset.json")
+                config_file = os.path.join(
+                    temp_dir, f"{self.config['name']}_finetune_config.yaml"
+                )
+                self.create_yaml_config(filename=config_file)
+                zip.write(config_file, arcname="finetune_config.yaml")
+                zip.write(self.config["dataset_path"], arcname="dataset.json")
 
             print("⬆️  Uploading to Cerebrium...")
             with open(zip_path, "rb") as f:
                 headers = {
                     "Content-Type": "application/zip",
                 }
                 with tqdm(
@@ -202,15 +204,15 @@
                         stream=True,
                     )
                 if upload_response.status_code != 200:
                     print(
                         "API request failed with status code:",
                         upload_response.status_code,
                     )
-                    print("Error uploading to Cerebrium:", upload_response.text)
+                    print("❌ Error uploading to Cerebrium:", upload_response.text)
                     raise Exception("Error uploading to Cerebrium")
                 else:
-                    print(f"✅ Resources uploaded successfully for {job_id}.")
+                    print(f"✅ Resources uploaded successfully for {job_id}")
             print(
-                "You can query the training status with `cerebrium get-training-jobs <API_KEY>` \n",
-                "Your training logs can be found at `cerebrium get-training-logs <JOB_ID> <API_KEY>` ",
+                f"You can query the training status with `cerebrium get-training-jobs --api-key {api_key}` \n",
+                f"Your training logs can be found at `cerebrium get-training-logs {job_id} --api-key {api_key}` ",
             )
```

### Comparing `cerebrium-1.1.6/cerebrium/trainer/finetuning_model.py` & `cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from typing import Union
 
-import transformers
-
 
 class FineTuningModel:
     def __init__(
         self,
         hf_base_model_path: str,
         model_type: str = "AutoModelForCausalLM",
         lora_kwargs: Union[dict, None] = None,
         base_model_kwargs: Union[dict, None] = None,
-        verbose: bool = False,
     ):
         if lora_kwargs is None:
             lora_kwargs = {}
         if base_model_kwargs is None:
             base_model_kwargs = {}
 
         self.model_type = model_type
+        try:
+            import transformers
+        except ImportError as e:
+            raise ImportError(
+                "Transformers not installed. Please install `transformers` with pip or conda to run this model type."
+            ) from e
         assert hasattr(
             transformers, model_type
         ), f"Model type {model_type} not found in transformers library. Please check your spelling and try again."
         self.hf_base_model_path = hf_base_model_path
         self.lora_kwargs = lora_kwargs
         self.base_model_kwargs = base_model_kwargs
         self.init_kwargs()
```

### Comparing `cerebrium-1.1.6/cerebrium/trainer/userDataset/base_dataset.py` & `cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,44 @@
-from typing import Union
-
 from .data_validator import Dataset_Validator
 
 
 class FineTuningDataset:
     # TODO Docstrings
-    def __init__(
-        self,
-        dataset_path,
-        verbose: bool = False,
-        hf_dataset_kwargs: Union[dict, None] = None,
-        **kwargs
-    ):
+    def __init__(self, dataset_path, verbose: bool = False, **kwargs):
         """Base dataset class for fine-tuning using the Cerebrium package.
         Your dataset is loaded and run through a sanity check to ensure that it is ready for training.
 
         Args:
             dataset_path (str): path to the JSON/JSONL file on your system that contains your fine-tuning data.
-            input_column (str, optional): Name of the input column in your dataset. Defaults to "prompt".
+            instruction_column (str, optional): Name of the input column in your dataset. Defaults to "prompt".
             label_column (str, optional): Name of the label column in your dataset. Defaults to "completion".
             context_column (str, optional): Name of the context column in your dataset . Defaults to "context".
             prompt_template (str): The template to be used for finetuning. Can be {"short", "long"} or a string to format. E.g f"###My Question\n{input}\n\n###Models Answer\n" which will be formatted with your input data.
             cutoff_len (int, optional): Maximum length to cut inputs to. Defaults to 512.
             train_val_ratio (float, optional): Ratio between train and validation data for splits. Defaults to 0.9.
             custom_schema (dict, optional): Custom jsonschema for validating your dataset. Defaults to None
             verbose (bool, optional): Verbose prints. Defaults to False
         """
         self.dataset_path = dataset_path
 
         # validator
         self.verbose = kwargs.get("verbose", False)
 
         self.prompt_template = kwargs.get("prompt_template", "")
-        self.input_column = kwargs.get("input_column", "prompt")
+        self.instruction_column = kwargs.get("instruction_column", "prompt")
         self.label_column = kwargs.get("label_column", "completion")
         self.context_column = kwargs.get("context_column", "context")
         self.cutoff_len = kwargs.get("cutoff_len", 512)
         self.train_val_ratio = kwargs.get("train_val_ratio", 0.9)
-        self.verbose = verbose
+        self.verbose = verbose  # override with verbose from params
 
         self.custom_schema = kwargs.get("custom_schema", None)
         # validate file before training
         validator = Dataset_Validator(
-            prompt_column=self.input_column,
+            prompt_column=self.instruction_column,
             context_column=self.context_column,
             label_column=self.label_column,
             custom_schema=self.custom_schema,
             verbose=self.verbose,
         )
 
         assert validator(
```

### Comparing `cerebrium-1.1.6/cerebrium/trainer/userDataset/data_validator.py` & `cerebrium-1.1.7/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Union
-
-import pandas as pd
 from jsonschema import Draft202012Validator
 
 
 # class to perform validation
 class Dataset_Validator:
     """
     Class to check JSON dataset and ensure the data is labeled for training.
@@ -55,25 +53,24 @@
             self.schema = custom_schema
 
         Draft202012Validator.check_schema(self.schema)
         self.validator = Draft202012Validator(self.schema)
 
     def __call__(
         self, filename: Path, return_dataframe: bool = False
-    ) -> Union[pd.DataFrame, bool]:
+    ):
         # Check if the file exists
         assert os.path.exists(filename), f"The file '{filename}' could not be found"
         if self.verbose:
             print("Found dataset file.")
 
-        df_data = self.load_json_file(filename=filename)
-
         # Check the json is valid for training.
-        if self.is_valid_for_training(df=df_data):
-            return df_data if return_dataframe else True
+        if return_dataframe:
+            df_data = self.load_json_file(filename=filename)
+            return df_data if self.is_valid_for_training(df=df_data) else True
         else:
             return False
 
     def is_valid_for_training(self, df) -> bool:
         if self.verbose:
             print(f"Found {len(df)} data entries")
         for _, row in df.iterrows():
@@ -81,15 +78,21 @@
             pt = row.to_json()
             self.validator.validate(pt)
 
         if self.verbose:
             print("All entries in the dataset passed validation ✅")
         return True
 
-    def load_json_file(self, filename) -> pd.DataFrame:
+    def load_json_file(self, filename):
+        try:
+            import pandas as pd
+        except ImportError as error:
+            print("Pandas is required for loading JSON files. Please install 'pandas' with pip or conda.")
+            raise error
+        
         extension = os.path.splitext(filename)[1]
 
         if extension in {".json", ".jsonl"}:
             if extension == ".jsonl":
                 self.pd_json_kwargs["orient"] = "records"
             if self.verbose:
                 print(f"Reading in JSON file at {filename}")
```

### Comparing `cerebrium-1.1.6/PKG-INFO` & `cerebrium-1.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,34 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.6
+Version: 1.1.7
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: onnxruntime
-Provides-Extra: onnxruntime-gpu
-Provides-Extra: tensorflow
-Provides-Extra: worker
-Requires-Dist: Pillow (>=9.4,<10.0.0) ; extra == "worker"
-Requires-Dist: accelerate (>=0.18.0,<0.19.0) ; extra == "worker"
-Requires-Dist: arize (>=6.0.2,<7.0)
-Requires-Dist: bitsandbytes (>=0.38.0,<0.39.0) ; extra == "worker"
-Requires-Dist: boto3 (>=1.26)
-Requires-Dist: celery (>=5.2.0,<5.3.0) ; extra == "worker"
-Requires-Dist: censius (>=1.6,<2.0)
-Requires-Dist: chitra (>=0.2.0,<0.3.0) ; extra == "worker"
-Requires-Dist: cloudpickle (>=2.0,<2.1)
-Requires-Dist: datadog (>=0.45.0,<0.51.0) ; extra == "worker"
-Requires-Dist: datasets (>=2.10.0,<2.11.0) ; extra == "worker"
-Requires-Dist: ddtrace (>=1.10.0,<1.11.0) ; extra == "worker"
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: monitoring
+Requires-Dist: arize (>=6.0.2) ; extra == "monitoring"
+Requires-Dist: censius (>=1.6,<2.0) ; extra == "monitoring"
+Requires-Dist: cloudpickle (>=2.2)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
-Requires-Dist: keras (>=2.12.0) ; extra == "tensorflow"
-Requires-Dist: loguru (>=0.6) ; extra == "worker"
-Requires-Dist: numpy (>=1.20,<2.0)
-Requires-Dist: onnxruntime (>=1.13,<2.0) ; extra == "onnxruntime"
-Requires-Dist: onnxruntime-gpu (>=1.14,<2.0) ; extra == "onnxruntime-gpu"
-Requires-Dist: pandas (>=1.5,<3.0)
-Requires-Dist: requests (>=2.28,<3.0)
-Requires-Dist: scikit-learn (>=1.2,<2.0)
-Requires-Dist: spacy (>=3.5.0,<4.0.0)
+Requires-Dist: loguru (>=0.7)
+Requires-Dist: pandas (>=1.5,<3.0) ; extra == "monitoring"
+Requires-Dist: prodict (>=0.8.18,<0.9.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.30,<3.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
-Requires-Dist: tensorflow (>=2.12.0) ; extra == "tensorflow"
-Requires-Dist: torch (>=1.13,<3.0)
 Requires-Dist: tqdm (>=4.64,<4.65)
-Requires-Dist: transformers (>=4.26,<5.0)
-Requires-Dist: typer[all] (==0.7.0)
-Requires-Dist: xformers (>=0.0.16) ; extra == "worker"
-Requires-Dist: xgboost (>=1.7,<2.0)
+Requires-Dist: typer[all] (>=0.7.0)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
 Description-Content-Type: text/markdown
 
 # Cerebrium
```

