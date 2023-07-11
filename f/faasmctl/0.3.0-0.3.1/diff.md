# Comparing `tmp/faasmctl-0.3.0.tar.gz` & `tmp/faasmctl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.0.tar", last modified: Mon Jul 10 17:22:58 2023, max compression
+gzip compressed data, was "faasmctl-0.3.1.tar", last modified: Tue Jul 11 08:52:54 2023, max compression
```

## Comparing `faasmctl-0.3.0.tar` & `faasmctl-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.722644 faasmctl-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 17:20:59.000000 faasmctl-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-10 17:22:58.722644 faasmctl-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-10 17:20:59.000000 faasmctl-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.714644 faasmctl-0.3.0/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.714644 faasmctl-0.3.0/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.718644 faasmctl-0.3.0/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.722644 faasmctl-0.3.0/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-10 17:22:49.000000 faasmctl-0.3.0/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-10 17:22:49.000000 faasmctl-0.3.0/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 17:20:59.000000 faasmctl-0.3.0/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:22:58.714644 faasmctl-0.3.0/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 17:22:58.000000 faasmctl-0.3.0/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 17:20:59.000000 faasmctl-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:22:58.722644 faasmctl-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.276413 faasmctl-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 08:50:51.000000 faasmctl-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 08:52:54.276413 faasmctl-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 08:50:51.000000 faasmctl-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.264413 faasmctl-0.3.1/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.268413 faasmctl-0.3.1/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.276413 faasmctl-0.3.1/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.276413 faasmctl-0.3.1/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-11 08:52:44.000000 faasmctl-0.3.1/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-11 08:52:44.000000 faasmctl-0.3.1/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 08:50:51.000000 faasmctl-0.3.1/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:52:54.264413 faasmctl-0.3.1/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 08:52:54.000000 faasmctl-0.3.1/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-11 08:50:51.000000 faasmctl-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:52:54.276413 faasmctl-0.3.1/setup.cfg
```

### Comparing `faasmctl-0.3.0/LICENSE.md` & `faasmctl-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/PKG-INFO` & `faasmctl-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.0
+pip install faasmctl==0.3.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.0/README.md` & `faasmctl-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.0
+pip install faasmctl==0.3.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.0/faasmctl/tasks/deploy.py` & `faasmctl-0.3.1/faasmctl/tasks/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,36 @@
 from invoke import task
 from os import environ
 from os.path import join
 from subprocess import run
 
 
 @task
-def compose(ctx, workers=2, dev=False, clean=False, ini_file=None):
+def compose(ctx, workers=2, mount_source=None, clean=False, ini_file=None):
     """
     Deploy a Faasm cluster on docker compose
     """
     # First, check-out the Faasm source if necessary
-    if "FAASM_SOURCE_DIR" in environ:
+    if mount_source:
         if clean:
             print(
-                "WARNING: using the --clean flag with a FAASM_SOURCE_DIR "
+                "WARNING: using the --clean flag with --mount_source "
                 "env. variable is disabled, as local changes could be "
                 "erased!"
             )
         faasm_checkout, faasm_ver = fetch_faasm_code(
-            faasm_source=environ["FAASM_SOURCE_DIR"], force=False
+            faasm_source=mount_source, force=False
         )
     else:
-        if dev:
-            print(
-                "WARNING: using the --dev flag to start a development "
-                "cluster is only supported if you set the FAASM_SOURCE_DIR"
-                " env. variable. For more information check the deployment"
-                " documentation on ./docs/deploy.md"
-            )
-            dev = False
+        # Otherwise, we will check out the code in a faasmctl-specific working
+        # directoy
         faasm_checkout, faasm_ver = fetch_faasm_code(force=clean)
 
     env = {}
-    if dev:
+    if mount_source:
         env["FAASM_BUILD_DIR"] = join(faasm_checkout, "dev/faasm/build")
         env["FAASM_BUILD_MOUNT"] = "/build/faasm"
         env["FAASM_CODE_MOUNT"] = "/usr/local/code/faasm"
         env["FAASM_CONAN_MOUNT"] = "/root/.conan"
         env["FAASM_LOCAL_MOUNT"] = "/usr/local/faasm"
         env["PLANNER_BUILD_MOUNT"] = env["FAASM_BUILD_MOUNT"]
```

### Comparing `faasmctl-0.3.0/faasmctl/tasks/flush.py` & `faasmctl-0.3.1/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/tasks/invoke.py` & `faasmctl-0.3.1/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/config.py` & `faasmctl-0.3.1/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/deploy.py` & `faasmctl-0.3.1/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/flush.py` & `faasmctl-0.3.1/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.1/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.1/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/invoke.py` & `faasmctl-0.3.1/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl/util/planner.py` & `faasmctl-0.3.1/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.1/faasmctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.0
+pip install faasmctl==0.3.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.0/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.1/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.0/pyproject.toml` & `faasmctl-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

