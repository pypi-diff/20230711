# Comparing `tmp/gxabm-2.7.3.tar.gz` & `tmp/gxabm-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.7.3.tar", last modified: Sun Jul  9 21:01:55 2023, max compression
+gzip compressed data, was "gxabm-2.7.4.tar", last modified: Tue Jul 11 14:05:24 2023, max compression
```

## Comparing `gxabm-2.7.3.tar` & `gxabm-2.7.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.936751 gxabm-2.7.3/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.3/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-09 21:01:55.936564 gxabm-2.7.3/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.3/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.927479 gxabm-2.7.3/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-07-09 21:01:19.000000 gxabm-2.7.3/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.932971 gxabm-2.7.3/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    19884 2023-07-09 21:01:19.000000 gxabm-2.7.3/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.3/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.3/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.3/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.3/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.3/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.933883 gxabm-2.7.3/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      715 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-07-09 21:01:55.936801 gxabm-2.7.3/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.3/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.936002 gxabm-2.7.3/test/
--rw-r--r--   0 suderman   (502) staff       (20)      543 2023-06-30 04:22:19.000000 gxabm-2.7.3/test/ThreadPoolTests.py
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.3/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.3/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.3/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.3/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.3/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-11 14:05:24.667330 gxabm-2.7.4/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.4/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-11 14:05:24.667158 gxabm-2.7.4/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.4/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-11 14:05:24.657042 gxabm-2.7.4/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-07-11 14:05:12.000000 gxabm-2.7.4/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.4/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.4/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-11 14:05:24.663948 gxabm-2.7.4/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.4/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19997 2023-07-11 14:04:56.000000 gxabm-2.7.4/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.4/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-26 20:05:31.000000 gxabm-2.7.4/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-07-11 14:04:56.000000 gxabm-2.7.4/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8016 2023-07-11 14:04:56.000000 gxabm-2.7.4/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7786 2023-07-11 14:04:56.000000 gxabm-2.7.4/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.4/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4357 2023-07-11 14:04:56.000000 gxabm-2.7.4/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.4/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-07-09 22:12:16.000000 gxabm-2.7.4/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.4/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-26 20:05:31.000000 gxabm-2.7.4/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.4/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.4/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-26 20:05:31.000000 gxabm-2.7.4/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.4/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.4/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-11 14:05:24.664898 gxabm-2.7.4/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      715 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-07-11 14:05:24.000000 gxabm-2.7.4/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-07-11 14:05:24.667384 gxabm-2.7.4/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.4/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-11 14:05:24.666587 gxabm-2.7.4/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      543 2023-06-30 04:22:19.000000 gxabm-2.7.4/test/ThreadPoolTests.py
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.4/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.4/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.4/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.4/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.4/test/workflow.py
```

### Comparing `gxabm-2.7.3/PKG-INFO` & `gxabm-2.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.3
+Version: 2.7.4
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.3/README.md` & `gxabm-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/__main__.py` & `gxabm-2.7.4/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/benchmark.py` & `gxabm-2.7.4/abm/lib/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,18 +199,19 @@
                         dsid = dsdata['id']
                         dssize = dsdata['size']
                         input_data_size.append(dssize)
                         print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
                         inputs[input[0]] = {'id': dsid, 'src': 'hda', 'size': dssize}
                     else:
                         raise Exception(f'Invalid input value')
-            print(f"Running workflow {wfid}")
+            print(f"Running workflow {wfid} in history {new_history_name}")
             invocation = gi.workflows.invoke_workflow(wfid, inputs=inputs, history_name=new_history_name)
             id = invocation['id']
-            invocations = gi.invocations.wait_for_invocation(id, 86400, 10, False)
+            #invocations = gi.invocations.wait_for_invocation(id, 86400, 10, False)
+            invocations = gi.invocations.wait_for_invocation(id, 86400, 10, True)
             print("Waiting for jobs")
             if history_prefix is not None:
                 parts = history_prefix.split()
                 invocations['run'] = parts[0]
                 invocations['cloud'] = parts[1]
                 if len(parts) > 2:
                     invocations['job_conf'] = parts[2]
```

### Comparing `gxabm-2.7.3/abm/lib/cloudlaunch.py` & `gxabm-2.7.4/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/common.py` & `gxabm-2.7.4/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/config.py` & `gxabm-2.7.4/abm/lib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     profile['key'] = key
     save_profiles(profiles)
     print_json(profile)
 
 
 def url(context: Context, args: list):
     if len(args) != 2:
-        print(f"USAGE: abm config key <cloud> <url>")
+        print(f"USAGE: abm config url <cloud> <url>")
         return
     profile_name = args[0]
     url = args[1]
     profiles = load_profiles()
     if not profile_name in profiles:
         print(f"ERROR: Unknown cloud {profile_name}")
         return
```

### Comparing `gxabm-2.7.3/abm/lib/dataset.py` & `gxabm-2.7.4/abm/lib/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from bioblend.galaxy import dataset_collections
-from common import connect, Context, print_json, _get_dataset_data, _make_dataset_element
+from common import connect, Context, print_json, _get_dataset_data, _make_dataset_element, find_history
 from pprint import pprint
 from pathlib import Path
 
 import os
 import yaml
 
 def list(context: Context, args: list):
@@ -143,14 +143,15 @@
     )
     print(json.dumps(result, indent=4))
 
 
 def import_from_config(context: Context, args: list):
     gi = None
     key = None
+    history = None
     kwargs = {}
     while len(args) > 0:
         arg = args.pop(0)
         if arg in ['--hs', '--hist', '--history']:
             history = args.pop(0)
         elif arg in ['-c', '--create']:
             gi = connect(context)
@@ -174,14 +175,17 @@
     if not key in datasets:
         print(f"ERROR: dataset {key} has not been defined.")
         return
     url = datasets[key]
 
     if gi is None:
         gi = connect(context)
+    if history is not None:
+        history = find_history(gi, history)
+        
     response = gi.tools.put_url(url, history, **kwargs)
     print(json.dumps(response, indent=4))
 
 
 def _import_from_url(gi, history, url, **kwargs):
     response = gi.tools.put_url(url, history, **kwargs)
     print(json.dumps(response, indent=4))
```

### Comparing `gxabm-2.7.3/abm/lib/experiment.py` & `gxabm-2.7.4/abm/lib/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     namespace = 'galaxy'
     chart = 'anvil/galaxykubeman'
     if 'galaxy' in config:
         namespace = config['galaxy']['namespace']
         chart = config['galaxy']['chart']
     if 'job_configs' in config and len(config['job_configs']) > 0:
         for conf in config['job_configs']:
+            rules_file = f"rules/{conf}.yml"
+            print(f"Applying {rules_file} namespace:{namespace} chart:{chart}")
             if not helm.update(context, [f"rules/{conf}.yml", namespace, chart]):
                 log.warning(f"job configuration not found: rules/{conf}.yml")
                 continue
             for n in range(config['runs']):
                 history_name_prefix = f"{n+1} {cloud} {conf}"
                 for workflow_conf in config['benchmark_confs']:
                     benchmark.run(context, workflow_conf, history_name_prefix, config['name'])
```

### Comparing `gxabm-2.7.3/abm/lib/folder.py` & `gxabm-2.7.4/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/helm.py` & `gxabm-2.7.4/abm/lib/helm.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,28 +33,32 @@
         return False
 
     if not os.path.exists(values):
         print(f"ERROR: Rules file not found: {values}")
         return False
 
     print(f"Applying rules {values} to {context.GALAXY_SERVER}")
+    print(f"Helm update namespace: {namespace}")
+    print(f"Helm update chart: {chart}")
     #command = f'{helm} upgrade galaxy {chart} -n {namespace} --reuse-values --set-file jobs.rules."container_mapper_rules\.yml".content={rules}'
     command = f'{helm} upgrade galaxy {chart} -n {namespace} --reuse-values -f {values}'
     env = get_env(context)
     try:
         result = run(command, env)
     except RuntimeError as e:
         print(f"Unable to helm upgrade {context.GALAXY_SERVER}")
         print(e)
         return False
 
     if result is None:
         return False
 
     print('Waiting for the new deployments to come online')
+    # Give kubernetes a moment to start processing the update.
+    time.sleep(30)
     wait_until_ready(namespace, env)
     return True
 
 
 def update_cli(context: Context, args: list):
     """
     Runs the ``helm upgrade`` command on the cluster to update the
```

### Comparing `gxabm-2.7.3/abm/lib/history.py` & `gxabm-2.7.4/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/invocation.py` & `gxabm-2.7.4/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/job.py` & `gxabm-2.7.4/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/kubectl.py` & `gxabm-2.7.4/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/library.py` & `gxabm-2.7.4/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/menu.yml` & `gxabm-2.7.4/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/users.py` & `gxabm-2.7.4/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/abm/lib/workflow.py` & `gxabm-2.7.4/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.4/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.3
+Version: 2.7.4
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.3/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.4/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/setup.py` & `gxabm-2.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/test/ThreadPoolTests.py` & `gxabm-2.7.4/test/ThreadPoolTests.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/test/check_tools.py` & `gxabm-2.7.4/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/test/metrics.py` & `gxabm-2.7.4/test/metrics.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.3/test/workflow.py` & `gxabm-2.7.4/test/workflow.py`

 * *Files identical despite different names*

