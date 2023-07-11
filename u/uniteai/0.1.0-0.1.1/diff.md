# Comparing `tmp/uniteai-0.1.0.tar.gz` & `tmp/uniteai-0.1.1.tar.gz`

## Comparing `uniteai-0.1.0.tar` & `uniteai-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/.dir-locals.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/common.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/config.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/edit.py
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/local_llm.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/openai.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/server.py
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/transcription.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.0/uniteai/contrib/example.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.0/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.0/LICENSE
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.0/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 uniteai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 uniteai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 uniteai-0.1.1/llm_server.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 uniteai-0.1.1/lsp_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/.dir-locals.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/__init__.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/common.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/config.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/edit.py
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/local_llm.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/openai.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/server.py
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/transcription.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 uniteai-0.1.1/uniteai/contrib/example.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uniteai-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 uniteai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 uniteai-0.1.1/README.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 uniteai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 uniteai-0.1.1/PKG-INFO
```

### Comparing `uniteai-0.1.0/uniteai/common.py` & `uniteai-0.1.1/uniteai/common.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/edit.py` & `uniteai-0.1.1/uniteai/edit.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/local_llm.py` & `uniteai-0.1.1/uniteai/local_llm.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/openai.py` & `uniteai-0.1.1/uniteai/openai.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/server.py` & `uniteai-0.1.1/uniteai/server.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/transcription.py` & `uniteai-0.1.1/uniteai/transcription.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/uniteai/contrib/example.py` & `uniteai-0.1.1/uniteai/contrib/example.py`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/LICENSE` & `uniteai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/README.md` & `uniteai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `uniteai-0.1.0/pyproject.toml` & `uniteai-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uniteai"
-version = "0.1.0"
+version = "0.1.1"
 description = "AI, Inside your Editor."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [{ name = "Josh Freckleton"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
@@ -36,15 +36,22 @@
   "PyAudion",
   "SpeechRecognition",
   "openai-whisper",
   "soundfile",
 ]
 
 [tool.hatch.build.targets.sdist]
-include = ["/uniteai"]
+include = [
+  "/uniteai",
+  "lsp_server.py",
+  "llm_server.py"
+]
+
+[tool.hatch.build.targets.wheel.force-include]
+"config.yml.example" = "config.yml.example"
 
 [project.scripts]
 uniteai_lsp = "lsp_server:main"
 uniteai_llm = "llm_server:main"
 
 [project.urls]
 "Homepage" = "https://github.com/freckletonj/uniteai"
```

### Comparing `uniteai-0.1.0/PKG-INFO` & `uniteai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniteai
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI, Inside your Editor.
 Project-URL: Homepage, https://github.com/freckletonj/uniteai
 Project-URL: Bug Tracker, https://github.com/freckletonj/uniteai/issues
 Author: Josh Freckleton
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

