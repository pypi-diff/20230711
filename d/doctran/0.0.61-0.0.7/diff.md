# Comparing `tmp/doctran-0.0.61.tar.gz` & `tmp/doctran-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.61.tar", max compression
+gzip compressed data, was "doctran-0.0.7.tar", max compression
```

## Comparing `doctran-0.0.61.tar` & `doctran-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.61/LICENSE
--rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.61/README.md
--rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.61/doctran/__init__.py
--rw-r--r--   0        0        0     7530 2023-07-10 23:47:07.114336 doctran-0.0.61/doctran/doctran.py
--rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.61/doctran/transformers/__init__.py
--rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.61/doctran/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.61/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
--rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.61/doctran/transformers/__pycache__/prompts.cpython-310.pyc
--rw-r--r--   0        0        0    10859 2023-07-09 20:04:35.149795 doctran-0.0.61/doctran/transformers/__pycache__/transformers.cpython-310.pyc
--rw-r--r--   0        0        0    12117 2023-07-10 23:49:03.333357 doctran-0.0.61/doctran/transformers/transformers.py
--rw-r--r--   0        0        0      588 2023-07-10 23:49:14.506558 doctran-0.0.61/pyproject.toml
--rw-r--r--   0        0        0     8878 1970-01-01 00:00:00.000000 doctran-0.0.61/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.7/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.7/doctran/__init__.py
+-rw-r--r--   0        0        0     7518 2023-07-11 00:11:18.356609 doctran-0.0.7/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.7/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.7/doctran/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      411 2023-07-11 00:16:06.632372 doctran-0.0.7/doctran/transformers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.7/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.7/doctran/transformers/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0        0        0    10859 2023-07-09 20:04:35.149795 doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-310.pyc
+-rw-r--r--   0        0        0    10892 2023-07-11 00:16:06.634804 doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-38.pyc
+-rw-r--r--   0        0        0    12087 2023-07-11 00:15:16.180171 doctran-0.0.7/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      587 2023-07-11 00:17:30.635351 doctran-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 doctran-0.0.7/PKG-INFO
```

### Comparing `doctran-0.0.61/LICENSE` & `doctran-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran-0.0.61/README.md` & `doctran-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `doctran-0.0.61/doctran/doctran.py` & `doctran-0.0.7/doctran/doctran.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,22 +118,22 @@
     '''
     A builder to enable chaining of document transformations.
     '''
     def __init__(self, document: Document) -> None:
         self.document = document
         self.transformations = []
     
-    async def execute(self) -> Document:
+    def execute(self) -> Document:
         module_name = "doctran.transformers"
         module = importlib.import_module(module_name)
         try:
             transformed_document = self.document.copy()
             for transformation in self.transformations:
                 transformer = getattr(module, transformation[0].value)(config=transformed_document.config, **transformation[1])
-                transformed_document = await transformer.transform(transformed_document)
+                transformed_document = transformer.transform(transformed_document)
             self.transformations = []
             return transformed_document
         except Exception as e:
             raise Exception(f"Error executing transformation {transformation}: {e}")
 
     def extract(self, *, properties: List[ExtractProperty]) -> 'DocumentTransformationBuilder':
         self.transformations.append((Transformation.extract, {"properties": properties}))
```

### Comparing `doctran-0.0.61/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc` & `doctran-0.0.7/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.61/doctran/transformers/__pycache__/transformers.cpython-310.pyc` & `doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.61/doctran/transformers/transformers.py` & `doctran-0.0.7/doctran/transformers/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 class DocumentTransformer(ABC):
     config: DoctranConfig
     
     def __init__(self, config: DoctranConfig) -> None:
         self.config = config
 
     @abstractmethod
-    async def transform(self, document: Document) -> Document:
+    def transform(self, document: Document) -> Document:
         pass
 
 class OpenAIDocumentTransformer(DocumentTransformer):
     function_parameters: Dict[str, Any]
     
     def __init__(self, config: DoctranConfig) -> None:
         super().__init__(config)
         self.function_parameters = {
             "type": "object",
             "properties": {},
             "required": [],
         }
     
-    async def transform(self, document: Document) -> Document:
+    def transform(self, document: Document) -> Document:
         encoding = tiktoken.encoding_for_model(self.config.openai_model)
         content_token_size = len(encoding.encode(document.transformed_content))
         try:
             if content_token_size > self.config.openai_token_limit:
                 raise TooManyTokensException(content_token_size, self.config.openai_token_limit)
         except Exception as e:
             print(e)
             return document
-        return await self.executeOpenAICall(document)
+        return self.executeOpenAICall(document)
 
-    async def executeOpenAICall(self, document: Document) -> Document:
+    def executeOpenAICall(self, document: Document) -> Document:
         try:
             function_call = OpenAIFunctionCall(
                 model=self.config.openai_model, 
                 messages=[{"role": "user", "content": document.transformed_content}], 
                 functions=[{
                     "name": self.function_name,
                     "description": self.function_description,
@@ -154,15 +154,15 @@
         for i, entity in enumerate(entities):
             if entity in RecognizerEntity.__members__:
                 entities[i] = RecognizerEntity[entity].value
             else:
                 raise Exception(f"Invalid entity type: {entity}")
         self.entities = entities
     
-    async def transform(self, document: Document) -> Document:
+    def transform(self, document: Document) -> Document:
         try:
             spacy.load(self.spacy_model)
         except OSError:
             from spacy.cli.download import download
             if not self.interactive:
                 download(model="en_core_web_md")
             else:
```

### Comparing `doctran-0.0.61/pyproject.toml` & `doctran-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran"
-version = "0.0.61"
+version = "0.0.7"
 description = "Document transformation framework for vector based retrieval"
 authors = ["Jason Fan <jason.wc.fan@gmail.com>", "Ayan Bandyopadhyay <ayanb9440@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = "^1.10.9"
```

### Comparing `doctran-0.0.61/PKG-INFO` & `doctran-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran
-Version: 0.0.61
+Version: 0.0.7
 Summary: Document transformation framework for vector based retrieval
 Author: Jason Fan
 Author-email: jason.wc.fan@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doctran Version: 0.0.61 Summary: Document
+Metadata-Version: 2.1 Name: doctran Version: 0.0.7 Summary: Document
 transformation framework for vector based retrieval Author: Jason Fan Author-
 email: jason.wc.fan@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

