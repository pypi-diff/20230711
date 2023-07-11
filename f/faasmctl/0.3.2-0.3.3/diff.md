# Comparing `tmp/faasmctl-0.3.2.tar.gz` & `tmp/faasmctl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.2.tar", last modified: Tue Jul 11 09:12:08 2023, max compression
+gzip compressed data, was "faasmctl-0.3.3.tar", last modified: Tue Jul 11 19:07:07 2023, max compression
```

## Comparing `faasmctl-0.3.2.tar` & `faasmctl-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.517828 faasmctl-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 09:09:56.000000 faasmctl-0.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 09:12:08.517828 faasmctl-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 09:09:56.000000 faasmctl-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.509828 faasmctl-0.3.2/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.513828 faasmctl-0.3.2/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.517828 faasmctl-0.3.2/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.517828 faasmctl-0.3.2/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-11 09:11:57.000000 faasmctl-0.3.2/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-11 09:11:57.000000 faasmctl-0.3.2/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 09:09:56.000000 faasmctl-0.3.2/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:08.509828 faasmctl-0.3.2/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 09:12:08.000000 faasmctl-0.3.2/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-11 09:09:56.000000 faasmctl-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:12:08.517828 faasmctl-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 19:03:24.000000 faasmctl-0.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 19:07:07.218190 faasmctl-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 19:03:24.000000 faasmctl-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.214190 faasmctl-0.3.3/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-11 19:06:58.000000 faasmctl-0.3.3/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-11 19:06:58.000000 faasmctl-0.3.3/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.214190 faasmctl-0.3.3/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-11 19:03:24.000000 faasmctl-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:07:07.218190 faasmctl-0.3.3/setup.cfg
```

### Comparing `faasmctl-0.3.2/LICENSE.md` & `faasmctl-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/PKG-INFO` & `faasmctl-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.2
+Version: 0.3.3
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
-pip install faasmctl==0.3.2
+pip install faasmctl==0.3.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.2/README.md` & `faasmctl-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.2
+pip install faasmctl==0.3.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.2/faasmctl/tasks/deploy.py` & `faasmctl-0.3.3/faasmctl/util/compose.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,71 @@
-from faasmctl.util.compose import delete_compose_cluster
-from faasmctl.util.config import get_faasm_ini_file, get_faasm_ini_value
-from faasmctl.util.deploy import fetch_faasm_code, generate_ini_file
+from faasmctl.util.config import get_faasm_ini_value
+from faasmctl.util.deploy import generate_ini_file
 from faasmctl.util.random import generate_gid
-from invoke import task
 from os import environ
 from os.path import join
 from subprocess import run
 
 
-@task
-def compose(ctx, workers=2, mount_source=None, clean=False, ini_file=None):
-    """
-    Deploy a Faasm cluster on docker compose
-    """
-    # First, check-out the Faasm source if necessary
-    if mount_source:
-        if clean:
-            print(
-                "WARNING: using the --clean flag with --mount_source "
-                "env. variable is disabled, as local changes could be "
-                "erased!"
-            )
-        faasm_checkout, faasm_ver = fetch_faasm_code(
-            faasm_source=mount_source, force=False
-        )
-    else:
-        # Otherwise, we will check out the code in a faasmctl-specific working
-        # directoy
-        faasm_checkout, faasm_ver = fetch_faasm_code(force=clean)
-
+def get_compose_env_vars(faasm_checkout, mount_source):
     env = {}
     if mount_source:
         env["FAASM_BUILD_DIR"] = join(faasm_checkout, "dev/faasm/build")
         env["FAASM_BUILD_MOUNT"] = "/build/faasm"
         env["FAASM_CODE_MOUNT"] = "/usr/local/code/faasm"
         env["FAASM_CONAN_MOUNT"] = "/root/.conan"
         env["FAASM_LOCAL_MOUNT"] = "/usr/local/faasm"
         env["PLANNER_BUILD_MOUNT"] = env["FAASM_BUILD_MOUNT"]
+    else:
+        # FIXME: by using `./dev` in non-mounted clusters we make it impossible
+        # to cleanly remove them (as ./dev is root-owned), so we can't rm -rf
+        # the directory
+        env["FAASM_BUILD_DIR"] = join(faasm_checkout, "dev/faasm/build")
+        env["FAASM_BUILD_MOUNT"] = "/host_dev/build"
+        env["FAASM_CODE_MOUNT"] = "/host_dev/code"
+        env["FAASM_CONAN_MOUNT"] = "/host_dev/conan"
+        env["FAASM_LOCAL_MOUNT"] = "/host_dev/faasm-local"
+        env["PLANNER_BUILD_MOUNT"] = "/build/faabric/static"
+
+    # Get Faasm version
+    with open(join(faasm_checkout, "VERSION"), "r") as fh:
+        faasm_ver = fh.read()
+        faasm_ver = faasm_ver.strip()
 
     # Whitelist env. variables that we recognise
     if "WASM_VM" in environ:
         wasm_vm = environ["WASM_VM"]
         if wasm_vm == "sgx-sim":
             worker_img = "faasm/worker-sgx-sim:{}".format(faasm_ver)
             env["WASM_VM"] = "sgx"
             env["FAASM_CLI_IMAGE"] = "faasm/cli-sgx-sim:{}".format(faasm_ver)
             env["FAASM_WORKER_IMAGE"] = worker_img
         elif wasm_vm == "sgx":
             env["WASM_VM"] = "sgx"
             env["FAASM_CLI_IMAGE"] = "faasm/cli-sgx:{}".format(faasm_ver)
             env["FAASM_WORKER_IMAGE"] = "faasm/worker-sgx:{}".format(faasm_ver)
 
+    if "FAASM_CLI_IMAGE" in environ:
+        env["FAASM_CLI_IMAGE"] = environ["FAASM_CLI_IMAGE"]
+
+    return env
+
+
+def deploy_compose_cluster(faasm_checkout, workers, mount_source, ini_file):
+    """
+    Deploy a docker compose cluster
+
+    Parameters:
+    - faasm_checkout (str): path to the Faasm's source code checkout
+    - workers (int): number of workers to deploy
+    - mount_source (bool): flag to indicate whether we mount code/binaries
+    - ini_file (str): path to the ini_file to generate (if selected)
+    """
+    env = get_compose_env_vars(faasm_checkout, mount_source)
+
     # Generate random compose project name
     env["COMPOSE_PROJECT_NAME"] = "faasm-{}".format(generate_gid())
 
     # Deploy the compose cluster
     cmd = [
         "docker compose up -d",
         "--scale worker={}".format(workers),
@@ -65,23 +76,48 @@
 
     # Finally, generate the faasm.ini file to interact with the cluster
     generate_ini_file(
         "compose",
         out_file=ini_file,
         name=env["COMPOSE_PROJECT_NAME"],
         cwd=faasm_checkout,
+        mount_source=mount_source,
     )
 
 
-@task
-def delete(ctx, ini_file=None):
+def delete_compose_cluster(ini_file):
     """
-    Delete a running Faasm cluster by passing the path to the --ini-file
+    Delete a cluster running on docker compose
+
+    Parameters:
+    - ini_file (str): path to the ini_file generated by the deploy command
     """
-    if not ini_file:
-        ini_file = get_faasm_ini_file()
+    working_dir = get_faasm_ini_value(ini_file, "Faasm", "working_dir")
+    cluster_name = get_faasm_ini_value(ini_file, "Faasm", "cluster_name")
+    compose_cmd = [
+        "docker compose",
+        "-p {}".format(cluster_name),
+        "down",
+    ]
+    compose_cmd = " ".join(compose_cmd)
+    run(compose_cmd, shell=True, check=True, cwd=working_dir)
 
-    backend = get_faasm_ini_value(ini_file, "Faasm", "backend")
-    if backend == "compose":
-        delete_compose_cluster(ini_file)
-    else:
-        raise RuntimeError("Unsupported backend: {}".format(backend))
+
+def run_compose_cmd(ini_file, cmd):
+    cluster_name = get_faasm_ini_value(ini_file, "Faasm", "cluster_name")
+    work_dir = get_faasm_ini_value(ini_file, "Faasm", "working_dir")
+    mount_source = get_faasm_ini_value(ini_file, "Faasm", "mount_source")
+    mount_source = mount_source == "True"
+
+    compose_cmd = [
+        "docker compose",
+        "-p {}".format(cluster_name),
+        cmd,
+    ]
+    compose_cmd = " ".join(compose_cmd)
+    run(
+        compose_cmd,
+        shell=True,
+        check=True,
+        cwd=work_dir,
+        env=get_compose_env_vars(work_dir, mount_source),
+    )
```

### Comparing `faasmctl-0.3.2/faasmctl/tasks/flush.py` & `faasmctl-0.3.3/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/tasks/invoke.py` & `faasmctl-0.3.3/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/config.py` & `faasmctl-0.3.3/faasmctl/util/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from configparser import ConfigParser
 from os import environ
 from os.path import exists
 
+BACKEND_INI_STRING = "backend"
+
 
 def get_faasm_ini_file():
     """
     Try to read faasm's ini file from the environment, fail otherwise
     """
     if "FAASM_INI_FILE" not in environ:
         raise RuntimeError("No FAASM_INI_FILE env. variable detected!")
```

### Comparing `faasmctl-0.3.2/faasmctl/util/deploy.py` & `faasmctl-0.3.3/faasmctl/util/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,19 @@
                 "ERROR: we were not able to clean the checkout dir. This is"
                 " probably due to an issue in Faasm where some directories "
                 "in a compose cluster are root-owned (in the container). "
                 "Try running the following:\n{}".format(tmp_fix)
             )
             raise RuntimeError("Error. Try running:\n{}".format(tmp_fix))
 
+    # FIXME: allow a purely detached faasm checkout. Right now, cpp's code
+    # source is _always_ mounted from clients/cpp
+    git_cmd = "git submodule update --init"
+    run(git_cmd, shell=True, check=True, cwd=checkout_path)
+
     faasm_ver = _check_version_mismatch(checkout_path)
 
     return checkout_path, faasm_ver
 
 
 def generate_ini_file(backend, out_file, **kwargs):
     if backend == "compose":
@@ -97,14 +102,15 @@
 
         # This comment line can't be outside of the Faasm section
         fh.write("# Auto-generated at {}\n".format(datetime.now()))
 
         fh.write("backend = {}\n".format(backend))
         if backend == "compose":
             fh.write("working_dir = {}\n".format(working_dir))
+            fh.write("mount_source = {}\n".format(kwargs["mount_source"]))
         if backend == "compose":
             fh.write("cluster_name = {}\n".format(cluster_name))
         fh.write("upload_host = {}\n".format(upload_ip))
         if backend == "compose":
             fh.write("upload_host_in_docker = upload\n")
         fh.write("upload_port = {}\n".format(upload_port))
         fh.write("planner_host = {}\n".format(planner_ip))
```

### Comparing `faasmctl-0.3.2/faasmctl/util/docker.py` & `faasmctl-0.3.3/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/flush.py` & `faasmctl-0.3.3/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.3/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.3/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/invoke.py` & `faasmctl-0.3.3/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/planner.py` & `faasmctl-0.3.3/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl/util/upload.py` & `faasmctl-0.3.3/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.2/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.3/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.2
+Version: 0.3.3
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
-pip install faasmctl==0.3.2
+pip install faasmctl==0.3.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.2/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.3/faasmctl.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 faasmctl.egg-info/PKG-INFO
 faasmctl.egg-info/SOURCES.txt
 faasmctl.egg-info/dependency_links.txt
 faasmctl.egg-info/entry_points.txt
 faasmctl.egg-info/requires.txt
 faasmctl.egg-info/top_level.txt
 faasmctl/tasks/__init__.py
+faasmctl/tasks/cli.py
+faasmctl/tasks/delete.py
 faasmctl/tasks/deploy.py
 faasmctl/tasks/flush.py
 faasmctl/tasks/invoke.py
+faasmctl/tasks/logs.py
+faasmctl/tasks/status.py
 faasmctl/tasks/upload.py
+faasmctl/util/backend.py
 faasmctl/util/batch.py
 faasmctl/util/compose.py
 faasmctl/util/config.py
 faasmctl/util/deploy.py
 faasmctl/util/docker.py
 faasmctl/util/env.py
 faasmctl/util/faasm.py
```

### Comparing `faasmctl-0.3.2/pyproject.toml` & `faasmctl-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

