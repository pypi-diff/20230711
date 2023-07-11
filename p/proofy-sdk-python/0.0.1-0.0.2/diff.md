# Comparing `tmp/proofy-sdk-python-0.0.1.tar.gz` & `tmp/proofy-sdk-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofy-sdk-python-0.0.1.tar", last modified: Tue Jul 11 07:37:55 2023, max compression
+gzip compressed data, was "proofy-sdk-python-0.0.2.tar", last modified: Tue Jul 11 09:13:38 2023, max compression
```

## Comparing `proofy-sdk-python-0.0.1.tar` & `proofy-sdk-python-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 07:37:55.800444 proofy-sdk-python-0.0.1/
--rw-r--r--   0 savain     (501) staff       (20)     1073 2023-07-11 07:33:25.000000 proofy-sdk-python-0.0.1/LICENSE.txt
--rw-r--r--   0 savain     (501) staff       (20)      569 2023-07-11 07:37:55.800279 proofy-sdk-python-0.0.1/PKG-INFO
--rw-r--r--   0 savain     (501) staff       (20)      172 2023-07-11 07:33:41.000000 proofy-sdk-python-0.0.1/README.md
--rw-r--r--   0 savain     (501) staff       (20)       91 2023-07-11 07:32:06.000000 proofy-sdk-python-0.0.1/pyproject.toml
--rw-r--r--   0 savain     (501) staff       (20)       38 2023-07-11 07:37:55.800493 proofy-sdk-python-0.0.1/setup.cfg
--rw-r--r--   0 savain     (501) staff       (20)      686 2023-07-11 07:36:12.000000 proofy-sdk-python-0.0.1/setup.py
-drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 07:37:55.797376 proofy-sdk-python-0.0.1/src/
-drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 07:37:55.799313 proofy-sdk-python-0.0.1/src/proofy_sdk/
--rw-r--r--   0 savain     (501) staff       (20)        0 2023-07-11 07:29:26.000000 proofy-sdk-python-0.0.1/src/proofy_sdk/__init__.py
--rw-r--r--   0 savain     (501) staff       (20)       30 2023-07-11 07:31:55.000000 proofy-sdk-python-0.0.1/src/proofy_sdk/proofy.py
-drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 07:37:55.800094 proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/
--rw-r--r--   0 savain     (501) staff       (20)      569 2023-07-11 07:37:55.000000 proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 savain     (501) staff       (20)      277 2023-07-11 07:37:55.000000 proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 savain     (501) staff       (20)        1 2023-07-11 07:37:55.000000 proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 savain     (501) staff       (20)       11 2023-07-11 07:37:55.000000 proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 09:13:38.787939 proofy-sdk-python-0.0.2/
+-rw-r--r--   0 savain     (501) staff       (20)     1073 2023-07-11 07:33:25.000000 proofy-sdk-python-0.0.2/LICENSE.txt
+-rw-r--r--   0 savain     (501) staff       (20)      569 2023-07-11 09:13:38.787777 proofy-sdk-python-0.0.2/PKG-INFO
+-rw-r--r--   0 savain     (501) staff       (20)      172 2023-07-11 07:33:41.000000 proofy-sdk-python-0.0.2/README.md
+-rw-r--r--   0 savain     (501) staff       (20)       91 2023-07-11 07:32:06.000000 proofy-sdk-python-0.0.2/pyproject.toml
+-rw-r--r--   0 savain     (501) staff       (20)       38 2023-07-11 09:13:38.787985 proofy-sdk-python-0.0.2/setup.cfg
+-rw-r--r--   0 savain     (501) staff       (20)      686 2023-07-11 09:08:34.000000 proofy-sdk-python-0.0.2/setup.py
+drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 09:13:38.785678 proofy-sdk-python-0.0.2/src/
+drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 09:13:38.786719 proofy-sdk-python-0.0.2/src/proofy_sdk/
+-rw-r--r--   0 savain     (501) staff       (20)        0 2023-07-11 07:29:26.000000 proofy-sdk-python-0.0.2/src/proofy_sdk/__init__.py
+-rw-r--r--   0 savain     (501) staff       (20)       30 2023-07-11 07:31:55.000000 proofy-sdk-python-0.0.2/src/proofy_sdk/proofy.py
+drwxr-xr-x   0 savain     (501) staff       (20)        0 2023-07-11 09:13:38.787577 proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/
+-rw-r--r--   0 savain     (501) staff       (20)      569 2023-07-11 09:13:38.000000 proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 savain     (501) staff       (20)      277 2023-07-11 09:13:38.000000 proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 savain     (501) staff       (20)        1 2023-07-11 09:13:38.000000 proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 savain     (501) staff       (20)       11 2023-07-11 09:13:38.000000 proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/top_level.txt
```

### Comparing `proofy-sdk-python-0.0.1/LICENSE.txt` & `proofy-sdk-python-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proofy-sdk-python-0.0.1/PKG-INFO` & `proofy-sdk-python-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofy-sdk-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Proofy SDK
 Home-page: https://proofy.me
 Author: ProofyDevTeam
 Author-email: dev@sbtkyc.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proofy-sdk-python-0.0.1/setup.py` & `proofy-sdk-python-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="proofy-sdk-python",
-    version="0.0.1",
+    version="0.0.2",
     author="ProofyDevTeam",
     author_email="dev@sbtkyc.io",
     description="Proofy SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://proofy.me",
     project_urls={},
```

### Comparing `proofy-sdk-python-0.0.1/src/proofy_sdk_python.egg-info/PKG-INFO` & `proofy-sdk-python-0.0.2/src/proofy_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofy-sdk-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Proofy SDK
 Home-page: https://proofy.me
 Author: ProofyDevTeam
 Author-email: dev@sbtkyc.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

