# Comparing `tmp/abml-0.1.6.tar.gz` & `tmp/abml-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abml-0.1.6.tar", max compression
+gzip compressed data, was "abml-0.1.7.tar", max compression
```

## Comparing `abml-0.1.6.tar` & `abml-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0      586 2023-04-08 14:31:24.000000 abml-0.1.6/abml/__init__.py
--rw-r--r--   0        0        0    12263 2023-04-03 09:51:54.000000 abml-0.1.6/abml/abml_assembly.py
--rw-r--r--   0        0        0     3969 2023-03-22 07:48:31.449857 abml-0.1.6/abml/abml_bcs.py
--rw-r--r--   0        0        0        0 2023-03-27 09:39:35.000000 abml-0.1.6/abml/abml_config.py
--rw-r--r--   0        0        0     1280 2023-03-15 10:30:19.422097 abml-0.1.6/abml/abml_constraints.py
--rw-r--r--   0        0        0    18780 2023-04-11 06:35:31.492437 abml-0.1.6/abml/abml_dataclass.py
--rw-r--r--   0        0        0     8020 2023-04-11 07:17:39.600876 abml-0.1.6/abml/abml_helpers.py
--rw-r--r--   0        0        0     4223 2023-04-03 10:04:11.000000 abml-0.1.6/abml/abml_interaction_prop.py
--rw-r--r--   0        0        0     2678 2023-04-07 15:07:46.000000 abml-0.1.6/abml/abml_interactions.py
--rw-r--r--   0        0        0     5198 2023-03-28 12:54:48.239612 abml-0.1.6/abml/abml_jnl_loader.py
--rw-r--r--   0        0        0     2691 2023-04-07 15:17:38.000000 abml-0.1.6/abml/abml_jobs.py
--rw-r--r--   0        0        0     2028 2023-04-05 08:25:23.318715 abml-0.1.6/abml/abml_loads.py
--rw-r--r--   0        0        0     1727 2023-04-08 14:04:31.000000 abml-0.1.6/abml/abml_loggers.py
--rw-r--r--   0        0        0     4833 2023-03-30 12:29:52.000000 abml-0.1.6/abml/abml_materials.py
--rw-r--r--   0        0        0     6246 2023-03-30 14:44:49.000000 abml-0.1.6/abml/abml_mesh.py
--rw-r--r--   0        0        0    23347 2023-04-09 19:25:35.000000 abml-0.1.6/abml/abml_parts.py
--rw-r--r--   0        0        0      823 2023-03-14 07:49:32.486729 abml-0.1.6/abml/abml_sections.py
--rw-r--r--   0        0        0     6676 2023-04-11 07:11:20.706006 abml-0.1.6/abml/abml_sketch.py
--rw-r--r--   0        0        0      552 2023-03-21 10:29:46.264400 abml-0.1.6/abml/abml_steps.py
--rw-r--r--   0        0        0       22 2023-04-05 06:54:54.905037 abml-0.1.6/abml/logging.yaml
--rw-r--r--   0        0        0      397 2023-04-11 07:34:16.484479 abml-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 14:05:32.882361 abml-0.1.6/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 abml-0.1.6/setup.py
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 abml-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 13:03:48.000000 abml-0.1.7/abml/__init__.py
+-rw-r--r--   0        0        0     1953 2023-07-04 14:42:49.000000 abml-0.1.7/abml/abml_analysis.py
+-rw-r--r--   0        0        0     9980 2023-07-11 11:53:53.681699 abml-0.1.7/abml/abml_assembly.py
+-rw-r--r--   0        0        0     2619 2023-06-27 11:40:18.000000 abml-0.1.7/abml/abml_bc.py
+-rw-r--r--   0        0        0     1137 2023-07-11 12:55:32.472073 abml-0.1.7/abml/abml_cae.py
+-rw-r--r--   0        0        0     1317 2023-07-01 12:21:56.430989 abml-0.1.7/abml/abml_constraint.py
+-rw-r--r--   0        0        0     9338 2023-07-03 07:45:16.434253 abml-0.1.7/abml/abml_helpers.py
+-rw-r--r--   0        0        0     8617 2023-07-04 08:37:25.000000 abml-0.1.7/abml/abml_interaction.py
+-rw-r--r--   0        0        0     2154 2023-07-03 10:40:57.714394 abml-0.1.7/abml/abml_interaction_property.py
+-rw-r--r--   0        0        0     3482 2023-07-03 09:10:06.187673 abml-0.1.7/abml/abml_loads.py
+-rw-r--r--   0        0        0     3315 2023-07-05 08:54:45.000000 abml-0.1.7/abml/abml_logger.py
+-rw-r--r--   0        0        0     5941 2023-07-01 13:40:02.852130 abml-0.1.7/abml/abml_materials.py
+-rw-r--r--   0        0        0     4172 2023-06-28 06:51:34.000000 abml-0.1.7/abml/abml_models.py
+-rw-r--r--   0        0        0    16851 2023-07-11 11:52:40.768141 abml-0.1.7/abml/abml_parts.py
+-rw-r--r--   0        0        0     2295 2023-06-27 10:39:10.000000 abml-0.1.7/abml/abml_region.py
+-rw-r--r--   0        0        0     1591 2023-06-22 11:08:10.552904 abml-0.1.7/abml/abml_sections.py
+-rw-r--r--   0        0        0     8637 2023-07-11 11:19:36.312947 abml-0.1.7/abml/abml_session.py
+-rw-r--r--   0        0        0     8597 2023-07-03 13:10:36.123213 abml-0.1.7/abml/abml_sketches.py
+-rw-r--r--   0        0        0     2831 2023-06-22 12:09:46.610466 abml-0.1.7/abml/abml_steps.py
+-rw-r--r--   0        0        0      332 2023-07-11 19:28:05.960694 abml-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 13:19:01.000000 abml-0.1.7/README.md
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 abml-0.1.7/PKG-INFO
```

### Comparing `abml-0.1.6/abml/abml_jobs.py` & `abml-0.1.7/abml/abml_analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,67 @@
-from abml_dataclass import Abml_Registry
-
-# from abml_helpers import cprint
 from abaqus import mdb
-from abaqusConstants import ANALYSIS, DEFAULT, OFF
-import os
-from shutil import copy, move
-from io import open
-from abml_helpers import cprint
+from abml.abml_helpers import convert_abaqus_constants, cprint
+import logging
+from os import rename, listdir, getcwd, path
+
+class Abml_Analysis():
+    def __init__(self, **data):
+        self.data = data
+        self.jobs = self.data.get("jobs", {})
+    
+        self.create_jobs()
+    
+    def create_jobs(self):
+        for job in self.jobs:
+            Abml_Job(name=job, **self.jobs[job])
+
 
 
-@Abml_Registry.register("jobs")
-class Abml_Job:
-    def __init__(self, name, model, **kwargs):  # noqa
-        self.name = str(name)
-        self.model = model
-        self.kwargs = kwargs
+class Abml_Job():
+    def __init__(self, name, **kwargs):
+        self.name = name
+        self.kwargs = convert_abaqus_constants(**kwargs)
+        self.commands = self.kwargs.pop("commands", [])
+
         self.create()
 
-    def create(self):
-        subroutine_flag = self.kwargs.get("subroutine", False)
-        if subroutine_flag:
-            subroutine_path = os.path.abspath("{}.for".format(self.name))
-        else:
-            subroutine_path = None
-
-        kwargs = {
-            "name": self.name,
-            "model": self.model.name,
-            "description": self.kwargs.get("description", ""),
-            "type": ANALYSIS,
-            "userSubroutine": subroutine_path,
-            "numCpus": self.kwargs.get("cpus", 1),
-            "numGPUs": self.kwargs.get("gpus", 0),
-            "multiprocessingMode": DEFAULT,
+        self.access = mdb.jobs[self.name]
+        self.command_map = { 
+            "writeInput": self.write_input,
+            "submit": self.access.submit,
+            "waitForCompletion": self.access.waitForCompletion,
+            "kill": self.access.kill, 
+            "clearMessages": self.access.clearMessages,
+            "setValues": self.access.setValues,
         }
 
-        mdb.Job(**kwargs)
+        self.command_map = {k.lower():v for k,v in self.command_map.items()}
+
+        self.call_commands()
+
+    def create(self):
+        mdb.Job(name=self.name, **self.kwargs)
+
+    def call_commands(self):
+        for command in self.commands:
+            type_ = next(iter(command))
+            self.command_map[type_.lower()](**command[type_])
+
+
+    def write_input(self, **kwargs):
+        name = None
+        if "name" in kwargs:
+            name = kwargs.pop("name")
+
+        mdb.jobs[self.name].writeInput(**kwargs)
+
+        if name is not None:
+            src = path.join(getcwd(), "{}.inp".format(self.name))
+            dest = path.join(getcwd(), name)
+            
+            rename(src, dest)
+    
+    def submit(self):
+        mdb.jobs[self.name].submit(**self.submit_kwargs)
 
-        if self.kwargs.get("write_input", False):
-            self.write_input()
-            self.add_to_header(subroutine=self.sub_name, priority=self.kwargs.get("priority", "default"))
-
-    def write_input(self):
-        mdb.jobs[self.name].writeInput(consistencyChecking=OFF)
-
-    def load_subname(self):
-        if "subroutine_queue" in self.kwargs:
-            self.sub_name = self.kwargs["subroutine_queue"]
-        else:
-            self.sub_name = "{}.for".format(self.name)
-
-    def write_and_copy_input_to_path(self, path):
-        self.write_input()
-        self.add_to_header(subroutine="{}.for".format(self.name), priority=self.kwargs.get("priority", "default"))
-        filename = "{}.inp".format(self.name)
-        copy(filename, os.path.join(path, filename))
-
-    def write_and_move_input_to_path(self, path):
-        self.write_input()
-        self.add_to_header(subroutine="{}.inp".format(self.name), priority=self.kwargs.get("priority", "default"))
-        filename = "{}.inp".format(self.name)
-        move(filename, os.path.join(path, filename))
-
-    def add_to_header(self, **kwargs):
-        filename = "{}.inp".format(self.name)
-        with open(filename, "r", encoding="utf-8") as f:
-            input_file = f.readlines()
-
-        for key, value in kwargs.items():
-            input_file.insert(1, "** {key}={value}\n".format(key=key, value=value))
-
-        with open(filename, "w", encoding="utf-8") as f:
-            input_file = "".join(input_file)
-            f.write(input_file)
+    def waitForCompletion(self):
+        mdb.jobs[self.name].waitForCompletion()
```

