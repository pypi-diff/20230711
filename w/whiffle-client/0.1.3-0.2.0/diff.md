# Comparing `tmp/whiffle_client-0.1.3.tar.gz` & `tmp/whiffle_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/app/dist/.tmp-xiwz3ys9/whiffle_client-0.1.3.tar", last modified: Wed Jun 21 06:54:00 2023, max compression
+gzip compressed data, was "/builds/whiffle/hindcasting/whiffle-client/dist/.tmp-55yuhyal/whiffle_client-0.2.0.tar", last modified: Tue Jul 11 09:52:22 2023, max compression
```

## Comparing `whiffle_client-0.1.3.tar` & `whiffle_client-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-20 10:03:07.000000 whiffle_client-0.1.3/LICENCE.txt
--rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1333 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      780 2023-06-20 10:06:11.000000 whiffle_client-0.1.3/README.md
--rw-rw-r--   0 root         (0) root         (0)      994 2023-06-21 06:51:29.000000 whiffle_client-0.1.3/USER_README.md
--rw-rw-r--   0 root         (0) root         (0)      681 2023-06-21 06:53:36.000000 whiffle_client-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/tests/
--rw-rw-r--   0 root         (0) root         (0)     3502 2023-06-20 16:15:11.000000 whiffle_client-0.1.3/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client/
--rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/client.py
--rw-rw-r--   0 root         (0) root         (0)     2515 2023-06-20 16:14:16.000000 whiffle_client-0.1.3/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client/resources/
--rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/resources/example_generic_params.json
--rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1333 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7093 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.1.3/LICENCE.txt` & `whiffle_client-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.3/PKG-INFO` & `whiffle_client-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.1.3/README.md` & `whiffle_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.3/USER_README.md` & `whiffle_client-0.2.0/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.3/pyproject.toml` & `whiffle_client-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "whiffle_client"
-version = "0.1.3"
 description = "Python based web client to interact with Whiffle services"
 readme = "USER_README.md"
 
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -13,16 +12,24 @@
 ]
 
 dependencies = [
     "click~=8.0.4",
     "PyYAML~=6.0",
     "requests~=2.27.1",
 ]
-# dynamic = ["version"]
+dynamic = ["version"]
+
 [tool.setuptools]
 packages = ["whiffle_client"]
 
 [project.scripts]
 whiffle = "whiffle_client.entrypoints:whiffle"
 
 [tool.setuptools.package-data]
 whiffle_client = ["resources/whiffle_config.yaml", "resources/example_generic_params.json"]
+
+[build-system]
+requires = ["setuptools>=42", "wheel", "setuptools-git-versioning"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools-git-versioning]
+enabled = true
```

### Comparing `whiffle_client-0.1.3/tests/test_client.py` & `whiffle_client-0.2.0/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,15 @@
         return self.data
 
 
 def mock_new_task_response(mocker, warnings={}):
     mocker.patch(
         "whiffle_client.Client._create_request",
         return_value=MockResponse(
-            {
-                "task_id": "hash1234",
-                "task_status": "created",
-                "warnings": warnings,
-            },
+            {"task_id": "hash1234", "task_status": "created", "warnings": warnings}
         ),
     )
 
 
 class TestAPI:
     def test_init_client_with_default_params(self):
         with open(CONFIG_FILE_PATH) as file_object:
@@ -97,20 +93,29 @@
         res = runner.invoke(whiffle, ["config-edit", "user.token", token])
         assert token in res.output
         res = runner.invoke(whiffle, ["config-list"])
         assert token in res.output
 
     def test_run_task(self, mocker):
         mock_new_task_response(mocker)
-        mock = mocker.patch(
-            "whiffle_client.Client.communicate",
-        )
+        mock = mocker.patch("whiffle_client.Client.process")
         runner.invoke(whiffle, ["run", default_task_path])
         mock.assert_called_once()
 
-    def test_run_task(self, mocker):
+    def test_tasks_list(self, mocker):
         mock_new_task_response(mocker)
-        mock = mocker.patch(
-            "whiffle_client.Client.get_tasks",
-        )
+        mock = mocker.patch("whiffle_client.Client.get_tasks")
         runner.invoke(whiffle, ["tasks-list"])
-        mock.assert_called_once()
+        mock.assert_called_once()
+
+    def test_download_task(self, mocker):
+        mock_new_task_response(mocker)
+        mock = mocker.patch("whiffle_client.Client.download")
+        res = runner.invoke(whiffle, ["tasks-download", "123"])
+        assert not "Error" in res.output, res.output
+        mock.assert_called_once()
+
+    def test_attatch_task(self, mocker):
+        mock_new_task_response(mocker)
+        mock = mocker.patch("whiffle_client.Client.communicate")
+        runner.invoke(whiffle, ["tasks-attach", "123"])
+        mock.assert_called_once()
```

### Comparing `whiffle_client-0.1.3/whiffle_client/client.py` & `whiffle_client-0.2.0/whiffle_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,15 @@
 class NoTokenError(Exception):
     pass
 
 
 class Client:
     """TODO: Client to launch task"""
 
-    def __init__(
-        self,
-        access_token=None,
-        url=None,
-        session=None,
-    ):
+    def __init__(self, access_token=None, url=None, session=None):
         """
         Authentication order:
         1. `access_token` passed when creating class.
         2. token in CONFIG_FILE_PATH (JSON format)
         """
 
         with open(CONFIG_FILE_PATH) as file_object:
@@ -171,16 +166,15 @@
                     flush=True,
                 )
         file.close()
         print()
 
     def get_progress(self, task_id):
         res = self._create_request(
-            self.session.get,
-            "/api/aspforge/tasks/{}/progress".format(task_id),
+            self.session.get, "/api/aspforge/tasks/{}/progress".format(task_id)
         )
         return res.json()
 
     # Follow the progress of a task. By default, take the latest task_id.
     def communicate(self, task_id=None, filename=None):
         if task_id == None:
             task_id = self.get_tasks()[-1]["task_id"]
```

### Comparing `whiffle_client-0.1.3/whiffle_client/entrypoints.py` & `whiffle_client-0.2.0/whiffle_client/entrypoints.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 def whiffle():
     pass
 
 
 @whiffle.command()
 @click.argument("number_of_tasks", default=10)
 def tasks_list(number_of_tasks):
+    """List tasks"""
+
     number_of_tasks = int(number_of_tasks)
     client = Client()
     tasks = client.get_tasks()
     click.echo(
         "{:33}{:11}{:16} {:16} progress".format(
             "task id", "status", "start time", "finish time"
         )
@@ -26,18 +28,19 @@
             task["finished"] = ""
         click.echo(
             "{task_id:33}{task_status:11}{received:17.16}{finished:17.16}{processed_steps}/{total_steps}".format(
                 **task
             )
         )
 
+
 @whiffle.command()
 @click.argument("file_path")
 def run(file_path) -> str:
-    """Run task type given a set of parameters.
+    """Run task with given a set of parameters
 
     \b
     Parameters
     ----------
     file_path : str
         Path to (json|yaml) file containing parameters
 
@@ -52,15 +55,15 @@
     return client.process(file_path)
 
 
 @whiffle.command()
 @click.argument("key")
 @click.argument("value")
 def config_edit(key, value) -> str:
-    """Edit Whiffle configuration file
+    """Edit configuration file
 
     \b
     Parameters
     ----------
     key : str
         Dot separated key value (e.g.: user.token)
     value : str
@@ -95,7 +98,37 @@
 
     with open(CONFIG_FILE_PATH) as file_object:
         config = yaml.safe_load(file_object)
 
     click.echo("Current configuration:\n-----\n")
     click.echo(yaml.safe_dump(config))
     click.echo("-----")
+
+
+@whiffle.command()
+@click.argument("task_id")
+def tasks_download(task_id):
+    """Download task
+
+    \b
+    Parameters
+    ----------
+    task_id : str
+    """
+    click.echo(f"downloading task output {task_id}")
+    client = Client()
+    client.download(task_id)
+
+
+@whiffle.command()
+@click.argument("task_id")
+def tasks_attach(task_id):
+    """Attach to task
+
+    \b
+    Parameters
+    ----------
+    task_id : str
+    """
+    click.echo(f"attaching to task {task_id}")
+    client = Client()
+    client.communicate(task_id)
```

### Comparing `whiffle_client-0.1.3/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.2.0/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.3/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.2.0/whiffle_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle-client
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

