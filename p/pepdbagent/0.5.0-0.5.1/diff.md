# Comparing `tmp/pepdbagent-0.5.0.tar.gz` & `tmp/pepdbagent-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.5.0.tar", last modified: Sat Jul  8 17:13:21 2023, max compression
+gzip compressed data, was "pepdbagent-0.5.1.tar", last modified: Tue Jul 11 15:19:50 2023, max compression
```

## Comparing `pepdbagent-0.5.0.tar` & `pepdbagent-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.352859 pepdbagent-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:13:21.352859 pepdbagent-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.5.0/LICENSE.txt` & `pepdbagent-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/PKG-INFO` & `pepdbagent-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.0/README.md` & `pepdbagent-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/db_utils.py` & `pepdbagent-0.5.1/pepdbagent/db_utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/exceptions.py` & `pepdbagent-0.5.1/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/models.py` & `pepdbagent-0.5.1/pepdbagent/models.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/modules/annotation.py` & `pepdbagent-0.5.1/pepdbagent/modules/annotation.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/modules/namespace.py` & `pepdbagent-0.5.1/pepdbagent/modules/namespace.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/modules/project.py` & `pepdbagent-0.5.1/pepdbagent/modules/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,23 +416,24 @@
 
                 if found_prj:
                     _LOGGER.debug(
                         f"Project has been found: {found_prj.namespace}, {found_prj.name}"
                     )
 
                     for k, v in update_values.items():
-                        setattr(found_prj, k, v)
+                        if getattr(found_prj, k) != v:
+                            setattr(found_prj, k, v)
 
-                        # standardizing project name
-                        if k == "name":
-                            if "config" in update_values:
-                                update_values["config"]["name"] = v
-                            else:
-                                found_prj.config["name"] = v
-                        found_prj.name = found_prj.config["name"]
+                            # standardizing project name
+                            if k == "name":
+                                if "config" in update_values:
+                                    update_values["config"]["name"] = v
+                                else:
+                                    found_prj.config["name"] = v
+                                found_prj.name = found_prj.config["name"]
 
                     if "samples" in update_dict:
                         if found_prj.samples_mapping:
                             for sample in found_prj.samples_mapping:
                                 _LOGGER.debug(f"deleting samples: {str(sample)}")
                                 session.delete(sample)
 
@@ -467,15 +468,15 @@
         """
         update_final = UpdateModel()
 
         if update_values.config is not None:
             if update_values.description is not None:
                 update_values.config["description"] = update_values.description
             if update_values.name is not None:
-                update_values.config["name"] = update_values.description
+                update_values.config["name"] = update_values.name
             update_final = UpdateModel(
                 config=update_values.config, **update_final.dict(exclude_unset=True)
             )
 
         if update_values.tag is not None:
             update_final = UpdateModel(
                 tag=update_values.tag, **update_final.dict(exclude_unset=True)
```

### Comparing `pepdbagent-0.5.0/pepdbagent/pepdbagent.py` & `pepdbagent-0.5.1/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent/utils.py` & `pepdbagent-0.5.1/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.5.1/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.0/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.5.1/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/setup.py` & `pepdbagent-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/tests/conftest.py` & `pepdbagent-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.0/tests/test_pepagent.py` & `pepdbagent-0.5.1/tests/test_pepagent.py`

 * *Files identical despite different names*

