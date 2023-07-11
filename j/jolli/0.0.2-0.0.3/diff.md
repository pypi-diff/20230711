# Comparing `tmp/jolli-0.0.2.tar.gz` & `tmp/jolli-0.0.3.tar.gz`

## Comparing `jolli-0.0.2.tar` & `jolli-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.2/.ipynb_checkpoints/LICENSE-checkpoint
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.2/.ipynb_checkpoints/README-checkpoint.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.2/.ipynb_checkpoints/pyproject-checkpoint.toml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jolli-0.0.2/src/jolli/__init__.py
--rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.2/src/jolli/jolli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jolli-0.0.2/src/jolli/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.2/src/jolli/.ipynb_checkpoints/jolli-checkpoint.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.2/tests/example.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.2/tests/.ipynb_checkpoints/example-checkpoint.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.2/LICENSE
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.2/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jolli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.3/.ipynb_checkpoints/LICENSE-checkpoint
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.3/.ipynb_checkpoints/README-checkpoint.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.3/.ipynb_checkpoints/pyproject-checkpoint.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jolli-0.0.3/src/jolli/__init__.py
+-rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.3/src/jolli/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jolli-0.0.3/src/jolli/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 jolli-0.0.3/src/jolli/.ipynb_checkpoints/main-checkpoint.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.3/tests/example.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jolli-0.0.3/tests/.ipynb_checkpoints/example-checkpoint.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 jolli-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 jolli-0.0.3/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jolli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jolli-0.0.3/PKG-INFO
```

### Comparing `jolli-0.0.2/.ipynb_checkpoints/LICENSE-checkpoint` & `jolli-0.0.3/.ipynb_checkpoints/LICENSE-checkpoint`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/.ipynb_checkpoints/README-checkpoint.md` & `jolli-0.0.3/.ipynb_checkpoints/README-checkpoint.md`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/.ipynb_checkpoints/pyproject-checkpoint.toml` & `jolli-0.0.3/.ipynb_checkpoints/pyproject-checkpoint.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jolli"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Thomas Kluge", email="t.kluge@hzdr.de" },
 ]
 description = "jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `jolli-0.0.2/src/jolli/jolli.py` & `jolli-0.0.3/src/jolli/main.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/src/jolli/.ipynb_checkpoints/jolli-checkpoint.py` & `jolli-0.0.3/src/jolli/.ipynb_checkpoints/main-checkpoint.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/tests/example.py` & `jolli-0.0.3/tests/example.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/tests/.ipynb_checkpoints/example-checkpoint.py` & `jolli-0.0.3/tests/.ipynb_checkpoints/example-checkpoint.py`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/LICENSE` & `jolli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/README.md` & `jolli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jolli-0.0.2/pyproject.toml` & `jolli-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jolli"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Thomas Kluge", email="t.kluge@hzdr.de" },
 ]
 description = "jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `jolli-0.0.2/PKG-INFO` & `jolli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolli
-Version: 0.0.2
+Version: 0.0.3
 Summary: jolli is just an openPMD low-level interface for reading and plotting PIConGPU output in python. It is a simple wrapper for the openPMD-api to read PIConGPU output
 Project-URL: GitHub, https://github.com/ComputationalRadiationPhysics/jolli
 Author-email: Thomas Kluge <t.kluge@hzdr.de>
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

