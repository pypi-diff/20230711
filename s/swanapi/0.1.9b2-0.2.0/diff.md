# Comparing `tmp/swanapi-0.1.9b2-py3-none-any.whl.zip` & `tmp/swanapi-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11147 bytes, number of entries: 15
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-10 19:07 swanapi/__init__.py
--rw-r--r--  2.0 unx    10349 b- defN 23-Jul-10 20:37 swanapi/base_inference.py
+Zip file size: 10878 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      157 b- defN 23-Jul-11 00:16 swanapi/__init__.py
+-rw-r--r--  2.0 unx     8931 b- defN 23-Jul-11 01:15 swanapi/base_inference.py
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-11 00:57 swanapi/base_requests.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
--rw-r--r--  2.0 unx     2759 b- defN 23-Jul-10 19:56 swanapi/server.py
+-rw-r--r--  2.0 unx     2769 b- defN 23-Jul-11 00:45 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      349 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1228 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/RECORD
-15 files, 26139 bytes uncompressed, 9105 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      340 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1225 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/RECORD
+15 files, 25484 bytes uncompressed, 8840 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,46 +1,46 @@
 Filename: swanapi/__init__.py
 Comment: 
 
 Filename: swanapi/base_inference.py
 Comment: 
 
+Filename: swanapi/base_requests.py
+Comment: 
+
 Filename: swanapi/make_build.py
 Comment: 
 
 Filename: swanapi/server.py
 Comment: 
 
 Filename: swanapi/swan_types.py
 Comment: 
 
-Filename: swanapi/utils.py
-Comment: 
-
 Filename: swanapi/docker_builder/__init__.py
 Comment: 
 
 Filename: swanapi/docker_builder/config.py
 Comment: 
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.9b2.dist-info/METADATA
+Filename: swanapi-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.9b2.dist-info/WHEEL
+Filename: swanapi-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.9b2.dist-info/entry_points.txt
+Filename: swanapi-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.9b2.dist-info/top_level.txt
+Filename: swanapi-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.9b2.dist-info/RECORD
+Filename: swanapi-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .server import SwanInference
-from .base_inference import SwanRequests
+from .base_requests import SwanRequests
 from .swan_types import Files
 
 __all__ = ["SwanInference", "SwanRequests", "Files"]
```

## swanapi/base_inference.py

```diff
@@ -1,15 +1,13 @@
-from .utils import check_elements_in_list, is_float, is_list, is_dict
+from .utils import utils
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 import inspect
 import numpy as np
-import cv2
-import base64
-import requests
-from .swan_types import Files
+from PIL import Image as _Image
+from pathlib import Path
 
 
 class BaseInference:
     def __init__(self):
         # self.mode's options - ["both", "input_only", "output_only"]
         self.mode = "both"
         self.fn = None
@@ -57,20 +55,20 @@
         if not isinstance(self.backbone_inputs, list):
             self.backbone_inputs = [self.backbone_inputs]
         if not isinstance(self.backbone_outputs, list):
             self.backbone_outputs = [self.backbone_outputs]
 
         # 类型检查: 输入的类型是否在self.types_list中
         if self.mode == "both":
-            assert check_elements_in_list(self.backbone_inputs, self.types_list)
-            assert check_elements_in_list(self.backbone_outputs, self.types_list)
+            assert utils.check_elements_in_list(self.backbone_inputs, self.types_list)
+            assert utils.check_elements_in_list(self.backbone_outputs, self.types_list)
         elif self.mode == "input_only":
-            assert check_elements_in_list(self.backbone_inputs, self.types_list)
+            assert utils.check_elements_in_list(self.backbone_inputs, self.types_list)
         else:
-            assert check_elements_in_list(self.backbone_outputs, self.types_list)
+            assert utils.check_elements_in_list(self.backbone_outputs, self.types_list)
 
     def backbone_get_fn_parameters(self) -> None:
         # 使用inspect库，得到fn函数的签名变量
         signature = inspect.signature(self.fn)
 
         # 得到fn函数的参数名列表，形如["input_image", "input_text"]
         self.fn_param_names = [param for param in signature.parameters]
@@ -92,146 +90,102 @@
         # self.requests_inputs - 用户输入的完整json字典
         self.requests_inputs = requests_inputs
         # 获取网络请求的参数个数
         self.requests_inputs_param_names = list(self.requests_inputs.keys())
         # 判断网络请求输入的参数的个数是否与inputs定义的个数一致
         assert len(self.requests_inputs_param_names) == len(self.backbone_inputs), "请求传入的参数数量与inputs定义的不一致"
         # 判断网络请求输入的参数名是否与fn定义的一致
-        assert check_elements_in_list(self.requests_inputs_param_names, self.fn_param_names), "请求传入的参数key与fn定义的不一致"
+        assert utils.check_elements_in_list(self.requests_inputs_param_names, self.fn_param_names), "请求传入的参数key与fn定义的不一致"
 
     def requests_input_converter(self) -> None:
         # 对于每一个requests内容的输入类型，做相应的转换
         for iter, param_name in enumerate(self.fn_param_names):
             # param_name : 'input_image', 'custom_size_height', 'custom_size_width'
             # 获取内容values
             values = self.requests_inputs[param_name]
             # 对于输入的类型为image的情况
             if self.backbone_inputs[iter] == "image":
+                # 如果输入的是字节流，则使用imdecode解码图像
                 if isinstance(values, bytes):
-
-                    self.requests_inputs[param_name] = \
-                        cv2.cvtColor(cv2.imdecode(np.frombuffer(values, np.uint8), cv2.IMREAD_COLOR),
-                                     cv2.COLOR_RGB2BGR)
-                # 如果输入的是字符串，则作为图像路径处理
+                    self.requests_inputs[param_name] = utils.bytes_to_array(values)
+                # 如果输入的是字符串，则作为图像路径处理，使用Imread读取图像
                 elif isinstance(values, str):
-                    self.requests_inputs[param_name] = cv2.imread(values, cv2.IMREAD_UNCHANGED)
+                    im = _Image.open(values)
+                    self.requests_inputs[param_name] = np.array(im)
                 else:
                     raise TypeError("网络请求中{}的类型与定义的image类型不一致".format(param_name))
 
             # 对于输入的类型为number的情况
             elif self.backbone_inputs[iter] == "number":
-                assert is_float(values), "网络请求中{}的类型与定义的number类型不一致".format(param_name)
+                assert utils.is_float(values), "网络请求中{}的类型与定义的number类型不一致".format(param_name)
                 self.requests_inputs[param_name] = float(values)
 
             # 对于输入的类型为text的情况
             elif self.backbone_inputs[iter] == "text":
                 assert isinstance(values, str), "网络请求中{}的类型与定义的text类型不一致".format(param_name)
                 self.requests_inputs[param_name] = values
 
             # 对于输入的类型为list的情况
             elif self.backbone_inputs[iter] == "list":
-                self.requests_inputs[param_name] = is_list(values)
+                self.requests_inputs[param_name] = utils.is_list(values)
 
             # 对于输入的类型为dict的情况
             elif self.backbone_inputs[iter] == "dict":
-                self.requests_inputs[param_name] = is_dict(values)
+                self.requests_inputs[param_name] = utils.is_dict(values)
 
             else:
                 raise TypeError("backbone_type_checker have BUGs")
 
     def requests_output_type_checker(self, result: Any) -> None:
         # 根据result得到返回变量数量
         if isinstance(result, tuple):
             self.requests_outputs_variables_num = len(result)
-        # Todo:对于输出为0/None的兼容性开发
-        elif result is None:
-            self.requests_outputs_variables_num = 0
         else:
             self.requests_outputs_variables_num = 1
 
-        assert self.requests_outputs_variables_num == len(self.backbone_outputs), "fn输出的数量与outputs定义的不一致"
+        assert self.requests_outputs_variables_num >= len(self.backbone_outputs), "fn返回结果的数量不能小于backbone_outputs的数量"
 
     def requests_output_converter(self, result: Any) -> Union[Dict[str, Any], None]:
         if self.requests_outputs_variables_num == 1:
             result = [result]
-        elif self.requests_outputs_variables_num > 1:
-            result = list(result)
         else:
+            result = list(result)
+
+        if len(self.backbone_outputs) == 0:
             return None
+
         result_json = {}
         for iter, backbone_output in enumerate(self.backbone_outputs):
             if result[iter] is None:
                 result_json[iter] = {"content": None}
             elif backbone_output == "image":
-                assert isinstance(result[iter], np.ndarray)
-                result[iter] = cv2.cvtColor(result[iter], cv2.COLOR_RGB2BGR)
-                result[iter] = cv2.imencode(".jpg", result[iter])[1].tostring()
-                result_json[iter] = {"content": base64.b64encode(result[iter])}
+                y = result[iter]
+                if isinstance(y, np.ndarray):
+                    im_base64 = utils.encode_array_to_base64(y)
+                elif isinstance(y, _Image.Image):
+                    im_base64 = utils.encode_pil_to_base64(y)
+                elif isinstance(y, (str, Path)):
+                    im_base64 = utils.encode_url_or_file_to_base64(y)
+                else:
+                    raise ValueError("Cannot process this value as an Image")
+                result_json[iter] = {"content": im_base64}
+
             elif backbone_output == "text":
                 assert isinstance(result[iter], str)
                 result_json[iter] = {"content": result[iter]}
+
             elif backbone_output == "number":
                 assert isinstance(result[iter], (int, float))
                 result_json[iter] = {"content": result[iter]}
+
             elif backbone_output == ["dict"]:
                 assert isinstance(result, dict)
                 result_json[iter] = {"content": result[iter]}
+
             elif backbone_output == ["list"]:
                 assert isinstance(result, list)
                 result_json[iter] = {"content": result[iter]}
+
             else:
                 raise TypeError("类型检查模块存在Bug")
 
         return result_json
-
-
-class BaseRequests:
-    """
-    增加在Python端快速调用SwanAPI服务的类。
-    主要降低API调用的门槛，尤其是对图像等数据类型。
-    必要输入：
-    - url: str, API的url地址
-    - inputs: Json
-    - methods: 请求的类型，可选值为["GET", "POST", "PUT", "DELETE"]
-    """
-
-    def base_request(self,
-                     url: str,
-                     inputs: Dict[str, Any],
-                     methods: str):
-        payload = {}
-        files = []
-        headers = {}
-
-        for key, value in inputs.items():
-            # 如果value的类型是文件类型
-            if isinstance(value, Files):
-                files.append((key, value.content()))
-            else:
-                payload[key] = value
-
-        inputs_dict = {}
-        if len(files) != 0:
-            inputs_dict['files'] = files
-        if len(payload) != 0:
-            inputs_dict['data'] = payload
-
-        response = requests.request(methods, url, headers=headers, **inputs_dict)
-        return response.json()
-
-    def post(self,
-             url: str,
-             inputs: Dict[str, Any],
-             ):
-        return self.base_request(url, inputs, "POST")
-
-    def get(self,
-            url: str,
-            inputs: Dict[str, Any],
-            ):
-        return self.base_request(url, inputs, "get")
-
-
-def SwanRequests(url: str,
-                 inputs: Dict[str, Any],
-                 methods: str = "POST"):
-    return BaseRequests().base_request(url, inputs, methods)
```

## swanapi/server.py

```diff
@@ -1,13 +1,15 @@
 from flask import Flask, request
 from typing import Any, Callable, Dict, List, Optional, Type, Union
-from .utils import bytes_encoder
+from .utils import utils
 from .base_inference import BaseInference
 import json
 
+import time
+
 app = Flask("SwanAPI Server")
 
 
 class SwanInference(BaseInference):
     """
     我们将分为两个生命周期：
     1. Backbone: 以fn, inputs和outputs为基础，构建一个推理骨架
@@ -42,25 +44,24 @@
         self.backbone_get_fn_parameters()
 
     def requests(self, **inputs):
         # 检查Web输入的类型是否符合Backbone定义的输入类型
         self.requests_input_type_checker(inputs)
         # 根据类型转换为符合Backbone定义的输入类型
         self.requests_input_converter()
-
         # 调用fn, 得到结果
         result = self.fn(**self.requests_inputs)
 
         # 检查结果是否符合Backbone定义的输出类型
         self.requests_output_type_checker(result)
         # 根据Backbone定义的输出类型进行转换
         result_json = self.requests_output_converter(result)
 
         # 将结果转换为json格式
-        return json.dumps(result_json, default=bytes_encoder)
+        return json.dumps(result_json, default=utils.bytes_encoder)
 
     def launch(self,
                server_name: str = "0.0.0.0",
                port: int = 8000
                ) -> None:
         """
         启动Web服务, 基于Flask
```

## Comparing `swanapi-0.1.9b2.dist-info/RECORD` & `swanapi-0.2.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-swanapi/__init__.py,sha256=h4WVKn4K78msugS-evjCc2iydSU5K8lyGYHeJm3vcQM,158
-swanapi/base_inference.py,sha256=udI0rNdobPZLRS_-qUXnbQ4cbJsoBeew2Q0UzwfUklk,10349
+swanapi/__init__.py,sha256=2N4vWNDaCYewP1euHTVKHE1zmtStmsi0af6S-lu8Bs0,157
+swanapi/base_inference.py,sha256=QlWvZI1rpff8pdcMLQ-AKDBHbAIKulXDXJd2I6TAnJw,8931
+swanapi/base_requests.py,sha256=kpGxsP26WgZG7SroPCoDZl_7fjsgHmXOSFHGKbCnozc,1831
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
-swanapi/server.py,sha256=_8CvGMp69-WSvNr6zfZlAb6-Mnxi1b-H9daH2vkXEpE,2759
+swanapi/server.py,sha256=eLtrZmN0RU9RP9Yzh7z33lqkzaZerylNHAVhYXxkr4E,2769
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
-swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
-swanapi-0.1.9b2.dist-info/METADATA,sha256=xQB2b5pTSJxvPa-OBXu8KJ51kMLan0jMKDwmWcjv3tw,349
-swanapi-0.1.9b2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.9b2.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.1.9b2.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.9b2.dist-info/RECORD,,
+swanapi-0.2.0.dist-info/METADATA,sha256=7m2ryE58-cufMAIClPhrkiNxQw7gEBJvvY1avCS92EE,340
+swanapi-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.2.0.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.2.0.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.2.0.dist-info/RECORD,,
```

