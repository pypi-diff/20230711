# Comparing `tmp/hugging_py_face-0.3.2.tar.gz` & `tmp/hugging_py_face-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.3.2.tar", last modified: Fri Jul  7 17:52:12 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.4.2.tar", last modified: Tue Jul 11 19:00:06 2023, max compression
```

## Comparing `hugging_py_face-0.3.2.tar` & `hugging_py_face-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/
--rw-rw-rw-   0        0        0     6177 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face/
--rw-rw-rw-   0        0        0      466 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      676 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3927 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0      884 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/base_api.py
--rw-rw-rw-   0        0        0     2852 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face/config/
--rw-rw-rw-   0        0        0      837 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config/config.yaml
--rw-rw-rw-   0        0        0      265 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config/logging.yaml
--rw-rw-rw-   0        0        0      320 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0      171 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/exceptions.py
--rw-rw-rw-   0        0        0     2447 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    24515 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/
+-rw-rw-rw-   0        0        0     6177 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      676 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3927 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0     1058 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/base_api.py
+-rw-rw-rw-   0        0        0     2852 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      837 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      265 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/config/logging.yaml
+-rw-rw-rw-   0        0        0      320 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0      171 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/exceptions.py
+-rw-rw-rw-   0        0        0     2483 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    24551 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 19:00:06.000000 hugging_py_face-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-11 18:59:45.000000 hugging_py_face-0.4.2/setup.py
```

### Comparing `hugging_py_face-0.3.2/PKG-INFO` & `hugging_py_face-0.4.2/hugging_py_face.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hugging_py_face
-Version: 0.3.2
+Name: hugging-py-face
+Version: 0.4.2
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.3.2/README.md` & `hugging_py_face-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/hugging_py_face/__init__.py` & `hugging_py_face-0.4.2/hugging_py_face/__init__.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/hugging_py_face/audio_processing.py` & `hugging_py_face-0.4.2/hugging_py_face/audio_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/hugging_py_face/base_api.py` & `hugging_py_face-0.4.2/hugging_py_face/base_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import logging
 import logging.config
 from huggingface_hub import HfApi
-from typing import Text
+from typing import Text, Optional
 
 from .config_parser import ConfigParser
 from .exceptions import TaskModelMismatchException
 
 logging_config_parser = ConfigParser('config/logging.yaml')
 logging.config.dictConfig(logging_config_parser.get_config_dict())
 logger = logging.getLogger()
 
 
 class BaseAPI:
-    def __init__(self, api_token):
+    def __init__(self, api_token: Text, api_url: Optional[Text] = None):
         self.api_token = api_token
 
         config_parser = ConfigParser()
         self.config = config_parser.get_config_dict()
 
+        if api_url:
+            self.api_url = api_url
+        else:
+            self.api_url = self.config['BASE_URL']
+
         self.logger = logger
 
         self.hf_api = HfApi()
 
     def _check_model_task_match(self, model: Text, task: Text) -> None:
         metadata = self.hf_api.model_info(model)
         if task != metadata.pipeline_tag:
```

### Comparing `hugging_py_face-0.3.2/hugging_py_face/computer_vision.py` & `hugging_py_face-0.4.2/hugging_py_face/computer_vision.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/hugging_py_face/config/config.yaml` & `hugging_py_face-0.4.2/hugging_py_face/config/config.yaml`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/hugging_py_face/multimedia_processing.py` & `hugging_py_face-0.4.2/hugging_py_face/multimedia_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from typing import Text, Dict, List, Optional, Union
 
 from .base_api import BaseAPI
 from .exceptions import HTTPServiceUnavailableException, APICallException
 
 
 class MultimediaProcessing(BaseAPI):
-    def __init__(self, api_token):
-        super().__init__(api_token)
+    def __init__(self, api_token: Text, api_url: Optional[Text] = None):
+        super().__init__(api_token, api_url)
 
     def _query(self, input: Text, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
         if model:
             self._check_model_task_match(model, task)
 
-        api_url = f"{self.config['BASE_URL']}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
+        api_url = f"{self.api_url}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
 
         headers = {
             "Authorization": f"Bearer {self.api_token}"
         }
 
         if input.startswith("http"):
             response = requests.get(input)
```

### Comparing `hugging_py_face-0.3.2/hugging_py_face/nlp.py` & `hugging_py_face-0.4.2/hugging_py_face/nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from typing import Text, List, Dict, Optional, Union
 
 from .base_api import BaseAPI
 from .exceptions import HTTPServiceUnavailableException, APICallException
 
 
 class NLP(BaseAPI):
-    def __init__(self, api_token):
-        super().__init__(api_token)
+    def __init__(self, api_token: Text, api_url: Optional[Text] = None):
+        super().__init__(api_token, api_url)
 
     def _query(self, inputs: Union[Text, List, Dict], parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
         if model:
             self._check_model_task_match(model, task)
 
-        api_url = f"{self.config['BASE_URL']}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
+        api_url = f"{self.api_url}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
 
         headers = {
             "Authorization": f"Bearer {self.api_token}"
         }
 
         data = {
             "inputs": inputs
```

### Comparing `hugging_py_face-0.3.2/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hugging-py-face
-Version: 0.3.2
+Name: hugging_py_face
+Version: 0.4.2
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.3.2/hugging_py_face.egg-info/SOURCES.txt` & `hugging_py_face-0.4.2/hugging_py_face.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.2/setup.py` & `hugging_py_face-0.4.2/setup.py`

 * *Files identical despite different names*

