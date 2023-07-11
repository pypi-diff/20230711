# Comparing `tmp/builderer-1.1.0.tar.gz` & `tmp/builderer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "builderer-1.1.0.tar", last modified: Tue Feb 28 14:47:27 2023, max compression
+gzip compressed data, was "builderer-2.0.0.tar", last modified: Tue Jul 11 21:51:46 2023, max compression
```

## Comparing `builderer-1.1.0.tar` & `builderer-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:47:27.217472 builderer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-28 14:47:16.000000 builderer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-28 14:47:27.217472 builderer-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-02-28 14:47:16.000000 builderer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:47:27.213472 builderer-1.1.0/builderer/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-28 14:47:16.000000 builderer-1.1.0/builderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-28 14:47:16.000000 builderer-1.1.0/builderer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-28 14:47:16.000000 builderer-1.1.0/builderer/_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-02-28 14:47:16.000000 builderer-1.1.0/builderer/builderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-02-28 14:47:16.000000 builderer-1.1.0/builderer/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:47:27.217472 builderer-1.1.0/builderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 14:47:27.000000 builderer-1.1.0/builderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-28 14:47:16.000000 builderer-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-02-28 14:47:27.217472 builderer-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:47:27.217472 builderer-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-02-28 14:47:16.000000 builderer-1.1.0/tests/test___main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-02-28 14:47:16.000000 builderer-1.1.0/tests/test_builderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-28 14:47:16.000000 builderer-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-28 14:47:16.000000 builderer-1.1.0/tests/test_file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:51:46.618897 builderer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 21:51:36.000000 builderer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-11 21:51:46.618897 builderer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-11 21:51:36.000000 builderer-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:51:46.618897 builderer-2.0.0/builderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/builderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-11 21:51:36.000000 builderer-2.0.0/builderer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:51:46.618897 builderer-2.0.0/builderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 21:51:46.000000 builderer-2.0.0/builderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 21:51:36.000000 builderer-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-11 21:51:46.618897 builderer-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:51:46.618897 builderer-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test___main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test_builderer_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test_builderer_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-11 21:51:36.000000 builderer-2.0.0/tests/test_file_config.py
```

### Comparing `builderer-1.1.0/LICENSE` & `builderer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `builderer-1.1.0/PKG-INFO` & `builderer-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: builderer
-Version: 1.1.0
+Version: 2.0.0
 Summary: Container based mono repo builder.
 Home-page: https://github.com/florian-sattler/builderer/
 Author: Florian Sattler
 Author-email: dev@florian-sattler.de
 License: MIT
 Project-URL: Documentation, https://builderer.florian-sattler.de/
 Project-URL: Source, https://github.com/florian-sattler/builderer/
 Project-URL: Changelog, https://github.com/florian-sattler/builderer/blob/main/CHANGELOG.md
 Project-URL: Tracker, https://github.com/florian-sattler/builderer/issues
 Project-URL: Download, https://pypi.org/project/builderer/#files
 Keywords: builderer,continuous integration,continuous delivery
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -30,15 +31,15 @@
     </a>
     <h1>
         builderer
     </h1>
     <p>
         <em>Container based mono repo builder</em>
     </p>
-    <p> 
+    <p>
         <a href="https://pypi.python.org/pypi/builderer">
             <img src="https://img.shields.io/pypi/v/builderer.svg">
         </a>
         <a href="https://pepy.tech/project/builderer">
             <img src="https://pepy.tech/badge/builderer">
         </a>
         <a href="https://github.com/florian-sattler/builderer">
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: builderer Version: 1.1.0 Summary: Container based
+Metadata-Version: 2.1 Name: builderer Version: 2.0.0 Summary: Container based
 mono repo builder. Home-page: https://github.com/florian-sattler/builderer/
 Author: Florian Sattler Author-email: dev@florian-sattler.de License: MIT
 Project-URL: Documentation, https://builderer.florian-sattler.de/ Project-URL:
 Source, https://github.com/florian-sattler/builderer/ Project-URL: Changelog,
 https://github.com/florian-sattler/builderer/blob/main/CHANGELOG.md Project-
 URL: Tracker, https://github.com/florian-sattler/builderer/issues Project-URL:
 Download, https://pypi.org/project/builderer/#files Keywords:
-builderer,continuous integration,continuous delivery Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
+builderer,continuous integration,continuous delivery Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE
              [https://builderer.florian-sattler.de/logo-color.svg]
                             ****** builderer ******
                        Container based mono repo builder
     [https://img.shields.io/pypi/v/builderer.svg] [https://pepy.tech/badge/
    builderer] [https://img.shields.io/pypi/pyversions/builderer.svg] [PyPI_-
       License] [https://img.shields.io/github/v/release/florian-sattler/
  builderer?label=github] [https://img.shields.io/badge/docs-yes-brightgreen]
```

### Comparing `builderer-1.1.0/README.md` & `builderer-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     </a>
     <h1>
         builderer
     </h1>
     <p>
         <em>Container based mono repo builder</em>
     </p>
-    <p> 
+    <p>
         <a href="https://pypi.python.org/pypi/builderer">
             <img src="https://img.shields.io/pypi/v/builderer.svg">
         </a>
         <a href="https://pepy.tech/project/builderer">
             <img src="https://pepy.tech/badge/builderer">
         </a>
         <a href="https://github.com/florian-sattler/builderer">
```

### Comparing `builderer-1.1.0/builderer/_documentation.py` & `builderer-2.0.0/builderer/_documentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 arg_verbose_desc = "Show issued commands and their live output."
 arg_tags_title = "Tags to use"
 arg_tags_desc = "One or multiple tags to use for each image. Defaults to ['latest']"
 arg_simulate_title = "Simulate execution"
 arg_simulate_desc = "Prevent issuing any commands just do the printing."
 arg_backend_title = "Build Backend"
 arg_backend_desc = "Overwrite the backend used to build, tag and pull images. Defaults to 'docker'"
+arg_max_parallel_title = "Maximum number of parallel jobs"
+arg_max_parallel_desc = "Limit the maximum number of parallel jobs per step. By default the num_parallel argument of each individual step is used."
+
 
 # just cli
 arg_cli_config = "Path to %(prog)s yaml configuration file. Defaults to '.builderer.yml'"
 arg_cli_no_push = "Prevent pushing images in all steps."
 
 # just parameters
-conf_parameters = "Overwrite default parameters. Values set here will be overwritten by command line arguments."
+conf_parameters = "Overwrite default parameters. Values set here will in turn be overwritten by command line arguments."
 conf_steps = "List of steps to execute."
 
 # steps
 step_type = "Type of the step"
+step_num_parallel_tmpl = "Number of parallel executions. Defaults to {}"
 
 step_action_name = "Name printed before running the action"
 step_action_commands = "List of commands. Each command is a list of strings: the executable followed by arguments."
 step_action_post = "Whether to add the action to the post queue"
 
 step_build_directory = "Directory containing the Dockerfile. This is also used as the build context."
 step_build_directories = "Directories containing each containing Dockerfile."
@@ -40,14 +44,15 @@
 step_build_extra_tags = "Additional tags to use in this step. Defaults to None."
 
 step_extract_image = "Name of the image to copy from."
 step_extract_path = "Source path inside the image."
 step_extract_dest = "Destination paths. The file will be copied to all destinations individually."
 
 step_forward_name = "Image name to forward."
+step_forward_names = "Image names to forward."
 step_forward_new_name = (
     "Set a new name for the image. By default the basename of the pulled image without the tag is used."
 )
 step_forward_extra_tags = "Additional tags to use in this step. Defaults to None."
 
 step_pull_name = "Image name to pull."
 step_pull_names = "Image names to pull."
```

### Comparing `builderer-1.1.0/builderer/builderer.py` & `builderer-2.0.0/builderer/actions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,92 @@
-"""Builderers file config is a thin wrapper around this library."""
+"""Builderers file config is a thin wrapper around this module as well as the builderer module."""
 
-import collections
 import dataclasses
 import os
 import posixpath
-import subprocess
 import typing
 import uuid
 
 
 @dataclasses.dataclass(frozen=True)
 class Action:
+    """A named sequence of commands."""
+
     name: str
     commands: list[list[str]]
 
 
-class Builderer:
-    """The Builderer class is used to collect build tasks and issue them afterwards."""
+@dataclasses.dataclass
+class ActionGroup:
+    """A sequence of actions with many or may not be run in parallel."""
+
+    actions: list[Action]
+    num_parallel: int
+
+
+class ActionFactory:
+    """The ActionFactory class is used to create build tasks."""
 
     def __init__(
         self,
         *,
         registry: str | None = None,
         prefix: str | None = None,
         push: bool = True,
         cache: bool = False,
-        verbose: bool = False,
         tags: list[str] = ["latest"],
-        simulate: bool = False,
         backend: typing.Literal["docker", "podman"] = "docker",
     ) -> None:
-        """Builderer runs commands inside in two queues. A action queue and a post queue.
-        First the action queue gets handled (FIFO) then the corresponding post actions get called in reversed order (LIFO)
-        Pushing is done as a post steps. This means a build is only pushed if builder of all images was successfull.
+        """Create predefined or custom actions.
 
         Args:
             registry (str | None, optional): Registry URL. Defaults to None.
             prefix (str | None, optional): Registry folder / namespace / user. Defaults to None.
             push (bool, optional): Whether to allow pushing images. Defaults to True.
             cache (bool, optional): Allow using cached images. Defaults to False.
-            verbose (bool, optional): Verbose output. Defaults to False.
             tags (list[str], optional): Tags to use. Defaults to ["latest"].
-            simulate (bool, optional): Prevent issuing commands. Defaults to False.
             backend (typing.Literal["docker", "podman"], optional): Overwrite backend to use. Defaults to "docker".
         """
         self.tags = tags
         self.registry = registry
         self.prefix = prefix
         self.cache = cache
         self.backend = backend
-        self.simulate = simulate
-        self.verbose = verbose
         self.push = push
 
-        self._actions: collections.deque[Action] = collections.deque()
-        self._post: collections.deque[Action] = collections.deque()
-
-    def action(self, name: str, commands: list[list[str]], post: bool) -> None:
-        """A generic action with multiple commands.
+    def action(self, name: str, commands: list[list[str]]) -> Action:
+        """Create a generic action with multiple commands.
 
         Hint: Use this mechanism if other commands aren't sufficient for your usecase.
 
         Args:
             name (str): Name of the action
             commands (list[list[str]]): List of commands. Each command is a list of strings: the executable followed by arguments.
-            post (bool): Whether to add the action to the post queue.
         """
-        item = Action(name=name, commands=commands)
-
-        if post:
-            self._post.appendleft(item)
-        else:
-            self._actions.append(item)
+        return Action(name=name, commands=commands)
 
     def _full_image_name(self, name: str) -> str:
         return posixpath.join(self.registry or "", self.prefix or "", name)
 
     def _build_cmd(self, full_name: str, extra_tags: list[str]) -> list[str]:
         tags = [i for tag in (self.tags + extra_tags) for i in ["-t", f"{full_name}:{tag}"]]
         cache = ["--no-cache"] if not self.cache else []
 
         return [self.backend, "build", *tags, *cache]
 
-    def _run_cmd(self, command: list[str]) -> tuple[int, bytes]:
-        if self.simulate:
-            return 0, b""
-
-        if self.verbose:
-            proc = subprocess.run(command)
-        else:
-            proc = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-        return proc.returncode, proc.stdout or b""
-
     def build_image(
         self,
         directory: str,
         *,
         dockerfile: str | None = None,
         name: str | None = None,
         push: bool = True,
         qualified: bool = True,
         extra_tags: list[str] | None = None,
-    ) -> None:
+    ) -> tuple[Action, Action | None]:
         """Build a docker image and push it to the registry.
 
         Args:
             directory (str): Directory containing the build context.
             dockerfile (str | None, optional): Path to Dockerfile. Name of the resulting image. Defaults to <directory>/Dockerfile.
             name (str | None, optional): Name of the resulting image. Defaults to the name of the Dockerfiles parent directory.
             push (bool, optional): Whether to push the image. Defaults to True.
@@ -120,113 +100,87 @@
             name = os.path.basename(directory)
 
         if extra_tags is None:
             extra_tags = []
 
         image_name = self._full_image_name(name) if qualified else name
 
-        self.action(
+        action_main = self.action(
             name=f"Building image: {name}",
             commands=[[*self._build_cmd(image_name, extra_tags), "-f", dockerfile, directory]],
-            post=False,
         )
 
         if not push or not self.push:
-            return
+            return action_main, None
 
-        self.action(
+        action_post = self.action(
             name=f"Pushing image: {name}",
             commands=[[self.backend, "push", f"{image_name}:{tag}"] for tag in self.tags + extra_tags],
-            post=True,
         )
 
-    def extract_from_image(self, image: str, path: str, *dest: str) -> None:
+        return action_main, action_post
+
+    def extract_from_image(self, image: str, path: str, *dest: str) -> Action:
         """Copy a file from within a docker image.
 
         Args:
             image (str): Name of the image to copy from.
             path (str): Source path inside the image.
             dest (str): Destination paths. The file will be copied to all destinations individually.
         """
         container_name = str(uuid.uuid4())
 
-        self.action(
+        return self.action(
             name=f"Extracting from image: {path} -> {', '.join(dest)}",
             commands=[
                 [self.backend, "container", "create", "--name", container_name, image],
                 *[[self.backend, "container", "cp", f"{container_name}:{path}", dst] for dst in dest],
                 [self.backend, "container", "rm", "-f", container_name],
             ],
-            post=False,
         )
 
-    def forward_image(self, name: str, *, new_name: str | None = None, extra_tags: list[str] | None = None) -> None:
-        """Pulls an image from a registry, retags it and pushes it using the new names.
+    def forward_image(
+        self, name: str, *, new_name: str | None = None, extra_tags: list[str] | None = None
+    ) -> tuple[Action, Action | None]:
+        """Pull an image from a registry, retag it and push it using the new names.
 
         Args:
             name (str): image name to pull
             new_name (str | None, optional): Set a new name for the image. By default the basename of the pulled image without the tag is used. Defaults to None.
             extra_tags: additional tags to use for this image. Defaults to None.
         """
         if new_name is None:
             new_name = os.path.basename(name).split(":")[0]
 
         if extra_tags is None:
             extra_tags = []
 
         image_name = self._full_image_name(new_name)
 
-        self.action(
+        action_main = self.action(
             name=f"Forwarding image: {name} -> {new_name}",
             commands=[
                 [self.backend, "pull", name],
                 *[[self.backend, "tag", name, f"{image_name}:{tag}"] for tag in self.tags + extra_tags],
             ],
-            post=False,
         )
 
         if not self.push:
-            return
+            return action_main, None
 
-        self.action(
+        action_post = self.action(
             name=f"Pushing image: {new_name}",
             commands=[[self.backend, "push", f"{image_name}:{tag}"] for tag in self.tags + extra_tags],
-            post=True,
         )
 
-    def pull_image(self, name: str) -> None:
-        """Pulls an image from a registry. This might be usefull to ensure a local image is up to date (e.g. for local builds)
+        return action_main, action_post
+
+    def pull_image(self, name: str) -> Action:
+        """Pull an image from a registry. This might be usefull to ensure a local image is up to date (e.g. for local builds).
 
         Args:
             name (str): image name to pull.
         """
-        self.action(
+        return self.action(
             name=f"Pulling image: {name}",
             commands=[[self.backend, "pull", name]],
-            post=False,
         )
-
-    def run(self) -> int:
-        """After adding all steps. This method will start to issue all commands. It stops when done or a command fails.
-
-        Returns:
-            int: return code. On success this will be zero. Otherwise it will be the return code of the failed command.
-        """
-        for queue in [self._actions, self._post]:
-            for action in queue:
-                print(action.name, flush=True)
-
-                for command in action.commands:
-                    if self.verbose:
-                        print(f"{command}", flush=True)
-
-                    returncode, stdout = self._run_cmd(command)
-
-                    if returncode != 0:
-                        print("Encountered error running:", flush=True)
-
-                        if not self.verbose:
-                            print(stdout.decode(), flush=True)
-
-                        return returncode
-
-        return 0
```

### Comparing `builderer-1.1.0/builderer.egg-info/PKG-INFO` & `builderer-2.0.0/builderer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: builderer
-Version: 1.1.0
+Version: 2.0.0
 Summary: Container based mono repo builder.
 Home-page: https://github.com/florian-sattler/builderer/
 Author: Florian Sattler
 Author-email: dev@florian-sattler.de
 License: MIT
 Project-URL: Documentation, https://builderer.florian-sattler.de/
 Project-URL: Source, https://github.com/florian-sattler/builderer/
 Project-URL: Changelog, https://github.com/florian-sattler/builderer/blob/main/CHANGELOG.md
 Project-URL: Tracker, https://github.com/florian-sattler/builderer/issues
 Project-URL: Download, https://pypi.org/project/builderer/#files
 Keywords: builderer,continuous integration,continuous delivery
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -30,15 +31,15 @@
     </a>
     <h1>
         builderer
     </h1>
     <p>
         <em>Container based mono repo builder</em>
     </p>
-    <p> 
+    <p>
         <a href="https://pypi.python.org/pypi/builderer">
             <img src="https://img.shields.io/pypi/v/builderer.svg">
         </a>
         <a href="https://pepy.tech/project/builderer">
             <img src="https://pepy.tech/badge/builderer">
         </a>
         <a href="https://github.com/florian-sattler/builderer">
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: builderer Version: 1.1.0 Summary: Container based
+Metadata-Version: 2.1 Name: builderer Version: 2.0.0 Summary: Container based
 mono repo builder. Home-page: https://github.com/florian-sattler/builderer/
 Author: Florian Sattler Author-email: dev@florian-sattler.de License: MIT
 Project-URL: Documentation, https://builderer.florian-sattler.de/ Project-URL:
 Source, https://github.com/florian-sattler/builderer/ Project-URL: Changelog,
 https://github.com/florian-sattler/builderer/blob/main/CHANGELOG.md Project-
 URL: Tracker, https://github.com/florian-sattler/builderer/issues Project-URL:
 Download, https://pypi.org/project/builderer/#files Keywords:
-builderer,continuous integration,continuous delivery Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
+builderer,continuous integration,continuous delivery Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE
              [https://builderer.florian-sattler.de/logo-color.svg]
                             ****** builderer ******
                        Container based mono repo builder
     [https://img.shields.io/pypi/v/builderer.svg] [https://pepy.tech/badge/
    builderer] [https://img.shields.io/pypi/pyversions/builderer.svg] [PyPI_-
       License] [https://img.shields.io/github/v/release/florian-sattler/
  builderer?label=github] [https://img.shields.io/badge/docs-yes-brightgreen]
```

### Comparing `builderer-1.1.0/setup.cfg` & `builderer-2.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.0
+current_version = 2.0.0
 commit = True
 tag = True
 
 [metadata]
 name = builderer
 version = attr: builderer.__version__
 description = Container based mono repo builder.
@@ -21,14 +21,15 @@
 	continuous integration
 	continuous delivery
 author = Florian Sattler
 author_email = dev@florian-sattler.de
 license = MIT
 license_file = LICENSE
 classifiers = 
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.10
@@ -48,15 +49,17 @@
 	tests
 
 [options.entry_points]
 console_scripts = 
 	builderer = builderer.__main__:main
 
 [flake8]
-per-file-ignores = __init__.py:F401
+per-file-ignores = 
+	__init__.py:F401
+	tests/*:D100,D101,D103,D104,D105,D107
 extend-ignore = E501
 max-complexity = 10
 max-line-length = 120
 
 [tool:pytest]
 addopts = --ignore setup.py
```

### Comparing `builderer-1.1.0/tests/test___main__.py` & `builderer-2.0.0/tests/test___main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             [],
             ".builderer.yml",
             {},
         ),
         (
             [
                 "--registry",
-                "reg.examle.com:6789",
+                "reg.example.com:6789",
                 "--prefix",
                 "user",
                 "--tags",
                 "foo",
                 "bar",
                 "baz",
                 "--no-push",
@@ -35,15 +35,15 @@
                 "--backend",
                 "podman",
                 "--config",
                 "test.yaml",
             ],
             "test.yaml",
             {
-                "registry": "reg.examle.com:6789",
+                "registry": "reg.example.com:6789",
                 "prefix": "user",
                 "tags": ["foo", "bar", "baz"],
                 "push": False,
                 "cache": True,
                 "verbose": True,
                 "simulate": True,
                 "backend": "podman",
```

### Comparing `builderer-1.1.0/tests/test_file_config.py` & `builderer-2.0.0/tests/test_file_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
             "prefix": None,
             "push": None,
             "cache": None,
             "verbose": None,
             "tags": None,
             "simulate": None,
             "backend": None,
+            "max_parallel": None,
         },
     }
 
 
 def test_load_example(datadir: pathlib.Path) -> None:
     file_config = builderer.config.BuildererConfig.load(datadir / "example.yml")
 
@@ -30,14 +31,15 @@
             "prefix": "username",
             "push": False,
             "cache": False,
             "verbose": False,
             "tags": ["a", "b"],
             "simulate": True,
             "backend": "podman",
+            "max_parallel": 4,
         },
         "steps": [],
     }
 
 
 def test_load_example_workspace(datadir: pathlib.Path) -> None:
     file_config = builderer.config.BuildererConfig.load(datadir / "example_workspace" / ".builderer.yml")
@@ -48,20 +50,31 @@
             "prefix": "foo",
             "push": None,
             "cache": None,
             "verbose": None,
             "tags": None,
             "simulate": None,
             "backend": None,
+            "max_parallel": None,
         },
         "steps": [
-            {"type": "pull_images", "names": ["docker.io/python:alpine", "docker.io/nginx:alpine"]},
-            {"type": "forward_image", "name": "docker.io/redis:alpine", "new_name": None, "extra_tags": None},
+            {
+                "type": "pull_images",
+                "names": ["docker.io/python:alpine", "docker.io/nginx:alpine"],
+                "num_parallel": 4,
+            },
+            {
+                "type": "forward_image",
+                "name": "docker.io/redis:alpine",
+                "new_name": None,
+                "extra_tags": None,
+            },
             {
                 "type": "build_images",
                 "directories": ["frontend", "backend"],
                 "push": True,
                 "qualified": True,
                 "extra_tags": None,
+                "num_parallel": 1,
             },
         ],
     }
```

