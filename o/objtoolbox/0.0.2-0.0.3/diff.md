# Comparing `tmp/objtoolbox-0.0.2.tar.gz` & `tmp/objtoolbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objtoolbox-0.0.2.tar", last modified: Fri Jul  7 12:15:22 2023, max compression
+gzip compressed data, was "objtoolbox-0.0.3.tar", last modified: Tue Jul 11 18:59:23 2023, max compression
```

## Comparing `objtoolbox-0.0.2.tar` & `objtoolbox-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.2/LICENSE
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.2/README.md
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      562 2023-07-07 09:38:49.000000 objtoolbox-0.0.2/pyproject.toml
--rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/setup.cfg
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/objtoolbox/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      128 2023-07-03 08:22:06.000000 objtoolbox-0.0.2/src/objtoolbox/__init__.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1774 2023-07-06 15:29:36.000000 objtoolbox-0.0.2/src/objtoolbox/merge.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)    12284 2023-07-03 08:26:22.000000 objtoolbox-0.0.2/src/objtoolbox/storage.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2233 2023-07-07 12:14:09.000000 objtoolbox-0.0.2/src/objtoolbox/utils.py
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/objtoolbox.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/requires.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.3/LICENSE
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.3/README.md
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      562 2023-07-11 18:57:33.000000 objtoolbox-0.0.3/pyproject.toml
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/setup.cfg
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/objtoolbox/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      128 2023-07-03 08:22:06.000000 objtoolbox-0.0.3/src/objtoolbox/__init__.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1787 2023-07-10 09:52:01.000000 objtoolbox-0.0.3/src/objtoolbox/merge.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)    12320 2023-07-07 13:36:04.000000 objtoolbox-0.0.3/src/objtoolbox/storage.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2434 2023-07-11 18:58:26.000000 objtoolbox-0.0.3/src/objtoolbox/utils.py
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/objtoolbox.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/requires.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/top_level.txt
```

### Comparing `objtoolbox-0.0.2/LICENSE` & `objtoolbox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.2/PKG-INFO` & `objtoolbox-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `objtoolbox-0.0.2/pyproject.toml` & `objtoolbox-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objtoolbox"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jona Ruof", email="jona.ruof@uni-ulm.de" },
 ]
 description = "Advanced utility functions for python objects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `objtoolbox-0.0.2/src/objtoolbox/merge.py` & `objtoolbox-0.0.3/src/objtoolbox/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from objtoolbox import get_obj_dict
+from objtoolbox import get_obj_dict, ext_setattr
 
 
 def merge(dst, src):
     """
     For a given destination and source object this synchronizes both objects,
     by copying from the source into the destination object (in-place), while
     keeping the destination object structure unchanged.
```

### Comparing `objtoolbox-0.0.2/src/objtoolbox/storage.py` & `objtoolbox-0.0.3/src/objtoolbox/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,17 @@
     # write to json
 
     os.makedirs(directory, exist_ok=True)
 
     ser = Serializer(directory, compressor=compressor)
     rep = ser.serialize(obj)
 
+    if rep is Skip:
+        return
+
     unfinished_path = os.path.join(directory, "unfinished.json")
 
     with open(unfinished_path, "w+") as fd:
         json.dump(rep, fd, indent=2)
 
     state_path = os.path.join(directory, "state.json")
```

### Comparing `objtoolbox-0.0.2/src/objtoolbox/utils.py` & `objtoolbox-0.0.3/src/objtoolbox/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+class bundle(dict):
+    """
+    A dict, which allows dot notation access.
+    """
+
+    def __init__(self, *args, **kwargs):
+
+        dict.__init__(self, *args, **kwargs)
+        self.__dict__ = self
+
+
 def get_value_by_path(obj, path):
     """
     This obtains a value from a given object, where the specific value
     can be adressed by a path given as either
 
     "/obj_list/0/sub_obj/value_a" or ["obj_list", 0, "sub_obj", "value_a"].
     """
```

### Comparing `objtoolbox-0.0.2/src/objtoolbox.egg-info/PKG-INFO` & `objtoolbox-0.0.3/src/objtoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

