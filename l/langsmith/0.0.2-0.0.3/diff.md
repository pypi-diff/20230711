# Comparing `tmp/langsmith-0.0.2.tar.gz` & `tmp/langsmith-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.2.tar", max compression
+gzip compressed data, was "langsmith-0.0.3.tar", max compression
```

## Comparing `langsmith-0.0.2.tar` & `langsmith-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     8006 2023-07-05 17:54:45.352295 langsmith-0.0.2/README.md
--rw-r--r--   0        0        0      479 2023-07-05 17:54:45.352708 langsmith-0.0.2/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.2/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.2/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.2/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-07-05 17:54:45.353810 langsmith-0.0.2/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14054 2023-07-05 17:54:45.354144 langsmith-0.0.2/langsmith/cli/main.py
--rw-r--r--   0        0        0    27679 2023-07-05 17:54:45.354525 langsmith-0.0.2/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.2/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.2/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.2/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.2/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6120 2023-07-05 17:54:45.356170 langsmith-0.0.2/langsmith/run_trees.py
--rw-r--r--   0        0        0     6452 2023-07-05 18:01:48.582191 langsmith-0.0.2/langsmith/schemas.py
--rw-r--r--   0        0        0     3688 2023-07-05 17:54:45.356784 langsmith-0.0.2/langsmith/utils.py
--rw-r--r--   0        0        0      878 2023-07-05 18:01:48.582953 langsmith-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8006 2023-07-05 17:54:45.352295 langsmith-0.0.3/README.md
+-rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.3/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.3/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.3/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.3/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-07-05 17:54:45.353810 langsmith-0.0.3/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14054 2023-07-05 17:54:45.354144 langsmith-0.0.3/langsmith/cli/main.py
+-rw-r--r--   0        0        0    27876 2023-07-11 05:55:53.837648 langsmith-0.0.3/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.3/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.3/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.3/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.3/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6120 2023-07-05 17:54:45.356170 langsmith-0.0.3/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6503 2023-07-11 05:53:09.644342 langsmith-0.0.3/langsmith/schemas.py
+-rw-r--r--   0        0        0     3683 2023-07-11 05:55:51.017340 langsmith-0.0.3/langsmith/utils.py
+-rw-r--r--   0        0        0      878 2023-07-11 06:02:01.855164 langsmith-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.3/PKG-INFO
```

### Comparing `langsmith-0.0.2/README.md` & `langsmith-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.3/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/cli/main.py` & `langsmith-0.0.3/langsmith/cli/main.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/client.py` & `langsmith-0.0.3/langsmith/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 )
 
 from langsmith.evaluation.evaluator import RunEvaluator
 from langsmith.schemas import (
     APIFeedbackSource,
     Dataset,
     DatasetCreate,
+    DataType,
     Example,
     ExampleCreate,
     ExampleUpdate,
     Feedback,
     FeedbackCreate,
     FeedbackSourceBase,
     FeedbackSourceType,
@@ -96,15 +97,15 @@
         return obj.isoformat()
     elif isinstance(obj, UUID):
         return str(obj)
     raise TypeError("Type %s not serializable" % type(obj))
 
 
 class Client(BaseSettings):
-    """Client for interacting with the LangChain+ API."""
+    """Client for interacting with the LangSmith API."""
 
     api_key: Optional[str] = Field(default=None, env="LANGCHAIN_API_KEY")
     api_url: str = Field(default="http://localhost:1984", env="LANGCHAIN_ENDPOINT")
     retry_config: Mapping[str, Any] = Field(
         default_factory=_default_retry_config, exclude=True
     )
     timeout_ms: int = Field(default=4000)
@@ -113,27 +114,27 @@
     def validate_api_key_if_hosted(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Verify API key is provided if url not localhost."""
         api_url: str = values.get("api_url", "http://localhost:1984")
         api_key: Optional[str] = values.get("api_key")
         if not _is_localhost(api_url):
             if not api_key:
                 raise LangChainPlusUserError(
-                    "API key must be provided when using hosted LangChain+ API"
+                    "API key must be provided when using hosted LangSmith API"
                 )
         return values
 
     def _repr_html_(self) -> str:
         """Return an HTML representation of the instance with a link to the URL."""
         if _is_localhost(self.api_url):
             link = "http://localhost"
         elif "dev" in self.api_url.split(".", maxsplit=1)[0]:
             link = "https://dev.langchain.plus"
         else:
             link = "https://www.langchain.plus"
-        return f'<a href="{link}", target="_blank" rel="noopener">LangChain+ Client</a>'
+        return f'<a href="{link}", target="_blank" rel="noopener">LangSmith Client</a>'
 
     def __repr__(self) -> str:
         """Return a string representation of the instance with a link to the URL."""
         return f"Client (API URL: {self.api_url})"
 
     @property
     def _headers(self) -> Dict[str, str]:
@@ -180,45 +181,50 @@
         self,
         df: pd.DataFrame,
         name: str,
         input_keys: Sequence[str],
         output_keys: Sequence[str],
         *,
         description: Optional[str] = None,
+        data_type: Optional[DataType] = DataType.kv,
     ) -> Dataset:
-        """Upload a dataframe as individual examples to the LangChain+ API."""
+        """Upload a dataframe as individual examples to the LangSmith API."""
         csv_file = BytesIO()
         df.to_csv(csv_file, index=False)
         csv_file.seek(0)
         return self.upload_csv(
             ("data.csv", csv_file),
             input_keys=input_keys,
             output_keys=output_keys,
             description=description,
             name=name,
+            data_type=data_type,
         )
 
     def upload_csv(
         self,
         csv_file: Union[str, Tuple[str, BytesIO]],
         input_keys: Sequence[str],
         output_keys: Sequence[str],
         *,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        data_type: Optional[DataType] = DataType.kv,
     ) -> Dataset:
-        """Upload a CSV file to the LangChain+ API."""
+        """Upload a CSV file to the LangSmith API."""
         data = {
-            "input_keys": ",".join(input_keys),
-            "output_keys": ",".join(output_keys),
+            "input_keys": input_keys,
+            "output_keys": output_keys,
         }
         if name:
             data["name"] = name
         if description:
             data["description"] = description
+        if data_type:
+            data["data_type"] = data_type.value
         if isinstance(csv_file, str):
             with open(csv_file, "rb") as f:
                 file_ = {"file": f}
                 response = requests.post(
                     self.api_url + "/datasets/upload",
                     headers=self._headers,
                     data=data,
@@ -247,15 +253,15 @@
         name: str,
         inputs: Dict[str, Any],
         run_type: Union[str, RunTypeEnum],
         *,
         execution_order: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
-        """Persist a run to the LangChain+ API."""
+        """Persist a run to the LangSmith API."""
         project_name = kwargs.pop(
             "project_name",
             kwargs.pop(
                 "session_name",
                 os.environ.get(
                     # TODO: Deprecate LANGCHAIN_SESSION
                     "LANGCHAIN_PROJECT",
@@ -288,15 +294,15 @@
         )
 
     def update_run(
         self,
         run_id: ID_TYPE,
         **kwargs: Any,
     ) -> None:
-        """Update a run to the LangChain+ API."""
+        """Update a run to the LangSmith API."""
         headers = {**self._headers, "Accept": "application/json"}
         request_with_retries(
             "patch",
             f"{self.api_url}/runs/{run_id}",
             request_kwargs={
                 "data": json.dumps(kwargs, default=_serialize_json),
                 "headers": headers,
@@ -316,15 +322,15 @@
             runs[child_run.id] = child_run
         run.child_runs = treemap.pop(run.id, [])
         for run_id, children in treemap.items():
             runs[run_id].child_runs = children
         return run
 
     def read_run(self, run_id: ID_TYPE, load_child_runs: bool = False) -> Run:
-        """Read a run from the LangChain+ API.
+        """Read a run from the LangSmith API.
 
         Args:
             run_id: The ID of the run to read.
             load_child_runs: Whether to load nested child runs.
 
         Returns:
             The run.
@@ -342,15 +348,15 @@
         project_name: Optional[str] = None,
         run_type: Optional[str] = None,
         dataset_name: Optional[str] = None,
         dataset_id: Optional[ID_TYPE] = None,
         reference_example_id: Optional[ID_TYPE] = None,
         **kwargs: Any,
     ) -> Iterator[Run]:
-        """List runs from the LangChain+ API."""
+        """List runs from the LangSmith API."""
         if project_name is not None:
             if project_id is not None:
                 raise ValueError("Only one of project_id or project_name may be given")
             project_id = self.read_project(project_name=project_name).id
         if dataset_name is not None:
             if dataset_id is not None:
                 raise ValueError("Only one of dataset_id or dataset_name may be given")
@@ -365,37 +371,34 @@
         if dataset_id is not None:
             query_params["dataset"] = dataset_id
         yield from (
             Run(**run) for run in self._get_paginated_list("/runs", params=query_params)
         )
 
     def delete_run(self, run_id: ID_TYPE) -> None:
-        """Delete a run from the LangChain+ API."""
+        """Delete a run from the LangSmith API."""
         response = requests.delete(
             f"{self.api_url}/runs/{run_id}",
             headers=self._headers,
         )
         raise_for_status_with_text(response)
 
     def create_project(
         self,
         project_name: str,
         *,
         project_extra: Optional[dict] = None,
-        mode: Optional[str] = None,
         upsert: bool = False,
     ) -> TracerSession:
-        """Create a project on the LangChain+ API."""
+        """Create a project on the LangSmith API."""
         endpoint = f"{self.api_url}/sessions"
         body = {
             "name": project_name,
             "extra": project_extra,
         }
-        if mode:
-            body["mode"] = mode
         params = {}
         if upsert:
             params["upsert"] = True
         response = requests.post(
             endpoint,
             headers=self._headers,
             json=body,
@@ -403,15 +406,15 @@
         raise_for_status_with_text(response)
         return TracerSession(**response.json())
 
     @xor_args(("project_id", "project_name"))
     def read_project(
         self, *, project_id: Optional[str] = None, project_name: Optional[str] = None
     ) -> TracerSessionResult:
-        """Read a project from the LangChain+ API.
+        """Read a project from the LangSmith API.
 
         Args:
             project_id: The ID of the project to read.
             project_name: The name of the project to read.
                 Note: Only one of project_id or project_name may be given.
         """
         path = "/sessions"
@@ -427,42 +430,47 @@
         if isinstance(result, list):
             if len(result) == 0:
                 raise LangChainPlusError(f"Project {project_name} not found")
             return TracerSessionResult(**result[0])
         return TracerSessionResult(**response.json())
 
     def list_projects(self) -> Iterator[TracerSession]:
-        """List projects from the LangChain+ API."""
+        """List projects from the LangSmith API."""
         yield from (
             TracerSession(**project)
             for project in self._get_paginated_list("/sessions")
         )
 
     @xor_args(("project_name", "project_id"))
     def delete_project(
         self, *, project_name: Optional[str] = None, project_id: Optional[str] = None
     ) -> None:
-        """Delete a project from the LangChain+ API."""
+        """Delete a project from the LangSmith API."""
         if project_name is not None:
             project_id = str(self.read_project(project_name=project_name).id)
         elif project_id is None:
             raise ValueError("Must provide project_name or project_id")
         response = requests.delete(
             self.api_url + f"/sessions/{project_id}",
             headers=self._headers,
         )
         raise_for_status_with_text(response)
 
     def create_dataset(
-        self, dataset_name: str, *, description: Optional[str] = None
+        self,
+        dataset_name: str,
+        *,
+        description: Optional[str] = None,
+        data_type: DataType = DataType.kv,
     ) -> Dataset:
-        """Create a dataset in the LangChain+ API."""
+        """Create a dataset in the LangSmith API."""
         dataset = DatasetCreate(
             name=dataset_name,
             description=description,
+            data_type=data_type,
         )
         response = requests.post(
             self.api_url + "/datasets",
             headers=self._headers,
             data=dataset.json(),
         )
         raise_for_status_with_text(response)
@@ -491,15 +499,15 @@
         if isinstance(result, list):
             if len(result) == 0:
                 raise LangChainPlusError(f"Dataset {dataset_name} not found")
             return Dataset(**result[0])
         return Dataset(**result)
 
     def list_datasets(self) -> Iterator[Dataset]:
-        """List the datasets on the LangChain+ API."""
+        """List the datasets on the LangSmith API."""
         yield from (
             Dataset(**dataset) for dataset in self._get_paginated_list("/datasets")
         )
 
     @xor_args(("dataset_id", "dataset_name"))
     def delete_dataset(
         self,
@@ -523,15 +531,15 @@
         self,
         inputs: Mapping[str, Any],
         dataset_id: Optional[ID_TYPE] = None,
         dataset_name: Optional[str] = None,
         created_at: Optional[datetime] = None,
         outputs: Optional[Mapping[str, Any]] = None,
     ) -> Example:
-        """Create a dataset example in the LangChain+ API."""
+        """Create a dataset example in the LangSmith API."""
         if dataset_id is None:
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
 
         data = {
             "inputs": inputs,
             "outputs": outputs,
             "dataset_id": dataset_id,
@@ -543,22 +551,22 @@
             f"{self.api_url}/examples", headers=self._headers, data=example.json()
         )
         raise_for_status_with_text(response)
         result = response.json()
         return Example(**result)
 
     def read_example(self, example_id: ID_TYPE) -> Example:
-        """Read an example from the LangChain+ API."""
+        """Read an example from the LangSmith API."""
         response = self._get_with_retries(f"/examples/{example_id}")
         return Example(**response.json())
 
     def list_examples(
         self, dataset_id: Optional[ID_TYPE] = None, dataset_name: Optional[str] = None
     ) -> Iterator[Example]:
-        """List the datasets on the LangChain+ API."""
+        """List the datasets on the LangSmith API."""
         params = {}
         if dataset_id is not None:
             params["dataset"] = dataset_id
         elif dataset_name is not None:
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
             params["dataset"] = dataset_id
         else:
@@ -724,15 +732,15 @@
         score: Union[float, int, bool, None] = None,
         value: Union[float, int, bool, str, dict, None] = None,
         correction: Union[str, dict, None] = None,
         comment: Union[str, None] = None,
         source_info: Optional[Dict[str, Any]] = None,
         feedback_source_type: Union[FeedbackSourceType, str] = FeedbackSourceType.API,
     ) -> Feedback:
-        """Create a feedback in the LangChain+ API.
+        """Create a feedback in the LangSmith API.
 
         Args:
             run_id: The ID of the run to provide feedback on.
             key: The name of the metric, tag, or 'aspect' this
                 feedback is about.
             score: The score to rate this run on the metric
                 or aspect.
@@ -764,25 +772,25 @@
             headers={**self._headers, "Content-Type": "application/json"},
             data=feedback.json(exclude_none=True),
         )
         raise_for_status_with_text(response)
         return Feedback(**response.json())
 
     def read_feedback(self, feedback_id: ID_TYPE) -> Feedback:
-        """Read a feedback from the LangChain+ API."""
+        """Read a feedback from the LangSmith API."""
         response = self._get_with_retries(f"/feedback/{feedback_id}")
         return Feedback(**response.json())
 
     def list_feedback(
         self,
         *,
         run_ids: Optional[Sequence[ID_TYPE]] = None,
         **kwargs: Any,
     ) -> Iterator[Feedback]:
-        """List the feedback objects on the LangChain+ API."""
+        """List the feedback objects on the LangSmith API."""
         params = {
             "run": run_ids,
             **kwargs,
         }
 
         yield from (
             Feedback(**feedback)
```

### Comparing `langsmith-0.0.2/langsmith/evaluation/evaluator.py` & `langsmith-0.0.3/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.3/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/run_helpers.py` & `langsmith-0.0.3/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/run_trees.py` & `langsmith-0.0.3/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.2/langsmith/schemas.py` & `langsmith-0.0.3/langsmith/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,19 +47,28 @@
     inputs: Optional[Dict[str, Any]] = None
     outputs: Optional[Dict[str, Any]] = None
 
     class Config:
         frozen = True
 
 
+class DataType(str, Enum):
+    """Enum for dataset data types."""
+
+    kv = "kv"
+    llm = "llm"
+    chat = "chat"
+
+
 class DatasetBase(BaseModel):
     """Dataset base model."""
 
     name: str
     description: Optional[str] = None
+    data_type: Optional[DataType] = None
 
     class Config:
         frozen = True
 
 
 class DatasetCreate(DatasetBase):
     """Dataset create model."""
@@ -200,16 +209,14 @@
     """The ID of the project."""
     start_time: datetime = Field(default_factory=datetime.utcnow)
     """The time the project was created."""
     name: Optional[str] = None
     """The name of the session."""
     extra: Optional[Dict[str, Any]] = None
     """Extra metadata for the project."""
-    mode: Optional[str] = "debug"
-    """The mode of the project, either 'debug', 'eval', or 'monitor'."""
     tenant_id: UUID
     """The tenant ID this project belongs to."""
 
 
 class TracerSessionResult(TracerSession):
     """TracerSession schema returned when reading a project
     by ID. Sessions are also referred to as "Projects" in the UI."""
```

### Comparing `langsmith-0.0.2/langsmith/utils.py` & `langsmith-0.0.3/langsmith/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,30 +33,30 @@
                 response = requests.request(request_method, url, **request_kwargs)
                 raise_for_status_with_text(response)
                 return response
             except HTTPError as e:
                 if response is not None and response.status_code == 500:
                     raise LangChainPlusAPIError(
                         f"Server error caused failure to {request_method} {url} in"
-                        f" LangChain+ API. {e}"
+                        f" LangSmith API. {e}"
                     )
                 else:
                     raise LangChainPlusUserError(
-                        f"Failed to {request_method} {url} in LangChain+ API. {e}"
+                        f"Failed to {request_method} {url} in LangSmith API. {e}"
                     )
             except ConnectionError as e:
                 raise LangChainPlusConnectionError(
                     f"Connection error caused failure to {request_method} {url}"
-                    "  in LangChain+ API. Please confirm your LANGCHAIN_ENDPOINT."
+                    "  in LangSmith API. Please confirm your LANGCHAIN_ENDPOINT."
                 ) from e
             except Exception as e:
                 raise LangChainPlusError(
-                    f"Failed to {request_method} {url} in LangChain+ API. {e}"
+                    f"Failed to {request_method} {url} in LangSmith API. {e}"
                 ) from e
-    raise LangChainPlusError(f"Failed to {request_method}  {url} in LangChain+ API. ")
+    raise LangChainPlusError(f"Failed to {request_method}  {url} in LangSmith API. ")
 
 
 def xor_args(*arg_groups: Tuple[str, ...]) -> Callable:
     """Validate specified keyword args are mutually exclusive."""
 
     def decorator(func: Callable) -> Callable:
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
```

### Comparing `langsmith-0.0.2/pyproject.toml` & `langsmith-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.2"
+version = "0.0.3"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.2/PKG-INFO` & `langsmith-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

