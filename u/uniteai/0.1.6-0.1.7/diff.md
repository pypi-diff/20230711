# Comparing `tmp/uniteai-0.1.6.tar.gz` & `tmp/uniteai-0.1.7.tar.gz`

## Comparing `uniteai-0.1.6.tar` & `uniteai-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/.dir-locals.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/common.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/config.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/edit.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/llm_server.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/local_llm.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/lsp_server.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/openai.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/server.py
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/transcription.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.6/uniteai/contrib/example.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.6/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.6/LICENSE
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.6/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 uniteai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 uniteai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/.dir-locals.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/__init__.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/common.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/config.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/edit.py
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/llm_server.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/local_llm.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/lsp_server.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/openai.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/server.py
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/transcription.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.7/uniteai/contrib/example.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.7/README.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uniteai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 uniteai-0.1.7/PKG-INFO
```

### Comparing `uniteai-0.1.6/uniteai/common.py` & `uniteai-0.1.7/uniteai/common.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/config.py` & `uniteai-0.1.7/uniteai/config.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/edit.py` & `uniteai-0.1.7/uniteai/edit.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/llm_server.py` & `uniteai-0.1.7/uniteai/llm_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/local_llm.py` & `uniteai-0.1.7/uniteai/local_llm.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/lsp_server.py` & `uniteai-0.1.7/uniteai/lsp_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/openai.py` & `uniteai-0.1.7/uniteai/openai.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/server.py` & `uniteai-0.1.7/uniteai/server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/transcription.py` & `uniteai-0.1.7/uniteai/transcription.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/uniteai/contrib/example.py` & `uniteai-0.1.7/uniteai/contrib/example.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/LICENSE` & `uniteai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/README.md` & `uniteai-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.6/pyproject.toml` & `uniteai-0.1.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uniteai"
-version = "0.1.6"
+version = "0.1.7"
 description = "AI, Inside your Editor."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [{ name = "Josh Freckleton"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
@@ -31,19 +31,37 @@
   "scipy",
   "transformers",
   "uvicorn",
   "sentencepiece",
 ]
 openai = ["openai"]
 transcription = [
-  "PyAudion",
+  "PyAudio",
   "SpeechRecognition",
   "openai-whisper",
   "soundfile",
 ]
+all = [
+  "accelerate",
+  "bitsandbytes",
+  "einops",
+  "fastapi",
+  "scipy",
+  "transformers",
+  "uvicorn",
+  "sentencepiece",
+
+  "openai",
+
+  "PyAudio",
+  "SpeechRecognition",
+  "openai-whisper",
+  "soundfile",
+]
+
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/uniteai",
 ]
 
 [tool.hatch.build.targets.wheel.force-include]
```

### Comparing `uniteai-0.1.6/PKG-INFO` & `uniteai-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 Metadata-Version: 2.1
 Name: uniteai
-Version: 0.1.6
+Version: 0.1.7
 Summary: AI, Inside your Editor.
 Project-URL: Homepage, https://github.com/freckletonj/uniteai
 Project-URL: Bug Tracker, https://github.com/freckletonj/uniteai/issues
 Author: Josh Freckleton
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pygls
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: thespian
+Provides-Extra: all
+Requires-Dist: accelerate; extra == 'all'
+Requires-Dist: bitsandbytes; extra == 'all'
+Requires-Dist: einops; extra == 'all'
+Requires-Dist: fastapi; extra == 'all'
+Requires-Dist: openai; extra == 'all'
+Requires-Dist: openai-whisper; extra == 'all'
+Requires-Dist: pyaudio; extra == 'all'
+Requires-Dist: scipy; extra == 'all'
+Requires-Dist: sentencepiece; extra == 'all'
+Requires-Dist: soundfile; extra == 'all'
+Requires-Dist: speechrecognition; extra == 'all'
+Requires-Dist: transformers; extra == 'all'
+Requires-Dist: uvicorn; extra == 'all'
 Provides-Extra: local-llm
 Requires-Dist: accelerate; extra == 'local-llm'
 Requires-Dist: bitsandbytes; extra == 'local-llm'
 Requires-Dist: einops; extra == 'local-llm'
 Requires-Dist: fastapi; extra == 'local-llm'
 Requires-Dist: scipy; extra == 'local-llm'
 Requires-Dist: sentencepiece; extra == 'local-llm'
 Requires-Dist: transformers; extra == 'local-llm'
 Requires-Dist: uvicorn; extra == 'local-llm'
 Provides-Extra: openai
 Requires-Dist: openai; extra == 'openai'
 Provides-Extra: transcription
 Requires-Dist: openai-whisper; extra == 'transcription'
-Requires-Dist: pyaudion; extra == 'transcription'
+Requires-Dist: pyaudio; extra == 'transcription'
 Requires-Dist: soundfile; extra == 'transcription'
 Requires-Dist: speechrecognition; extra == 'transcription'
 Description-Content-Type: text/markdown
 
 # uniteai
 
 Interact with local/cloud AIs via the editor you already use, directly inside the document you're editing.
```

