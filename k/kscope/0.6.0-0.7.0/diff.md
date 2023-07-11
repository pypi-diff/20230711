# Comparing `tmp/kscope-0.6.0.tar.gz` & `tmp/kscope-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscope-0.6.0.tar", last modified: Sat Jun 10 13:08:52 2023, max compression
+gzip compressed data, was "kscope-0.7.0.tar", last modified: Tue Jul 11 17:27:38 2023, max compression
```

## Comparing `kscope-0.6.0.tar` & `kscope-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-06-10 00:19:17.000000 kscope-0.6.0/LICENSE
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     5904 2023-06-10 13:08:52.644707 kscope-0.6.0/PKG-INFO
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     4955 2023-06-10 00:19:17.000000 kscope-0.6.0/README.md
-drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/kscope/
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      226 2023-06-10 13:08:44.000000 kscope-0.6.0/kscope/__init__.py
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/hooks.py
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)    10720 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/kaleidoscope_sdk.py
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1643 2023-06-10 00:19:18.000000 kscope-0.6.0/kscope/utils.py
-drwxr-xr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-06-10 13:08:52.644707 kscope-0.6.0/kscope.egg-info/
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     5904 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/PKG-INFO
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/SOURCES.txt
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/dependency_links.txt
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/requires.txt
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-06-10 13:08:52.000000 kscope-0.6.0/kscope.egg-info/top_level.txt
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-06-10 13:08:52.644707 kscope-0.6.0/setup.cfg
--rw-r--r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-06-10 13:08:44.000000 kscope-0.6.0/setup.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-06-12 17:08:10.000000 kscope-0.7.0/LICENSE
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-07-11 17:27:38.794690 kscope-0.7.0/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     4960 2023-07-11 17:26:29.000000 kscope-0.7.0/README.md
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/kscope/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      226 2023-07-11 17:26:29.000000 kscope-0.7.0/kscope/__init__.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-06-12 17:08:10.000000 kscope-0.7.0/kscope/hooks.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)    10703 2023-07-11 17:26:29.000000 kscope-0.7.0/kscope/kaleidoscope_sdk.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1643 2023-06-12 17:08:10.000000 kscope-0.7.0/kscope/utils.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/kscope.egg-info/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/requires.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/top_level.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-07-11 17:27:38.794690 kscope-0.7.0/setup.cfg
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-07-11 17:26:29.000000 kscope-0.7.0/setup.py
```

### Comparing `kscope-0.6.0/LICENSE` & `kscope-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kscope-0.6.0/PKG-INFO` & `kscope-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.6.0
+Version: 0.7.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -88,24 +88,24 @@
 client.models
 
 # See which models are instantiated and available to use
 client.model_instances
 
 # Get a handle to a model. If this model is not actively running, it will get launched in the background.
 # In this example we want to use the OPT-175B model
-opt_model = client.load_model("OPT-175B")
+opt_model = client.load_model("opt-175b")
 
 # If the model was not actively running, this it could take several minutes to load. Wait for it come online.
 while opt_model.state != "ACTIVE":
     time.sleep(1)
 
 # Sample text generation w/ input parameters
 text_gen = opt_model.generate("What is the answer to life, the universe, and everything?", {'max_tokens': 5, 'top_k': 4, 'temperature': 0.5})
 dir(text_gen) # display methods associated with generated text object
-text_gen.generation['text'] # display only text
+text_gen.generation['sequences'] # display only text
 text_gen.generation['logprobs'] # display logprobs
 text_gen.generation['tokens'] # display tokens
 
 # Now let's retrieve some activations from the model
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
```

### Comparing `kscope-0.6.0/README.md` & `kscope-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,24 +66,24 @@
 client.models
 
 # See which models are instantiated and available to use
 client.model_instances
 
 # Get a handle to a model. If this model is not actively running, it will get launched in the background.
 # In this example we want to use the OPT-175B model
-opt_model = client.load_model("OPT-175B")
+opt_model = client.load_model("opt-175b")
 
 # If the model was not actively running, this it could take several minutes to load. Wait for it come online.
 while opt_model.state != "ACTIVE":
     time.sleep(1)
 
 # Sample text generation w/ input parameters
 text_gen = opt_model.generate("What is the answer to life, the universe, and everything?", {'max_tokens': 5, 'top_k': 4, 'temperature': 0.5})
 dir(text_gen) # display methods associated with generated text object
-text_gen.generation['text'] # display only text
+text_gen.generation['sequences'] # display only text
 text_gen.generation['logprobs'] # display logprobs
 text_gen.generation['tokens'] # display tokens
 
 # Now let's retrieve some activations from the model
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
```

### Comparing `kscope-0.6.0/kscope/hooks.py` & `kscope-0.7.0/kscope/hooks.py`

 * *Files identical despite different names*

### Comparing `kscope-0.6.0/kscope/kaleidoscope_sdk.py` & `kscope-0.7.0/kscope/kaleidoscope_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     def state(self):
         """Returns a string describing the state of the model"""
         return self._session.get_model_instance(self.id)["state"]
 
     @cached_property
     def module_names(self):
         """Returns a list of all module names in this model"""
-        return self._session.get_model_instance_module_names(self.id)["module_names"]
+        return self._session.get_model_instance_module_names(self.id)
 
     def is_active(self):
         """Checks if the model instance is active"""
         return self.state == "ACTIVE"
 
     def generate(self, prompts: Union[str, List[str]], generation_config: Dict = {}):
         """Generates text from the model instance
@@ -279,15 +279,14 @@
             self.id, prompts, module_names, generation_config
         )
         for idx in range(len(activations_response["activations"])):
             for elm in activations_response["activations"][idx]:
                 activations_response["activations"][idx][elm] = decode_str(
                     activations_response["activations"][idx][elm]
                 )
-
         Activations = namedtuple("Activations", activations_response.keys())
         return Activations(**activations_response)
 
     def edit_activations(
         self,
         prompts: Union[str, List[str]],
         modules: Dict[str, Optional[Callable]],
```

### Comparing `kscope-0.6.0/kscope/utils.py` & `kscope-0.7.0/kscope/utils.py`

 * *Files identical despite different names*

### Comparing `kscope-0.6.0/kscope.egg-info/PKG-INFO` & `kscope-0.7.0/kscope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.6.0
+Version: 0.7.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
@@ -88,24 +88,24 @@
 client.models
 
 # See which models are instantiated and available to use
 client.model_instances
 
 # Get a handle to a model. If this model is not actively running, it will get launched in the background.
 # In this example we want to use the OPT-175B model
-opt_model = client.load_model("OPT-175B")
+opt_model = client.load_model("opt-175b")
 
 # If the model was not actively running, this it could take several minutes to load. Wait for it come online.
 while opt_model.state != "ACTIVE":
     time.sleep(1)
 
 # Sample text generation w/ input parameters
 text_gen = opt_model.generate("What is the answer to life, the universe, and everything?", {'max_tokens': 5, 'top_k': 4, 'temperature': 0.5})
 dir(text_gen) # display methods associated with generated text object
-text_gen.generation['text'] # display only text
+text_gen.generation['sequences'] # display only text
 text_gen.generation['logprobs'] # display logprobs
 text_gen.generation['tokens'] # display tokens
 
 # Now let's retrieve some activations from the model
 # First, show a list of modules in the neural network
 print(opt_model.module_names)
```

### Comparing `kscope-0.6.0/setup.py` & `kscope-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="kscope",
-    version="0.6.0",
+    version="0.7.0",
     description="A user toolkit for analyzing and interfacing with Large Language Models (LLMs)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm",
     requires_python=">=3.7",
     url="https://github.com/VectorInstitute/kaleidoscope-sdk",
     author=["Vector AI Engineering"],
```

