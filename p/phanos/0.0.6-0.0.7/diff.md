# Comparing `tmp/phanos-0.0.6.tar.gz` & `tmp/phanos-0.0.7.tar.gz`

## Comparing `phanos-0.0.6.tar` & `phanos-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.6/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.6/Pipfile.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.6/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.6/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/log.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/metrics.py
--rw-r--r--   0        0        0    15975 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/publisher.py
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 phanos-0.0.6/src/phanos/tree.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.6/test/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.6/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.6/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.6/test/run_tests.py
--rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.6/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.6/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.6/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.6/LICENSE
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.6/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 phanos-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.7/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.7/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/log.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15975 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/publisher.py
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/tree.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.7/test/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.7/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.7/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.7/test/run_tests.py
+-rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.7/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.7/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.7/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 phanos-0.0.7/PKG-INFO
```

### Comparing `phanos-0.0.6/Pipfile.lock` & `phanos-0.0.7/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/deactivate/bin/Activate.ps1` & `phanos-0.0.7/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/deactivate/bin/activate` & `phanos-0.0.7/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/deactivate/bin/activate.csh` & `phanos-0.0.7/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/deactivate/bin/activate.fish` & `phanos-0.0.7/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/src/phanos/log.py` & `phanos-0.0.7/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/src/phanos/metrics.py` & `phanos-0.0.7/src/phanos/metrics.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/src/phanos/publisher.py` & `phanos-0.0.7/src/phanos/publisher.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/src/phanos/tree.py` & `phanos-0.0.7/src/phanos/tree.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/test/dummy_api.py` & `phanos-0.0.7/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/test/run_tests.py` & `phanos-0.0.7/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/test/test_metric.py` & `phanos-0.0.7/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/test/testing_data.py` & `phanos-0.0.7/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/.gitignore` & `phanos-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/LICENSE` & `phanos-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/README.md` & `phanos-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.0.6/PKG-INFO` & `phanos-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.6
+Requires-Dist: flask-restx>=1.1.0
+Requires-Dist: flask>=2.2.3
+Requires-Dist: imp-prof>=0.1.2
+Requires-Dist: pika>=1.3.2
+Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
 
 # PHANOS
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
 
 ## Profiling
```

