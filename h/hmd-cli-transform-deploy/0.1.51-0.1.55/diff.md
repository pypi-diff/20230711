# Comparing `tmp/hmd_cli_transform_deploy-0.1.51-py3-none-any.whl.zip` & `tmp/hmd_cli_transform_deploy-0.1.55-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6571 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/__init__.py
--rw-rw-rw-  2.0 unx     6538 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/controller.py
--rw-rw-rw-  2.0 unx     9551 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
--rw-rw-rw-  2.0 unx     2804 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       25 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      664 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/RECORD
-7 files, 19674 bytes uncompressed, 5365 bytes compressed:  72.7%
+Zip file size: 7106 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/__init__.py
+-rw-rw-rw-  2.0 unx     6704 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/controller.py
+-rw-rw-rw-  2.0 unx    11962 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
+-rw-rw-rw-  2.0 unx     2804 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       25 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/RECORD
+7 files, 22252 bytes uncompressed, 5900 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_transform_deploy/controller.py
 Comment: 
 
 Filename: hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.51.dist-info/METADATA
+Filename: hmd_cli_transform_deploy-0.1.55.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.51.dist-info/WHEEL
+Filename: hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.51.dist-info/top_level.txt
+Filename: hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.51.dist-info/RECORD
+Filename: hmd_cli_transform_deploy-0.1.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_transform_deploy/controller.py

```diff
@@ -1,11 +1,11 @@
 import json
 from cement import Controller, ex
 from importlib.metadata import version
-from hmd_cli_tools.hmd_cli_tools import get_standard_parameters
+from hmd_cli_tools.hmd_cli_tools import get_standard_parameters, load_hmd_env
 
 VERSION_BANNER = """
 hmd  version: {}
 """
 
 VERSION = version("hmd_cli_transform_deploy")
 
@@ -93,14 +93,15 @@
             result = do_deploy(**args)
             print(result)
         except Exception as e:
             print(f"Error deploying transform: {e}")
 
     @ex(help="list all deployed transforms", arguments=get_standard_parameters())
     def get_transforms(self):
+        load_hmd_env(override=False)
         hmd_region = self.app.pargs.hmd_region
         cust_code = self.app.pargs.customer_code
         environment = self.app.pargs.environment
 
         from .hmd_cli_transform_deploy import get_transforms as do_get_transforms
 
         result = do_get_transforms(
@@ -125,14 +126,15 @@
                     "action": "store",
                     "dest": "transform_name",
                 },
             ),
         ],
     )
     def load_local(self):
+        load_hmd_env(override=False)
         project_name = self.app.pargs.project
         transform_name = self.app.pargs.transform_name
 
         from .hmd_cli_transform_deploy import load as do_load
 
         result = do_load(project_name, transform_name)
 
@@ -156,14 +158,15 @@
                     "action": "store",
                     "dest": "run_params",
                 },
             ),
         ],
     )
     def run_transforms(self):
+        load_hmd_env(override=False)
         hmd_region = self.app.pargs.hmd_region
         cust_code = self.app.pargs.customer_code
         environment = self.app.pargs.environment
         transform_names = self.app.pargs.transform_names
         run_params = self.app.pargs.run_params
 
         if run_params is not None:
@@ -191,14 +194,15 @@
                     "dest": "instance_nid",
                     "required": True,
                 },
             ),
         ],
     )
     def get_logs(self):
+        load_hmd_env(override=False)
         hmd_region = self.app.pargs.hmd_region
         cust_code = self.app.pargs.customer_code
         environment = self.app.pargs.environment
         instance_nid = self.app.pargs.instance_nid
 
         from .hmd_cli_transform_deploy import get_instance_logs as do_get_logs
```

## hmd_cli_transform_deploy/hmd_cli_transform_deploy.py

```diff
@@ -1,10 +1,11 @@
 # Implement the lifecycle commands here
 import json
 import os
+import subprocess
 from time import sleep
 from typing import Any, Dict, List
 from hmd_cli_tools.hmd_cli_tools import (
     get_deployer_target_session,
     get_neuronsphere_domain,
 )
 from hmd_lib_transform.hmd_lib_transform import HmdLibTransform
@@ -20,14 +21,42 @@
 # Grab hostname for locally running NeuronSphere
 # This should only be set when running Robot Integration tests.
 LOCALHOST = os.environ.get("HMD_NEURONSPHERE_LOCALHOST", "localhost")
 
 LOCAL_URL = f"http://{LOCALHOST}/hmd_ms_transform/"
 
 
+def run_image_sequence(img_seq: list):
+    input_path = os.getcwd()
+    output_path = os.getcwd()
+
+    for img in img_seq:
+        img_name = img["image_name"]
+
+        base_cmd = f"docker run -v {input_path}:/hmd_transform/input -v {output_path}:/hmd_transform/output -e HMD_AUTH_TOKEN={get_auth_token()} "
+
+        for k, v in img["env"].items():
+            if v == "default":
+                v = os.environ.get(k, v)
+            base_cmd += f"-e {k}={v} "
+
+        base_cmd += f"{img_name} "
+
+        if len(img["cmd"]) > 0:
+            base_cmd += f"{' '.join(img['cmd'])} "
+
+        if len(img["args"]) > 0:
+            base_cmd += f"{' '.join(img['args'])}"
+
+        retcode = subprocess.run(base_cmd, shell=True)
+
+        if retcode.returncode != 0:
+            raise Exception(f"Error running {img['name']} image")
+
+
 def get_transform_client(
     hmd_region: str,
     cust_code: str,
     environment: str,
 ):
     base_url = LOCAL_URL if environment == "local" else None
     auth_token = get_auth_token()
@@ -205,45 +234,77 @@
         return
 
     selected_transforms = result.get("transform_names", transform_names)
 
     transform_run = {t.split("@")[0]: {} for t in selected_transforms}
 
     for tf in transform_run.keys():
+        tf_config = transform_client.base_client.invoke_custom_operation(
+            "apiop/get_transform_config", {"transform": {"name": tf}}, "POST"
+        )
         if run_params is None:
             questions = []
-            tf_config = transform_client.base_client.invoke_custom_operation(
-                "apiop/get_transform_config", {"transform": {"name": tf}}, "POST"
-            )
-            questions.append(
-                {
-                    "type": "input",
-                    "name": "run_params",
-                    "message": "Run Paramaters:",
-                    "default": json.dumps(tf_config.get("run_params", {}), indent=2),
-                    "multiline": True,
-                }
-            )
+            if "image_sequence" in tf_config:
+                for index, img in enumerate(tf_config["image_sequence"]):
+                    questions.append(
+                        {
+                            "type": "input",
+                            "name": f"container_env_{index}",
+                            "message": f"Container {index} Env:",
+                            "default": json.dumps(img.get("env", {}), indent=2),
+                            "multiline": True,
+                        }
+                    )
+            else:
+                questions.append(
+                    {
+                        "type": "input",
+                        "name": "run_params",
+                        "message": "Run Paramaters:",
+                        "default": json.dumps(
+                            tf_config.get("run_params", {}), indent=2
+                        ),
+                        "multiline": True,
+                    }
+                )
 
             result = prompt(questions)
-            if result.get("run_params") is None:
-                return
-            run_params = json.loads(result.get("run_params"))
-            transform_run[tf] = run_params
-            run_params = None
+            if "image_sequence" in tf_config:
+                for index, img in enumerate(tf_config["image_sequence"]):
+                    if result.get(f"container_env_{index}") is None:
+                        return
+                    env = json.loads(result.get(f"container_env_{index}"))
+                    tf_config["image_sequence"][index]["env"] = env
+
+                transform_run[tf] = tf_config["image_sequence"]
+            else:
+                if result.get("run_params") is None:
+                    return
+                run_params = json.loads(result.get("run_params"))
+                transform_run[tf] = run_params
+                run_params = None
         else:
+            if "image_sequence" in tf_config:
+                envs = run_params
+                for index, env in enumerate(envs):
+                    tf_config["image_sequence"][index]["env"] = env
+                transform_run[tf] = tf_config["image_sequence"]
+                continue
             transform_run[tf] = run_params
 
     if transform_names is None:
         transform_names = transform_run.keys()
 
     retry = []
     scheduled = []
     retried = []
     for name in transform_names:
+        if isinstance(transform_run[name], list):
+            run_image_sequence(transform_run[name])
+            continue
         print(f"Running: {name}, {json.dumps(transform_run[name])}")
         inst = transform_client.run_provider_transform(name, transform_run[name])
         if inst["status"] == "scheduling_failed":
             print(f"{name} failed to schedule.")
             retry.append(name)
         else:
             scheduled.append(
```

## Comparing `hmd_cli_transform_deploy-0.1.51.dist-info/METADATA` & `hmd_cli_transform_deploy-0.1.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-transform-deploy
-Version: 0.1.51
+Version: 0.1.55
 Summary: Command for deploying transforms
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
@@ -26,23 +26,23 @@
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
-Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.228)
-Requires-Dist: hmd-entity-storage (~=0.1.224)
-Requires-Dist: hmd-graphql-client (~=0.1.105)
+Requires-Dist: hmd-cli-app (~=1.1.597)
+Requires-Dist: hmd-cli-tools (~=1.1.229)
+Requires-Dist: hmd-entity-storage (~=0.1.225)
+Requires-Dist: hmd-graphql-client (~=0.1.106)
 Requires-Dist: hmd-lang-naming (~=0.1.12)
 Requires-Dist: hmd-lib-auth (~=0.1.75)
-Requires-Dist: hmd-lib-librarian-client (~=0.1.53)
-Requires-Dist: hmd-lib-naming (~=0.2.32)
-Requires-Dist: hmd-lib-transform (~=0.1.51)
+Requires-Dist: hmd-lib-librarian-client (~=0.1.54)
+Requires-Dist: hmd-lib-naming (~=0.2.34)
+Requires-Dist: hmd-lib-transform (~=0.1.52)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
@@ -52,15 +52,15 @@
 Requires-Dist: markupsafe (==2.1.0)
 Requires-Dist: multidict (==6.0.2)
 Requires-Dist: nest-asyncio (==1.5.4)
 Requires-Dist: oauthlib (==3.2.2)
 Requires-Dist: okta-jwt-verifier (==0.2.3)
 Requires-Dist: pfzy (==0.3.4)
 Requires-Dist: prompt-toolkit (==3.0.38)
-Requires-Dist: psycopg2-binary (==2.9.3)
+Requires-Dist: psycopg2-binary (==2.9.6)
 Requires-Dist: py (==1.11.0)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: pyasn1-modules (==0.2.8)
 Requires-Dist: pyjwt (==2.6.0)
 Requires-Dist: pyrsistent (==0.18.1)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-dotenv (==0.19.2)
```

## Comparing `hmd_cli_transform_deploy-0.1.51.dist-info/RECORD` & `hmd_cli_transform_deploy-0.1.55.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 hmd_cli_transform_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hmd_cli_transform_deploy/controller.py,sha256=uvp1ptZ7kC4fuwokVr_cWruaZge0Ctw2NpNcw1I5xQE,6538
-hmd_cli_transform_deploy/hmd_cli_transform_deploy.py,sha256=xWIuqzZSEB8h7L93YmPCfRhNMq451AeSv8RtMK_uh2c,9551
-hmd_cli_transform_deploy-0.1.51.dist-info/METADATA,sha256=mV0GmR9yFa1-hq9L7ezVH8VZ2HiVRhBdpRI3bXWWROI,2804
-hmd_cli_transform_deploy-0.1.51.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_cli_transform_deploy-0.1.51.dist-info/top_level.txt,sha256=DtG3sPNzAAQxAwWUR3qMTktl02xogyG5ckfqXQEDusU,25
-hmd_cli_transform_deploy-0.1.51.dist-info/RECORD,,
+hmd_cli_transform_deploy/controller.py,sha256=4UWXypCi-SOGm9u983yGUrqzvLY0jlk5yN0zSDtFaR8,6704
+hmd_cli_transform_deploy/hmd_cli_transform_deploy.py,sha256=-Qcy3-d1Tq0I_opUl_MEfhe3fBHXdLLkGgno0NuApIw,11962
+hmd_cli_transform_deploy-0.1.55.dist-info/METADATA,sha256=3y4vjjDCvW69Bq8qNhtqaOjdeLetHU9F9KsJPPgGUyk,2804
+hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt,sha256=DtG3sPNzAAQxAwWUR3qMTktl02xogyG5ckfqXQEDusU,25
+hmd_cli_transform_deploy-0.1.55.dist-info/RECORD,,
```

