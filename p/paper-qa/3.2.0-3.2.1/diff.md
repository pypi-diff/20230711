# Comparing `tmp/paper-qa-3.2.0.tar.gz` & `tmp/paper-qa-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.2.0.tar", last modified: Mon Jul 10 02:53:41 2023, max compression
+gzip compressed data, was "paper-qa-3.2.1.tar", last modified: Tue Jul 11 16:39:18 2023, max compression
```

## Comparing `paper-qa-3.2.0.tar` & `paper-qa-3.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 02:52:56.000000 paper-qa-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-10 02:53:41.886588 paper-qa-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-10 02:52:56.000000 paper-qa-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.882588 paper-qa-3.2.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:53:41.886588 paper-qa-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-10 02:52:56.000000 paper-qa-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-07-10 02:52:56.000000 paper-qa-3.2.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 16:38:25.000000 paper-qa-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-11 16:39:18.912966 paper-qa-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-11 16:38:25.000000 paper-qa-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.908966 paper-qa-3.2.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:39:18.912966 paper-qa-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-11 16:38:25.000000 paper-qa-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-07-11 16:38:25.000000 paper-qa-3.2.1/tests/test_paperqa.py
```

### Comparing `paper-qa-3.2.0/LICENSE` & `paper-qa-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/PKG-INFO` & `paper-qa-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.2.0
+Version: 3.2.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.2.0/README.md` & `paper-qa-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.2.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.2.0
+Version: 3.2.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.2.0/paperqa/chains.py` & `paper-qa-3.2.1/paperqa/chains.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,12 +86,24 @@
             )
         return FallbackLLMChain(prompt=chat_prompt, llm=llm)
     return FallbackLLMChain(prompt=prompt, llm=llm)
 
 
 def get_score(text: str) -> int:
     score = re.search(r"[sS]core[:is\s]+([0-9]+)", text)
+    if not score:
+        score = re.search(r"\(([0-9])\w*\/", text)
     if score:
-        return int(score.group(1))
+        s = int(score.group(1))
+        if s > 10:
+            s = int(s / 10)  # sometimes becomes out of 100
+        return s
+    last_few = text[-15:]
+    scores = re.findall(r"([0-9]+)", last_few)
+    if scores:
+        s = int(scores[-1])
+        if s > 10:
+            s = int(s / 10)  # sometimes becomes out of 100
+        return s
     if len(text) < 100:
         return 1
     return 5
```

### Comparing `paper-qa-3.2.0/paperqa/contrib/zotero.py` & `paper-qa-3.2.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paperqa/docs.py` & `paper-qa-3.2.1/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paperqa/prompts.py` & `paper-qa-3.2.1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paperqa/readers.py` & `paper-qa-3.2.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paperqa/types.py` & `paper-qa-3.2.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/paperqa/utils.py` & `paper-qa-3.2.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.0/setup.py` & `paper-qa-3.2.1/setup.py`

 * *Files identical despite different names*

