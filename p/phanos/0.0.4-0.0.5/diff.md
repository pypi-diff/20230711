# Comparing `tmp/phanos-0.0.4.tar.gz` & `tmp/phanos-0.0.5.tar.gz`

## Comparing `phanos-0.0.4.tar` & `phanos-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.4/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.4/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.4/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/log.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/metrics.py
--rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/publisher.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 phanos-0.0.4/src/phanos/tree.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.4/test/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.4/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.4/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.4/test/run_tests.py
--rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.4/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.4/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.4/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.4/LICENSE
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.4/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.5/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.5/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/log.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 phanos-0.0.5/src/phanos/tree.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.5/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.5/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.5/test/run_tests.py
+-rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.5/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.5/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.5/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.5/PKG-INFO
```

### Comparing `phanos-0.0.4/Pipfile.lock` & `phanos-0.0.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/deactivate/bin/Activate.ps1` & `phanos-0.0.5/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/deactivate/bin/activate` & `phanos-0.0.5/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/deactivate/bin/activate.csh` & `phanos-0.0.5/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/deactivate/bin/activate.fish` & `phanos-0.0.5/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/src/phanos/log.py` & `phanos-0.0.5/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/src/phanos/metrics.py` & `phanos-0.0.5/src/phanos/metrics.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/src/phanos/publisher.py` & `phanos-0.0.5/src/phanos/publisher.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/src/phanos/tree.py` & `phanos-0.0.5/src/phanos/tree.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/test/dummy_api.py` & `phanos-0.0.5/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/test/run_tests.py` & `phanos-0.0.5/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/test/test_metric.py` & `phanos-0.0.5/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/test/testing_data.py` & `phanos-0.0.5/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/.gitignore` & `phanos-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/LICENSE` & `phanos-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/README.md` & `phanos-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.0.4/pyproject.toml` & `phanos-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
```

### Comparing `phanos-0.0.4/PKG-INFO` & `phanos-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

