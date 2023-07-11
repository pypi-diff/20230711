# Comparing `tmp/paradigm_client-0.3.tar.gz` & `tmp/paradigm_client-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm_client-0.3.tar", last modified: Tue Jun 27 09:48:48 2023, max compression
+gzip compressed data, was "paradigm_client-0.4.tar", last modified: Tue Jul 11 12:53:54 2023, max compression
```

## Comparing `paradigm_client-0.3.tar` & `paradigm_client-0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.109690 paradigm_client-0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-27 09:48:18.000000 paradigm_client-0.3/.github/workflows/build-test-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-27 09:48:18.000000 paradigm_client-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 09:48:18.000000 paradigm_client-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 09:48:48.113690 paradigm_client-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-27 09:48:18.000000 paradigm_client-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/create_endpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/create_endpoint_batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/mini_instruct_sagemaker_model_consumer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/select_endpoint.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/paradigm_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/remote_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/paradigm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:48:18.000000 paradigm_client-0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:48:48.113690 paradigm_client-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-27 09:48:18.000000 paradigm_client-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-27 09:48:18.000000 paradigm_client-0.3/tests/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.442010 paradigm_client-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-11 12:53:28.000000 paradigm_client-0.4/.github/workflows/build-test-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-11 12:53:28.000000 paradigm_client-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 12:53:28.000000 paradigm_client-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-11 12:53:54.438009 paradigm_client-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 12:53:28.000000 paradigm_client-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-11 12:53:28.000000 paradigm_client-0.4/examples/create_endpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-11 12:53:28.000000 paradigm_client-0.4/examples/create_endpoint_batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-11 12:53:28.000000 paradigm_client-0.4/examples/mini_instruct_sagemaker_model_consumer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-11 12:53:28.000000 paradigm_client-0.4/examples/select_endpoint.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/paradigm_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:28.000000 paradigm_client-0.4/paradigm_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-07-11 12:53:28.000000 paradigm_client-0.4/paradigm_client/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-11 12:53:28.000000 paradigm_client-0.4/paradigm_client/remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-11 12:53:28.000000 paradigm_client-0.4/paradigm_client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-11 12:53:28.000000 paradigm_client-0.4/paradigm_client/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/paradigm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-11 12:53:54.000000 paradigm_client-0.4/paradigm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 12:53:54.000000 paradigm_client-0.4/paradigm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:53:54.000000 paradigm_client-0.4/paradigm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 12:53:54.000000 paradigm_client-0.4/paradigm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 12:53:54.000000 paradigm_client-0.4/paradigm_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 12:53:28.000000 paradigm_client-0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:53:54.442010 paradigm_client-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-11 12:53:28.000000 paradigm_client-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:54.438009 paradigm_client-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:28.000000 paradigm_client-0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-11 12:53:28.000000 paradigm_client-0.4/tests/test_remote_model.py
```

### Comparing `paradigm_client-0.3/.github/workflows/build-test-deploy.yaml` & `paradigm_client-0.4/.github/workflows/build-test-deploy.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,18 @@
       - name: Build package
         run: |
           pip install setuptools wheel
           python setup.py sdist bdist_wheel
 
       - name: Test package
         run: |
+          python3 -m venv .venv
+          source .venv/bin/activate
           pip install dist/*.whl
-          python tests/example.py
+          python3 -m pytest
 
       #      - name: Publish to TestPyPI
       #        uses: pypa/gh-action-pypi-publish@release/v1
       #        with:
       #          user: ${{ env.TWINE_USERNAME_TEST }}
       #          password: ${{ env.TWINE_PWD_TEST }}
       #          repository-url: https://test.pypi.org/legacy/
```

### Comparing `paradigm_client-0.3/.gitignore` & `paradigm_client-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/LICENSE` & `paradigm_client-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/PKG-INFO` & `paradigm_client-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm_client
-Version: 0.3
+Version: 0.4
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paradigm_client-0.3/README.md` & `paradigm_client-0.4/README.md`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/examples/create_endpoint.ipynb` & `paradigm_client-0.4/examples/create_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/examples/create_endpoint_batching.ipynb` & `paradigm_client-0.4/examples/create_endpoint_batching.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/examples/mini_instruct_sagemaker_model_consumer.ipynb` & `paradigm_client-0.4/examples/mini_instruct_sagemaker_model_consumer.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/examples/select_endpoint.ipynb` & `paradigm_client-0.4/examples/select_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/paradigm_client/communicator.py` & `paradigm_client-0.4/paradigm_client/communicator.py`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/paradigm_client/remote_model.py` & `paradigm_client-0.4/paradigm_client/remote_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
+import re
 import time
-from typing import Any, Generator, Optional, Union
+from typing import Any, Generator, Optional, Union, Dict, Literal
+import requests
 
 from pydantic import BaseModel, validate_arguments
 
 from .request import (
     CreateRequest,
     CreateParameters,
     AnalyseRequest,
     SelectRequest,
     TokenizeRequest,
     Endpoint,
 )
-from .response import CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse
+from .response import CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse, FeedbackResponse
 from .communicator import Communicator
 
+DEFAULT_BASE_ADDRESS = "https://paradigm.lighton.ai"
+
 
 def print_logs(msg, end: Optional[str] = None, verbose: bool = False):
     if verbose:
         print(msg, end=end, flush=True)
 
 
 class RemoteModel:
@@ -27,27 +31,32 @@
         base_address: Optional[str] = None,
         headers: Optional[dict[str, str]] = None,
         timeout_s: int = 180,
         verbose: bool = False,
         comm=None,
         raise_for_status: bool = False,
         model_name: Optional[str] = None,
+        api_key: Optional[str] = None
     ) -> None:
-        self.verbose = verbose
-        assert base_address is not None or comm is not None, "You must provide base_address or comm"
-        base_headers = {"Content-Type": "application/json", "Accept": "application/json"} | {
-            "X-API-KEY": os.environ.get("PARADIGM_API_KEY", str(None)),
-            "X-Model": str(model_name),
-        }
+        self._api_key = api_key if api_key is not None else os.environ.get("PARADIGM_API_KEY", str(None))
+        assert api_key != str(None), "You must provide an API key through the PARADIGM_API_KEY environment variable or the api_key parameter"
+
+        self.base_address = DEFAULT_BASE_ADDRESS if base_address is None else base_address
+        # Remove '/' at the end of the given base address
+        self.base_address = re.sub(r"\/+$", "", self.base_address)
+
+        self.base_headers = {"Content-Type": "application/json", "Accept": "application/json"}
+        updated_headers = {**self.base_headers, **{"X-API-KEY": self._api_key, "X-Model": str(model_name)}}
         self.comm = comm or Communicator(
-            base_address,
-            headers or base_headers,
+            self.base_address,
+            headers or updated_headers,
             timeout_s,
             raise_for_status=raise_for_status,
         )
+        self.verbose = verbose
         self._wait_for_model_server()
 
     def _post(
         self, data: Any, endpoint: Endpoint, num_tasks: int, show_progress: bool = True
     ) -> Union[list[SelectResponse], list[AnalyseResponse], list[CreateResponse], list[TokenizeResponse], ErrorResponse]:
 
         response = self.comm(data, endpoint, stream=False, **{"num_tasks": num_tasks, "show_progress": show_progress})
@@ -188,14 +197,33 @@
 
     @validate_arguments
     def tokenize_from_objects(
         self, tokenize_obj: Union[TokenizeRequest, list[TokenizeRequest]], show_progress: bool = False
     ) -> Union[list[TokenizeResponse], ErrorResponse]:
         return self._post_objects(tokenize_obj, Endpoint.tokenize, show_progress=show_progress)
 
+    def log_feedback(
+            self,
+            rating_id: Union[int, str],
+            completion_id: str,
+            data: Dict[Literal["flag", "value", "tag", "comment"], Union[float, str, bool]]
+    ):
+        """
+        Log a feedback into Paradigm.
+        :param rating_id: ID of the feedback type to use; must be created in Paradigm beforehand
+        :param completion_id: ID of the completion to link the feedback to. Can be obtained from a llm response.
+        :param data: Actual feedback data. Must be a dictionary
+        :return: FeedbackResponse object with the HTTP status code
+        """
+        response = requests.post(
+            f"{self.base_address}/api/v1/rate/{rating_id}/{completion_id}",
+            headers={**self.base_headers, **{'Authorization': f'Api-Key {self._api_key}'}},
+            json=data)
+        return FeedbackResponse(status_code=response.status_code)
+
     def _wait_for_model_server(self):
         print_logs(f"Waiting for the ModelServer to be ready", end="", verbose=self.verbose)
         counter = 0
         while not self.comm.is_available():
             print_logs(f".", end="", verbose=self.verbose)
             time.sleep(10.0)
             counter += 1
```

### Comparing `paradigm_client-0.3/paradigm_client/request.py` & `paradigm_client-0.4/paradigm_client/request.py`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.3/paradigm_client/response.py` & `paradigm_client-0.4/paradigm_client/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,7 +60,11 @@
     status_code: int
 
     def get_formatted_output(self, unused):
         return self
 
     def pickle(self):
         return pickle.dumps((self.dict(), None), protocol=pickle.HIGHEST_PROTOCOL)
+
+
+class FeedbackResponse(BaseModel):
+    status_code: int
```

### Comparing `paradigm_client-0.3/paradigm_client.egg-info/PKG-INFO` & `paradigm_client-0.4/paradigm_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-client
-Version: 0.3
+Version: 0.4
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paradigm_client-0.3/paradigm_client.egg-info/SOURCES.txt` & `paradigm_client-0.4/paradigm_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 paradigm_client/request.py
 paradigm_client/response.py
 paradigm_client.egg-info/PKG-INFO
 paradigm_client.egg-info/SOURCES.txt
 paradigm_client.egg-info/dependency_links.txt
 paradigm_client.egg-info/requires.txt
 paradigm_client.egg-info/top_level.txt
-tests/example.py
+tests/__init__.py
+tests/test_remote_model.py
```

### Comparing `paradigm_client-0.3/setup.py` & `paradigm_client-0.4/setup.py`

 * *Files identical despite different names*

