# Comparing `tmp/swanapi-0.2.1-py3-none-any.whl.zip` & `tmp/swanapi-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 15835 bytes, number of entries: 17
+Zip file size: 17232 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      157 b- defN 23-Jul-11 00:16 swanapi/__init__.py
 -rw-r--r--  2.0 unx     8931 b- defN 23-Jul-11 01:15 swanapi/base_inference.py
 -rw-r--r--  2.0 unx     1831 b- defN 23-Jul-11 00:57 swanapi/base_requests.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
--rw-r--r--  2.0 unx     2769 b- defN 23-Jul-11 00:45 swanapi/server.py
+-rw-r--r--  2.0 unx     2746 b- defN 23-Jul-11 03:40 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     3953 b- defN 23-Jul-11 07:06 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-Jul-11 07:27 swanapi/docker_builder/cuda_container.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
--rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
+-rw-r--r--  2.0 unx     1901 b- defN 23-Jul-11 07:25 swanapi/docker_builder/runner.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 01:19 swanapi/utils/__init__.py
 -rw-r--r--  2.0 unx    15239 b- defN 23-Jul-11 00:31 swanapi/utils/utils.py
--rw-r--r--  2.0 unx      340 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1384 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/RECORD
-17 files, 40882 bytes uncompressed, 13551 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx      368 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/RECORD
+18 files, 45269 bytes uncompressed, 14792 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -18,35 +18,38 @@
 
 Filename: swanapi/docker_builder/__init__.py
 Comment: 
 
 Filename: swanapi/docker_builder/config.py
 Comment: 
 
+Filename: swanapi/docker_builder/cuda_container.py
+Comment: 
+
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
 Filename: swanapi/utils/__init__.py
 Comment: 
 
 Filename: swanapi/utils/utils.py
 Comment: 
 
-Filename: swanapi-0.2.1.dist-info/METADATA
+Filename: swanapi-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.2.1.dist-info/WHEEL
+Filename: swanapi-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.2.1.dist-info/entry_points.txt
+Filename: swanapi-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.2.1.dist-info/top_level.txt
+Filename: swanapi-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.2.1.dist-info/RECORD
+Filename: swanapi-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/server.py

```diff
@@ -1,15 +1,13 @@
 from flask import Flask, request
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 from .utils import utils
 from .base_inference import BaseInference
 import json
 
-import time
-
 app = Flask("SwanAPI Server")
 
 
 class SwanInference(BaseInference):
     """
     我们将分为两个生命周期：
     1. Backbone: 以fn, inputs和outputs为基础，构建一个推理骨架
@@ -17,16 +15,16 @@
     """
 
     def __init__(self):
         super().__init__()
 
     def inference(self,
                   fn: Callable,
-                  inputs: Union[list[str], str, None] = None,
-                  outputs: Union[list[str], str, None] = None,
+                  inputs: Union[list, str, None] = None,
+                  outputs: Union[list, str, None] = None,
                   description: str = None
                   ) -> None:
         """
         用户构建backbone的入口函数
         """
         self.fn = fn
         self.backbone_inputs = inputs
```

## swanapi/docker_builder/config.py

```diff
@@ -52,22 +52,24 @@
     def config_predict_handle(self):
         self.predict_cli = "predict.py"
         self.predict_host = "0.0.0.0"
         self.predict_port_typecheck()
 
     def build_gpu_typecheck(self) -> None:
         GPU_LIST = ['false', 'true']
-        GPU_DEFAULT = "false"
+        GPU_INPUT = str(self.config_buid["gpu"]).lower()
         if 'gpu' in self.config_buid:
-            if str(self.config_buid["gpu"]).lower() not in GPU_LIST:
-                raise TypeError("[Error] 'gpu' in swan.yaml is not bool")
+            if GPU_INPUT not in GPU_LIST:
+                raise TypeError(
+                    "[Error] 'gpu' in swan.yaml 必须是 'true' 或 'false'"
+                )
             else:
-                self.gpu = self.config_buid["gpu"]
+                self.gpu = True if GPU_INPUT == 'true' else False
         else:
-            self.gpu = GPU_DEFAULT
+            self.gpu = False
 
     def build_system_packages_typecheck(self) -> None:
         if 'system_packages' in self.config_buid:
             self.system_packages = self.config_buid["system_packages"]
         else:
             self.system_packages = None
```

## swanapi/docker_builder/runner.py

```diff
@@ -1,11 +1,12 @@
 import os
 import subprocess
 from .config import SwanYaml
 from .generate_dockerfile import DockerfileBuild
+from .cuda_container import NVDetection, GPUCommad
 
 
 class Runner:
     """
     SwanAPI深度学习镜像构建的入口类
     """
 
@@ -16,21 +17,32 @@
     def build(self, image_name: str, running=False, save=False) -> None:
         """
         构建镜像并运行服务。
         :param image_name: 构建的镜像Tag名
         :param running: 构建完成后是否运行容器
         :param save: 构建完成后是否保留Dockerfile
         """
-        print("--> Building Docker Image...")
+        print("--> Building Docker Start.")
+        if self.config.gpu:
+            print("--> Detecting GPU...")
+            nv = NVDetection()
+            gc = GPUCommad(nv)
+            gpu_cmd = gc.get_gpu_command()
+            with open("script.sh", "w") as f:
+                f.write(gpu_cmd)
+            print("--> Install Nvidia Docker Requirements...")
+            cmd = ["sh", "script.sh"]
+            subprocess.run(cmd)
 
         # 将生成的Dockerfile写入当前目录
         with open("Dockerfile", "w") as f:
             f.write(self.dockerfile)
 
         # 命令：镜像构建
+        print("--> Building Docker Image...")
         cmd = ["docker", "build", "-t", "{}".format(image_name), "."]
         subprocess.run(cmd)
 
         # 如果不保存，在本地目录删除Dockerfile文件
         if not save:
             os.remove("Dockerfile")
```

## Comparing `swanapi-0.2.1.dist-info/RECORD` & `swanapi-0.2.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 swanapi/__init__.py,sha256=2N4vWNDaCYewP1euHTVKHE1zmtStmsi0af6S-lu8Bs0,157
 swanapi/base_inference.py,sha256=QlWvZI1rpff8pdcMLQ-AKDBHbAIKulXDXJd2I6TAnJw,8931
 swanapi/base_requests.py,sha256=kpGxsP26WgZG7SroPCoDZl_7fjsgHmXOSFHGKbCnozc,1831
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
-swanapi/server.py,sha256=eLtrZmN0RU9RP9Yzh7z33lqkzaZerylNHAVhYXxkr4E,2769
+swanapi/server.py,sha256=AuVDQd_AJbBejrYT5MY5R0NIM64_9QWMCUhqzfUH0Vw,2746
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
+swanapi/docker_builder/config.py,sha256=oMHdFbV8zGzlsIfMjPT1PimM1t6LLnkEIuKxEpjiANM,3953
+swanapi/docker_builder/cuda_container.py,sha256=M0nMeGXwhKCQ1XdqaBNVO3tshEs6d4pwY8HkcXC3FpM,3739
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
-swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
+swanapi/docker_builder/runner.py,sha256=rHLlSWqyJkXfWbSIBJGTWfiqtzsOdXYQZrHR0OoUAh8,1901
 swanapi/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/utils/utils.py,sha256=jx9anz_ty9T1FAJRAT8eLlsKoCOGha4CsPzKa2plK50,15239
-swanapi-0.2.1.dist-info/METADATA,sha256=8tapJs7f6UhkO3VOqSjhI2pRDoR1okRjIDqAebc-A7s,340
-swanapi-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.2.1.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.2.1.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.2.1.dist-info/RECORD,,
+swanapi-0.2.3.dist-info/METADATA,sha256=kUaOrop9Pnmzvf6mAI02y8BSlMoJgI6ORSoKYeBcxl4,368
+swanapi-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.2.3.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.2.3.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.2.3.dist-info/RECORD,,
```

