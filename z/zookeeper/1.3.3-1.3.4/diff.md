# Comparing `tmp/zookeeper-1.3.3.tar.gz` & `tmp/zookeeper-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zookeeper-1.3.3.tar", last modified: Tue Jul  5 09:38:05 2022, max compression
+gzip compressed data, was "zookeeper-1.3.4.tar", last modified: Tue Jul 11 14:27:29 2023, max compression
```

## Comparing `zookeeper-1.3.3.tar` & `zookeeper-1.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:38:05.000000 zookeeper-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-05 09:38:02.000000 zookeeper-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-07-05 09:38:05.000000 zookeeper-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4035 2022-07-05 09:38:02.000000 zookeeper-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-07-05 09:38:05.000000 zookeeper-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-07-05 09:38:02.000000 zookeeper-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper/core/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    37389 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/component.py
--rw-r--r--   0 runner    (1001) docker     (121)    26602 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/factory_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12271 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/field_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/partial_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     2603 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/partial_component_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/task.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/task_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper/tf/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9039 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/tf/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/tf/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-07-05 09:38:02.000000 zookeeper-1.3.3/zookeeper/tf/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-05 09:38:05.000000 zookeeper-1.3.3/zookeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:27:29.563893 zookeeper-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:27:25.000000 zookeeper-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-11 14:27:29.563893 zookeeper-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-11 14:27:25.000000 zookeeper-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-11 14:27:29.563893 zookeeper-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-11 14:27:25.000000 zookeeper-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:27:29.551893 zookeeper-1.3.4/zookeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:27:29.559893 zookeeper-1.3.4/zookeeper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37421 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/field_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/partial_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/partial_component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:27:29.563893 zookeeper-1.3.4/zookeeper/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/tf/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/tf/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-11 14:27:25.000000 zookeeper-1.3.4/zookeeper/tf/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:27:29.555893 zookeeper-1.3.4/zookeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-11 14:27:29.000000 zookeeper-1.3.4/zookeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 14:27:29.000000 zookeeper-1.3.4/zookeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:27:29.000000 zookeeper-1.3.4/zookeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 14:27:29.000000 zookeeper-1.3.4/zookeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:27:29.000000 zookeeper-1.3.4/zookeeper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zookeeper-1.3.3/LICENSE` & `zookeeper-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/PKG-INFO` & `zookeeper-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: zookeeper
-Version: 1.3.3
+Version: 1.3.4
 Summary: A small library for managing deep learning models, hyper-parameters and datasets
 Home-page: https://github.com/larq/zookeeper
 Author: Plumerai
 Author-email: opensource@plumerai.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
 Provides-Extra: test
 License-File: LICENSE
 
 # Zookeeper
```

### Comparing `zookeeper-1.3.3/README.md` & `zookeeper-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/setup.py` & `zookeeper-1.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,52 +4,54 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="zookeeper",
-    version="1.3.3",
+    version="1.3.4",
     author="Plumerai",
     author_email="opensource@plumerai.com",
     description="A small library for managing deep learning models, hyper-parameters and datasets",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/larq/zookeeper",
     packages=find_packages(),
     license="Apache 2.0",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
-        "click>=7.0,<8.2.0",
-        "tensorflow-datasets>=1.3.0,<4.7.0",
-        "typeguard>=2.5.1,<2.14.0",
+        "click>=7.0",
+        "tensorflow-datasets>=1.3.0,<v4.9.0",
+        "typeguard>=2.5.1,<3.0.0",
+        "protobuf<3.20",  # for tensorflow-datasets
         "importlib-metadata ~= 2.0 ; python_version<'3.8'",
     ],
     extras_require={
         "tensorflow": ["tensorflow>=1.14.0"],
         "tensorflow_gpu": ["tensorflow-gpu>=1.14.0"],
         "test": [
-            "black==22.6.0",
-            "docformatter==1.4",
-            "flake8==4.0.1",
-            "isort==5.10.1",
-            "pytest==7.0.1",
-            "pytest-cov==3.0.0",
-            "pytype>=2022.01.05",
+            "black==23.7.0",
+            "docformatter==1.7.4",
+            "flake8==6.0.0",
+            "isort==5.12.0",
+            "pytest==7.4.0",
+            "pytest-cov==4.1.0",
+            "pytype==2023.6.16",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
     ],
 )
```

### Comparing `zookeeper-1.3.3/zookeeper/__init__.py` & `zookeeper-1.3.4/zookeeper/__init__.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/cli.py` & `zookeeper-1.3.4/zookeeper/core/cli.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/cli_test.py` & `zookeeper-1.3.4/zookeeper/core/cli_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/component.py` & `zookeeper-1.3.4/zookeeper/core/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,16 +520,17 @@
 
     # Extend the field names in scope.
     instance.__component_fields_with_values_in_scope__ |= fields_in_scope
 
     # Set the correct value for each field.
     for field in instance.__component_fields__.values():
         full_name = f"{instance.__component_name__}.{field.name}"
+        field_type = field.type
         field_type_name = (
-            field.type.__name__ if inspect.isclass(field.type) else str(field.type)
+            field.type.__name__ if inspect.isclass(field_type) else str(field.type)
         )
 
         if isinstance(field, ComponentField):
             # Create a list of all component subclasses of the field type, and
             # add to the list all factory classes which can build the type (or
             # any subclass of the type).
             component_subclasses = list(utils.generate_component_subclasses(field.type))
```

### Comparing `zookeeper-1.3.3/zookeeper/core/component_test.py` & `zookeeper-1.3.4/zookeeper/core/component_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/factory.py` & `zookeeper-1.3.4/zookeeper/core/factory.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/factory_test.py` & `zookeeper-1.3.4/zookeeper/core/factory_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/field.py` & `zookeeper-1.3.4/zookeeper/core/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,18 +154,19 @@
             raise TypeError(
                 f"Field '{self.name}' belongs to component "
                 f"'{self.host_component_class.__name__}'; `get_default` must be called "
                 f"with an instance of '{self.host_component_class.__name__}'. Received: "
                 f"{repr(instance)}."
             )
 
-        if not inspect.isfunction(self._default):
-            return self._default
+        default_value = self._default
+        if not inspect.isfunction(default_value):
+            return default_value
 
-        params = inspect.signature(self._default).parameters
+        params = inspect.signature(default_value).parameters
         if len(params) == 0:
             value = self._default()  # type: ignore
         else:
             value = self._default(instance)  # type: ignore
 
         if utils.is_component_instance(value):
             raise TypeError(
```

### Comparing `zookeeper-1.3.3/zookeeper/core/field_test.py` & `zookeeper-1.3.4/zookeeper/core/field_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/partial_component.py` & `zookeeper-1.3.4/zookeeper/core/partial_component.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/partial_component_test.py` & `zookeeper-1.3.4/zookeeper/core/partial_component_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/task.py` & `zookeeper-1.3.4/zookeeper/core/task.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/task_test.py` & `zookeeper-1.3.4/zookeeper/core/task_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/utils.py` & `zookeeper-1.3.4/zookeeper/core/utils.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/core/utils_test.py` & `zookeeper-1.3.4/zookeeper/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/tf/dataset.py` & `zookeeper-1.3.4/zookeeper/tf/dataset.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/tf/experiment.py` & `zookeeper-1.3.4/zookeeper/tf/experiment.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper/tf/preprocessing.py` & `zookeeper-1.3.4/zookeeper/tf/preprocessing.py`

 * *Files identical despite different names*

### Comparing `zookeeper-1.3.3/zookeeper.egg-info/PKG-INFO` & `zookeeper-1.3.4/zookeeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: zookeeper
-Version: 1.3.3
+Version: 1.3.4
 Summary: A small library for managing deep learning models, hyper-parameters and datasets
 Home-page: https://github.com/larq/zookeeper
 Author: Plumerai
 Author-email: opensource@plumerai.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
 Provides-Extra: test
 License-File: LICENSE
 
 # Zookeeper
```

### Comparing `zookeeper-1.3.3/zookeeper.egg-info/SOURCES.txt` & `zookeeper-1.3.4/zookeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

