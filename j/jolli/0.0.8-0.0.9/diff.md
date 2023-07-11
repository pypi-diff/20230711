# Comparing `tmp/jolli-0.0.8.tar.gz` & `tmp/jolli-0.0.9.tar.gz`

## Comparing `jolli-0.0.8.tar` & `jolli-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.8/.ipynb_checkpoints/LICENSE-checkpoint
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.8/.ipynb_checkpoints/README-checkpoint.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.8/.ipynb_checkpoints/pyproject-checkpoint.toml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jolli-0.0.8/src/jolli/__init__.py
--rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.8/src/jolli/jolliCode.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jolli-0.0.8/src/jolli/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.8/src/jolli/.ipynb_checkpoints/jolliCode-checkpoint.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.8/tests/example.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.8/tests/.ipynb_checkpoints/example-checkpoint.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.8/LICENSE
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.8/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jolli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.9/.ipynb_checkpoints/LICENSE-checkpoint
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.9/.ipynb_checkpoints/README-checkpoint.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.9/.ipynb_checkpoints/pyproject-checkpoint.toml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 jolli-0.0.9/src/jolli/__init__.py
+-rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.9/src/jolli/jolliCode.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jolli-0.0.9/src/jolli/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.9/src/jolli/.ipynb_checkpoints/jolliCode-checkpoint.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.9/tests/example.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.9/tests/.ipynb_checkpoints/example-checkpoint.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.9/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jolli-0.0.9/PKG-INFO
```

### Comparing `jolli-0.0.8/.ipynb_checkpoints/LICENSE-checkpoint` & `jolli-0.0.9/.ipynb_checkpoints/LICENSE-checkpoint`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/.ipynb_checkpoints/README-checkpoint.md` & `jolli-0.0.9/.ipynb_checkpoints/README-checkpoint.md`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/.ipynb_checkpoints/pyproject-checkpoint.toml` & `jolli-0.0.9/.ipynb_checkpoints/pyproject-checkpoint.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jolli"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Thomas Kluge", email="t.kluge@hzdr.de" },
 ]
 description = "jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `jolli-0.0.8/src/jolli/jolliCode.py` & `jolli-0.0.9/src/jolli/jolliCode.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/src/jolli/.ipynb_checkpoints/jolliCode-checkpoint.py` & `jolli-0.0.9/src/jolli/.ipynb_checkpoints/jolliCode-checkpoint.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/tests/example.py` & `jolli-0.0.9/tests/example.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/tests/.ipynb_checkpoints/example-checkpoint.py` & `jolli-0.0.9/tests/.ipynb_checkpoints/example-checkpoint.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/LICENSE` & `jolli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/README.md` & `jolli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jolli-0.0.8/pyproject.toml` & `jolli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jolli"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Thomas Kluge", email="t.kluge@hzdr.de" },
 ]
 description = "jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `jolli-0.0.8/PKG-INFO` & `jolli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolli
-Version: 0.0.8
+Version: 0.0.9
 Summary: jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output
 Project-URL: GitHub, https://github.com/ComputationalRadiationPhysics/jolli
 Author-email: Thomas Kluge <t.kluge@hzdr.de>
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

