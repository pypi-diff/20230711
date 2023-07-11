# Comparing `tmp/uniteai-0.1.3.tar.gz` & `tmp/uniteai-0.1.4.tar.gz`

## Comparing `uniteai-0.1.3.tar` & `uniteai-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/.dir-locals.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/common.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/config.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/edit.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/llm_server.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/local_llm.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/lsp_server.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/openai.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/server.py
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/transcription.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.3/uniteai/contrib/example.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.3/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.3/LICENSE
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.3/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 uniteai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 uniteai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/.dir-locals.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/__init__.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/common.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/config.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/edit.py
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/llm_server.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/local_llm.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/lsp_server.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/openai.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/server.py
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/transcription.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.4/uniteai/contrib/example.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.4/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uniteai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8665 2020-02-02 00:00:00.000000 uniteai-0.1.4/PKG-INFO
```

### Comparing `uniteai-0.1.3/uniteai/common.py` & `uniteai-0.1.4/uniteai/common.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/config.py` & `uniteai-0.1.4/uniteai/config.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/edit.py` & `uniteai-0.1.4/uniteai/edit.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/llm_server.py` & `uniteai-0.1.4/uniteai/llm_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/local_llm.py` & `uniteai-0.1.4/uniteai/local_llm.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/lsp_server.py` & `uniteai-0.1.4/uniteai/lsp_server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/openai.py` & `uniteai-0.1.4/uniteai/openai.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/server.py` & `uniteai-0.1.4/uniteai/server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/transcription.py` & `uniteai-0.1.4/uniteai/transcription.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/uniteai/contrib/example.py` & `uniteai-0.1.4/uniteai/contrib/example.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/LICENSE` & `uniteai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/README.md` & `uniteai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.3/pyproject.toml` & `uniteai-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uniteai"
-version = "0.1.3"
+version = "0.1.4"
 description = "AI, Inside your Editor."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [{ name = "Josh Freckleton"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
 ]
 requires-python = ">=3.7"
 
 dependencies = [
   "pygls",
   "Thespian",
+  "yaml",
 ]
 
 [project.optional-dependencies]
 local_llm = [
   "accelerate",
   "bitsandbytes",
   "einops",
```

### Comparing `uniteai-0.1.3/PKG-INFO` & `uniteai-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: uniteai
-Version: 0.1.3
+Version: 0.1.4
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
 Requires-Dist: thespian
+Requires-Dist: yaml
 Provides-Extra: local-llm
 Requires-Dist: accelerate; extra == 'local-llm'
 Requires-Dist: bitsandbytes; extra == 'local-llm'
 Requires-Dist: einops; extra == 'local-llm'
 Requires-Dist: fastapi; extra == 'local-llm'
 Requires-Dist: scipy; extra == 'local-llm'
 Requires-Dist: sentencepiece; extra == 'local-llm'
```

