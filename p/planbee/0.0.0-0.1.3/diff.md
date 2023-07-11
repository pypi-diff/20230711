# Comparing `tmp/planbee-0.0.0.tar.gz` & `tmp/planbee-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planbee-0.0.0.tar", last modified: Tue Jul 11 10:08:15 2023, max compression
+gzip compressed data, was "planbee-0.1.3.tar", last modified: Tue Jul 11 11:10:29 2023, max compression
```

## Comparing `planbee-0.0.0.tar` & `planbee-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.491519 planbee-0.0.0/
--rw-rw-rw-   0        0        0     1101 2023-07-10 10:01:35.000000 planbee-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     2317 2023-07-11 10:08:15.491519 planbee-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1721 2023-07-10 12:02:28.000000 planbee-0.0.0/README.md
--rw-rw-rw-   0        0        0      565 2023-07-11 10:08:15.493933 planbee-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-07-11 10:07:57.000000 planbee-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.432574 planbee-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.442296 planbee-0.0.0/src/planbee/
--rw-rw-rw-   0        0        0      151 2023-07-10 12:04:21.000000 planbee-0.0.0/src/planbee/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.475322 planbee-0.0.0/src/planbee/models/
--rw-rw-rw-   0        0        0        0 2023-05-08 06:59:10.000000 planbee-0.0.0/src/planbee/models/__init__.py
--rw-rw-rw-   0        0        0     1450 2023-06-28 09:29:45.000000 planbee-0.0.0/src/planbee/models/resource.py
--rw-rw-rw-   0        0        0     1804 2023-07-07 11:45:40.000000 planbee-0.0.0/src/planbee/models/task.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.482316 planbee-0.0.0/src/planbee/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-08 06:59:10.000000 planbee-0.0.0/src/planbee/scheduler/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-28 09:21:34.000000 planbee-0.0.0/src/planbee/scheduler/core.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.489784 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:57:51.000000 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/__init__.py
--rw-rw-rw-   0        0        0     3792 2023-07-05 13:48:01.000000 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/main.py
--rw-rw-rw-   0        0        0    11080 2023-07-11 07:59:21.000000 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/task_allocator.py
--rw-rw-rw-   0        0        0     2494 2023-06-16 08:45:57.000000 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/task_graph.py
--rw-rw-rw-   0        0        0     6850 2023-06-29 07:34:04.000000 planbee-0.0.0/src/planbee/scheduler/heuristic_solver/window_manager.py
--rw-rw-rw-   0        0        0     3144 2023-06-27 09:01:48.000000 planbee-0.0.0/src/planbee/scheduler/scheduler_result.py
--rw-rw-rw-   0        0        0       58 2023-05-08 06:59:10.000000 planbee-0.0.0/src/planbee/scheduler/visualizations.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:08:15.470648 planbee-0.0.0/src/planbee.egg-info/
--rw-rw-rw-   0        0        0     2317 2023-07-11 10:08:15.000000 planbee-0.0.0/src/planbee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-07-11 10:08:15.000000 planbee-0.0.0/src/planbee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:08:15.000000 planbee-0.0.0/src/planbee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 06:25:50.000000 planbee-0.0.0/src/planbee.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-07-11 10:08:15.000000 planbee-0.0.0/src/planbee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 10:08:15.000000 planbee-0.0.0/src/planbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.385908 planbee-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-11 11:10:26.000000 planbee-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-11 11:10:29.385908 planbee-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-11 11:10:26.000000 planbee-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 11:10:29.385908 planbee-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 11:10:26.000000 planbee-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.377908 planbee-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.385908 planbee-0.1.3/src/planbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 11:10:29.385908 planbee-0.1.3/src/planbee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/window_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/top_level.txt
```

### Comparing `planbee-0.0.0/LICENSE` & `planbee-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Jacob Østergaard Nielsen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Jacob Østergaard Nielsen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `planbee-0.0.0/README.md` & `planbee-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# PlanBee 🐝
-
-If Plan A fails, dont worry there is always PlanBee! PlanBee is a Job Shop Scheduling algorithm module buzzing with features. Feed PlanBee with your tasks and resources and it quickly finds a solution. It employs the high-speed computation power of NumPy to achieve fast results. With PlanBee, Plan B becomes your Plan A!
-
-## Features 🚀
-
-- Define your own tasks and resources.
-- Specify available windows for each resource.
-- Indicate priority, duration, and necessary resources for each task.
-- Solve your scheduling problems with a single function call!
-- Get a detailed summary and visualization of the scheduling solution.
-
-## Installation 🛠️
-
-```sh
-pip install planbee
-```
-
-## Usage 🐍
-
-First, import the necessary modules:
-
-```python
-from PlanBee import Resource, Task, Scheduler
-```
-
-Then, define your resources:
-
-```python
-resource1 = Resource(id=1, available_windows=[(0, 10), (15, 20)])
-resource2 = Resource(id=2, available_windows=[(5, 20)])
-```
-
-And your tasks:
-
-```python
-task1 = Task(id=1, duration=5, priority=1, resources=[resource1, resource2], resource_count=1)
-task2 = Task(id=2, duration=3, priority=2, resources=[resource1], predecessors=[task1], resource_count=1)
-```
-
-Finally, use the Scheduler to solve:
-
-```python
-scheduler = Scheduler(tasks=[task1, task2])
-result = scheduler.schedule()
-```
-
-## Visualization 📊
-
-PlanBee provides a function to plot your schedule:
-
-```python
-result.plot_resource_plan()
-```
-
-## Contributions 💡
-
-Contributions are always welcome! See `CONTRIBUTING.md` for ways to get started.
-
-## License 📄
-
-This project is licensed under the terms of the [MIT license](LICENSE.md).
+# PlanBee 🐝
+
+If Plan A fails, dont worry there is always PlanBee! PlanBee is a Job Shop Scheduling algorithm module buzzing with features. Feed PlanBee with your tasks and resources and it quickly finds a solution. It employs the high-speed computation power of NumPy to achieve fast results. With PlanBee, Plan B becomes your Plan A!
+
+## Features 🚀
+
+- Define your own tasks and resources.
+- Specify available windows for each resource.
+- Indicate priority, duration, and necessary resources for each task.
+- Solve your scheduling problems with a single function call!
+- Get a detailed summary and visualization of the scheduling solution.
+
+## Installation 🛠️
+
+```sh
+pip install planbee
+```
+
+## Usage 🐍
+
+First, import the necessary modules:
+
+```python
+from PlanBee import Resource, Task, Scheduler
+```
+
+Then, define your resources:
+
+```python
+resource1 = Resource(id=1, available_windows=[(0, 10), (15, 20)])
+resource2 = Resource(id=2, available_windows=[(5, 20)])
+```
+
+And your tasks:
+
+```python
+task1 = Task(id=1, duration=5, priority=1, resources=[resource1, resource2], resource_count=1)
+task2 = Task(id=2, duration=3, priority=2, resources=[resource1], predecessors=[task1], resource_count=1)
+```
+
+Finally, use the Scheduler to solve:
+
+```python
+scheduler = Scheduler(tasks=[task1, task2])
+result = scheduler.schedule()
+```
+
+## Visualization 📊
+
+PlanBee provides a function to plot your schedule:
+
+```python
+result.plot_resource_plan()
+```
+
+## Contributions 💡
+
+Contributions are always welcome! See `CONTRIBUTING.md` for ways to get started.
+
+## License 📄
+
+This project is licensed under the terms of the [MIT license](LICENSE.md).
```

### Comparing `planbee-0.0.0/src/planbee/models/resource.py` & `planbee-0.1.3/src/planbee/models/resource.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import numpy as np
-from pydantic import BaseModel
-
-
-class Resource(BaseModel):
-    id: int
-    available_windows: list[tuple[int, int]] = []
-    efficiency_multiplier: float = 1
-
-    def __hash__(self):
-        return hash(self.id)
-
-    def __eq__(self, other):
-        if isinstance(other, Resource):
-            return self.id == other.id
-        return False
-
-    def merge_intervals(self) -> None:
-        """
-        Merges overlapping intervals in available_windows.
-
-        The method sorts the available windows based on the start times,
-        and then merges overlapping intervals.
-        """
-        if len(self.available_windows) == 0:
-            return
-
-        # Convert the available_windows to a numpy array
-        windows = np.array(self.available_windows, dtype=np.int32)
-
-        # Sort the array by start times
-        windows = windows[np.argsort(windows[:, 0])]
-
-        # Find where the current start is greater than the previous end
-        idx = np.where(windows[:-1, 1] < windows[1:, 0])[0]
-
-        # Stack end indices for intervals to merge with the next start indices
-        end_indices = np.hstack((idx, len(windows) - 1))
-        start_indices = np.hstack((0, idx + 1))
-
-        # The following line of code creates the merged intervals
-        self.available_windows = [
-            (windows[i, 0], windows[j, 1]) for i, j in zip(start_indices, end_indices)
-        ]
+import numpy as np
+from pydantic import BaseModel
+
+
+class Resource(BaseModel):
+    id: int
+    available_windows: list[tuple[int, int]] = []
+    efficiency_multiplier: float = 1
+
+    def __hash__(self):
+        return hash(self.id)
+
+    def __eq__(self, other):
+        if isinstance(other, Resource):
+            return self.id == other.id
+        return False
+
+    def merge_intervals(self) -> None:
+        """
+        Merges overlapping intervals in available_windows.
+
+        The method sorts the available windows based on the start times,
+        and then merges overlapping intervals.
+        """
+        if len(self.available_windows) == 0:
+            return
+
+        # Convert the available_windows to a numpy array
+        windows = np.array(self.available_windows, dtype=np.int32)
+
+        # Sort the array by start times
+        windows = windows[np.argsort(windows[:, 0])]
+
+        # Find where the current start is greater than the previous end
+        idx = np.where(windows[:-1, 1] < windows[1:, 0])[0]
+
+        # Stack end indices for intervals to merge with the next start indices
+        end_indices = np.hstack((idx, len(windows) - 1))
+        start_indices = np.hstack((0, idx + 1))
+
+        # The following line of code creates the merged intervals
+        self.available_windows = [
+            (windows[i, 0], windows[j, 1]) for i, j in zip(start_indices, end_indices)
+        ]
```

### Comparing `planbee-0.0.0/src/planbee/models/task.py` & `planbee-0.1.3/src/planbee/models/task.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from itertools import count
-from typing import Optional, Union
-
-from pydantic import BaseModel, validator
-
-from .resource import Resource
-
-
-class Task(BaseModel):
-    id: int
-    duration: int
-    priority: int
-    resources: list[list[Resource]]
-    resource_count: Union[int, str] = 1
-    predecessors: Optional[list["Task"]] = []
-    predecessor_delay: int = 0
-
-    @validator("resources", pre=True)
-    def ensure_list(cls, v):
-        if not isinstance(v, list):  # if a single resource object is passed
-            return [[v]]  # make it a list of list
-        if (
-            isinstance(v, list) and len(v) > 0 and not isinstance(v[0], list)
-        ):  # if a list of resources is passed
-            return [v]  # make it a list of list
-        return v  # if a list of lists is passed, return as it is
-
-    def get_resources(self):
-        return [
-            resource for resource_list in self.resources for resource in resource_list
-        ]
-
-    def get_resource_group_count(self):
-        return len(self.resources)
-
-    def get_resource_group_indices(self) -> list[list[int]]:
-        """
-        returns a list of lists of indices of resources in each resource group
-        """
-        counter = count()
-        return [[next(counter) for _ in sublist] for sublist in self.resources]
-
-    @validator("resource_count", always=True)
-    def set_resource_count(cls, v, values):
-        if isinstance(v, str) and v.lower() == "all":
-            if "resources" in values:
-                return max(
-                    len(resource_group) for resource_group in values["resources"]
-                )
-
-        elif isinstance(v, int):
-            return v
-        else:
-            raise ValueError("Invalid value for resource_count.")
+from itertools import count
+from typing import Optional, Union
+
+from pydantic import BaseModel, validator
+
+from .resource import Resource
+
+
+class Task(BaseModel):
+    id: int
+    duration: int
+    priority: int
+    resources: list[list[Resource]]
+    resource_count: Union[int, str] = 1
+    predecessors: Optional[list["Task"]] = []
+    predecessor_delay: int = 0
+
+    @validator("resources", pre=True)
+    def ensure_list(cls, v):
+        if not isinstance(v, list):  # if a single resource object is passed
+            return [[v]]  # make it a list of list
+        if (
+            isinstance(v, list) and len(v) > 0 and not isinstance(v[0], list)
+        ):  # if a list of resources is passed
+            return [v]  # make it a list of list
+        return v  # if a list of lists is passed, return as it is
+
+    def get_resources(self):
+        return [
+            resource for resource_list in self.resources for resource in resource_list
+        ]
+
+    def get_resource_group_count(self):
+        return len(self.resources)
+
+    def get_resource_group_indices(self) -> list[list[int]]:
+        """
+        returns a list of lists of indices of resources in each resource group
+        """
+        counter = count()
+        return [[next(counter) for _ in sublist] for sublist in self.resources]
+
+    @validator("resource_count", always=True)
+    def set_resource_count(cls, v, values):
+        if isinstance(v, str) and v.lower() == "all":
+            if "resources" in values:
+                return max(
+                    len(resource_group) for resource_group in values["resources"]
+                )
+
+        elif isinstance(v, int):
+            return v
+        else:
+            raise ValueError("Invalid value for resource_count.")
```

### Comparing `planbee-0.0.0/src/planbee/scheduler/heuristic_solver/main.py` & `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/main.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import numpy as np
-
-from .task_allocator import TaskAllocator
-from .task_graph import TaskGraph
-from .window_manager import WindowManager
-
-
-class HeuristicSolver:
-    def __init__(self, tasks, resources):
-        self.task_allocator = TaskAllocator()
-        self.task_graph = TaskGraph(tasks)
-        self.window_manager = WindowManager(resources)
-        self.task_vars = {
-            task.id: {
-                "task_id": task.id,
-                "assigned_resource_ids": None,
-                "task_start": None,
-                "task_end": None,
-                "resource_intervals": None,
-            }
-            for task in tasks
-        }
-        self.task_dict = {task.id: task for task in tasks}
-
-    def solve(self):
-        task_order = self.task_graph.get_task_order()
-        unscheduled_tasks = []
-
-        for task_id in task_order:
-            task = self.task_dict[task_id]
-
-            # get task resources and windows dict
-            task_resource_ids = [resource.id for resource in task.get_resources()]
-            task_earliest_start = self._get_task_earliest_start(task)
-
-            if task_earliest_start is None:
-                unscheduled_tasks.append(task_id)
-                continue
-
-            task_resource_windows_dict = (
-                self.window_manager.get_task_resource_windows_dict(
-                    task_resource_ids, task_earliest_start
-                )
-            )
-            if not task_resource_windows_dict:
-                unscheduled_tasks.append(task_id)
-                continue
-
-            # allocate task
-            allocated_resource_windows_dict = self.task_allocator.allocate_task(
-                resource_windows_dict=task_resource_windows_dict,
-                task_duration=task.duration,
-                resource_count=task.resource_count,
-                resource_group_indices=task.get_resource_group_indices(),
-            )
-
-            if not allocated_resource_windows_dict:
-                unscheduled_tasks.append(task_id)
-                continue
-
-            resource_windows_min_max = self.min_max_dict_np(
-                allocated_resource_windows_dict
-            )
-
-            # update resource windows
-            self.window_manager.update_resource_windows(resource_windows_min_max)
-
-            # Append task values
-            task_values = {
-                "task_id": task_id,
-                "assigned_resource_ids": list(allocated_resource_windows_dict.keys()),
-                "task_start": min(
-                    start for start, _ in resource_windows_min_max.values()
-                ),
-                "task_end": max(end for _, end in resource_windows_min_max.values()),
-                "resource_intervals": allocated_resource_windows_dict.values(),
-            }
-            self.task_vars[task_id] = task_values
-
-        return list(
-            self.task_vars.values()
-        )  # Return values of the dictionary as a list
-
-    def _get_task_earliest_start(self, task):
-        """
-        Retuns the earliest start of a task based on the latest end of its predecessors.
-        """
-        task_ends = []
-        for pred in task.predecessors:
-            task_end = self.task_vars[pred.id]["task_end"]
-            if task_end is None:
-                return None
-            task_ends.append(task_end + task.predecessor_delay)
-
-        return max(task_ends, default=0)
-
-    def min_max_dict_np(self, d):
-        result = {}
-
-        for key, value_list in d.items():
-            min_val = np.min([x[0] for x in value_list])
-            max_val = np.max([x[1] for x in value_list])
-            result[key] = (min_val, max_val)
-
-        return result
-        return result
+import numpy as np
+
+from .task_allocator import TaskAllocator
+from .task_graph import TaskGraph
+from .window_manager import WindowManager
+
+
+class HeuristicSolver:
+    def __init__(self, tasks, resources):
+        self.task_allocator = TaskAllocator()
+        self.task_graph = TaskGraph(tasks)
+        self.window_manager = WindowManager(resources)
+        self.task_vars = {
+            task.id: {
+                "task_id": task.id,
+                "assigned_resource_ids": None,
+                "task_start": None,
+                "task_end": None,
+                "resource_intervals": None,
+            }
+            for task in tasks
+        }
+        self.task_dict = {task.id: task for task in tasks}
+
+    def solve(self):
+        task_order = self.task_graph.get_task_order()
+        unscheduled_tasks = []
+
+        for task_id in task_order:
+            task = self.task_dict[task_id]
+
+            # get task resources and windows dict
+            task_resource_ids = [resource.id for resource in task.get_resources()]
+            task_earliest_start = self._get_task_earliest_start(task)
+
+            if task_earliest_start is None:
+                unscheduled_tasks.append(task_id)
+                continue
+
+            task_resource_windows_dict = (
+                self.window_manager.get_task_resource_windows_dict(
+                    task_resource_ids, task_earliest_start
+                )
+            )
+            if not task_resource_windows_dict:
+                unscheduled_tasks.append(task_id)
+                continue
+
+            # allocate task
+            allocated_resource_windows_dict = self.task_allocator.allocate_task(
+                resource_windows_dict=task_resource_windows_dict,
+                task_duration=task.duration,
+                resource_count=task.resource_count,
+                resource_group_indices=task.get_resource_group_indices(),
+            )
+
+            if not allocated_resource_windows_dict:
+                unscheduled_tasks.append(task_id)
+                continue
+
+            resource_windows_min_max = self.min_max_dict_np(
+                allocated_resource_windows_dict
+            )
+
+            # update resource windows
+            self.window_manager.update_resource_windows(resource_windows_min_max)
+
+            # Append task values
+            task_values = {
+                "task_id": task_id,
+                "assigned_resource_ids": list(allocated_resource_windows_dict.keys()),
+                "task_start": min(
+                    start for start, _ in resource_windows_min_max.values()
+                ),
+                "task_end": max(end for _, end in resource_windows_min_max.values()),
+                "resource_intervals": allocated_resource_windows_dict.values(),
+            }
+            self.task_vars[task_id] = task_values
+
+        return list(
+            self.task_vars.values()
+        )  # Return values of the dictionary as a list
+
+    def _get_task_earliest_start(self, task):
+        """
+        Retuns the earliest start of a task based on the latest end of its predecessors.
+        """
+        task_ends = []
+        for pred in task.predecessors:
+            task_end = self.task_vars[pred.id]["task_end"]
+            if task_end is None:
+                return None
+            task_ends.append(task_end + task.predecessor_delay)
+
+        return max(task_ends, default=0)
+
+    def min_max_dict_np(self, d):
+        result = {}
+
+        for key, value_list in d.items():
+            min_val = np.min([x[0] for x in value_list])
+            max_val = np.max([x[1] for x in value_list])
+            result[key] = (min_val, max_val)
+
+        return result
+        return result
```

### Comparing `planbee-0.0.0/src/planbee/scheduler/heuristic_solver/task_graph.py` & `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_graph.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import networkx as nx
-
-
-class TaskGraph:
-    def __init__(self, tasks):
-        self.tasks = {task.id: task for task in tasks}
-        self.graph = self._create_task_graph()
-
-    def _create_task_graph(self):
-        """
-        Creates a directed acyclic graph from the given tasks.
-        """
-        task_graph = nx.DiGraph()
-        for task in self.tasks.values():
-            task_graph.add_node(task.id, duration=task.duration, priority=task.priority)
-            for predecessor in task.predecessors:
-                task_graph.add_edge(predecessor.id, task.id)
-        return task_graph
-
-    def _compute_longest_paths(self):
-        """
-        Computes the longest path for each node in the task graph using a topological
-        sort.
-        """
-        longest_path = {task_id: 0 for task_id in self.tasks}
-        for task in nx.topological_sort(self.graph):
-            duration = self.graph.nodes[task]["duration"]
-            for predecessor in self.graph.predecessors(task):
-                longest_path[task] = max(
-                    longest_path[task], longest_path[predecessor] + duration
-                )
-        return longest_path
-
-    def _custom_topological_sort(self, longest_path):
-        """
-        Performs a custom topological sort of tasks considering priority and longest
-        path.
-        """
-        visited = set()
-        result = []
-
-        def visit(node):
-            """
-            Recursive function to traverse the task graph in the desired order.
-            """
-            if node not in visited:
-                visited.add(node)
-                predecessors = sorted(
-                    self.graph.predecessors(node),
-                    key=lambda n: (self.graph.nodes[n]["priority"], -longest_path[n]),
-                )
-                for predecessor in predecessors:
-                    visit(predecessor)
-                result.append(node)
-
-        for task in sorted(
-            self.tasks.values(),
-            key=lambda t: (self.graph.nodes[t.id]["priority"], -longest_path[t.id]),
-        ):
-            visit(task.id)
-
-        return result
-
-    def get_task_order(self):
-        """
-        Returns a list of task IDs in the order required to complete them as quickly
-        as possible while considering task priorities.
-        """
-        longest_path = self._compute_longest_paths()
-        return self._custom_topological_sort(longest_path)
+import networkx as nx
+
+
+class TaskGraph:
+    def __init__(self, tasks):
+        self.tasks = {task.id: task for task in tasks}
+        self.graph = self._create_task_graph()
+
+    def _create_task_graph(self):
+        """
+        Creates a directed acyclic graph from the given tasks.
+        """
+        task_graph = nx.DiGraph()
+        for task in self.tasks.values():
+            task_graph.add_node(task.id, duration=task.duration, priority=task.priority)
+            for predecessor in task.predecessors:
+                task_graph.add_edge(predecessor.id, task.id)
+        return task_graph
+
+    def _compute_longest_paths(self):
+        """
+        Computes the longest path for each node in the task graph using a topological
+        sort.
+        """
+        longest_path = {task_id: 0 for task_id in self.tasks}
+        for task in nx.topological_sort(self.graph):
+            duration = self.graph.nodes[task]["duration"]
+            for predecessor in self.graph.predecessors(task):
+                longest_path[task] = max(
+                    longest_path[task], longest_path[predecessor] + duration
+                )
+        return longest_path
+
+    def _custom_topological_sort(self, longest_path):
+        """
+        Performs a custom topological sort of tasks considering priority and longest
+        path.
+        """
+        visited = set()
+        result = []
+
+        def visit(node):
+            """
+            Recursive function to traverse the task graph in the desired order.
+            """
+            if node not in visited:
+                visited.add(node)
+                predecessors = sorted(
+                    self.graph.predecessors(node),
+                    key=lambda n: (self.graph.nodes[n]["priority"], -longest_path[n]),
+                )
+                for predecessor in predecessors:
+                    visit(predecessor)
+                result.append(node)
+
+        for task in sorted(
+            self.tasks.values(),
+            key=lambda t: (self.graph.nodes[t.id]["priority"], -longest_path[t.id]),
+        ):
+            visit(task.id)
+
+        return result
+
+    def get_task_order(self):
+        """
+        Returns a list of task IDs in the order required to complete them as quickly
+        as possible while considering task priorities.
+        """
+        longest_path = self._compute_longest_paths()
+        return self._custom_topological_sort(longest_path)
```

### Comparing `planbee-0.0.0/src/planbee/scheduler/scheduler_result.py` & `planbee-0.1.3/src/planbee/scheduler/scheduler_result.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-# scheduler_result.py
-import matplotlib.pyplot as plt
-import pandas as pd
-import seaborn as sns
-
-
-class SchedulerResult:
-    def __init__(self, task_vars):
-        self.task_vars = task_vars
-        self.unscheduled_tasks = [
-            task["task_id"]
-            for task in self.task_vars
-            if task["assigned_resource_ids"] is None
-        ]
-
-    def to_dict(self):
-        return self.task_vars
-
-    def to_dataframe(self):
-        df = pd.DataFrame(self.task_vars)
-        return df
-
-    def summary(self):
-        summary = f"Scheduled {len(self.task_vars) - len(self.unscheduled_tasks)} of {len(self.task_vars)} tasks."
-        if self.unscheduled_tasks:
-            summary += f"\nNo available resources found for task ids: {', '.join(map(str, self.unscheduled_tasks))}"
-        return summary
-
-    def plot_resource_plan(self) -> None:
-        df = self.get_resource_intervals_df()
-
-        # Create a color dictionary for each unique resource for distinction in the plot
-        tasks = df["task_id"].unique()
-        colors = sns.color_palette(
-            "deep", len(tasks)
-        )  # Using seaborn "dark" color palette
-        color_dict = dict(zip(tasks, colors))
-
-        # Set seaborn style
-        sns.set_style("whitegrid")
-
-        plt.figure(figsize=(12, 6))
-
-        for task_id, group_df in df.groupby("task_id"):
-            for task in group_df.itertuples():
-                plt.barh(
-                    task.resource_id,
-                    left=task.interval_start,
-                    width=task.interval_end - task.interval_start,
-                    color=color_dict[task_id],
-                    edgecolor="black",
-                )
-                plt.text(
-                    x=(task.interval_start + task.interval_end)
-                    / 2,  # x position, in the middle of task bar
-                    y=task.resource_id,  # y position, on the resource line
-                    s=task.task_id,  # text string, which is task_id here
-                    va="center",  # vertical alignment
-                    ha="center",  # horizontal alignment
-                    color="black",  # text color
-                    fontsize=10,
-                )  # font size
-
-        plt.xlabel("Time")
-        plt.ylabel("Resource")
-        plt.title("Resource Plan")
-        plt.yticks(df["resource_id"].unique())
-        plt.tight_layout()  # adjusts subplot params so that the subplot(s) fits into the figure area.
-        plt.show()
-
-    def get_resource_intervals_df(self) -> pd.DataFrame:
-        df = self.to_dataframe()
-        df = df.explode(["assigned_resource_ids", "resource_intervals"]).explode(
-            "resource_intervals"
-        )
-        df = df.dropna()
-        df["interval_start"] = df.resource_intervals.apply(lambda x: x[0])
-        df["interval_end"] = df.resource_intervals.apply(lambda x: x[1])
-        df = df.rename(columns={"assigned_resource_ids": "resource_id"})
-        df = df[["task_id", "resource_id", "interval_start", "interval_end"]]
-        df = df.infer_objects()
-        return df
+# scheduler_result.py
+import matplotlib.pyplot as plt
+import pandas as pd
+import seaborn as sns
+
+
+class SchedulerResult:
+    def __init__(self, task_vars):
+        self.task_vars = task_vars
+        self.unscheduled_tasks = [
+            task["task_id"]
+            for task in self.task_vars
+            if task["assigned_resource_ids"] is None
+        ]
+
+    def to_dict(self):
+        return self.task_vars
+
+    def to_dataframe(self):
+        df = pd.DataFrame(self.task_vars)
+        return df
+
+    def summary(self):
+        summary = f"Scheduled {len(self.task_vars) - len(self.unscheduled_tasks)} of {len(self.task_vars)} tasks."
+        if self.unscheduled_tasks:
+            summary += f"\nNo available resources found for task ids: {', '.join(map(str, self.unscheduled_tasks))}"
+        return summary
+
+    def plot_resource_plan(self) -> None:
+        df = self.get_resource_intervals_df()
+
+        # Create a color dictionary for each unique resource for distinction in the plot
+        tasks = df["task_id"].unique()
+        colors = sns.color_palette(
+            "deep", len(tasks)
+        )  # Using seaborn "dark" color palette
+        color_dict = dict(zip(tasks, colors))
+
+        # Set seaborn style
+        sns.set_style("whitegrid")
+
+        plt.figure(figsize=(12, 6))
+
+        for task_id, group_df in df.groupby("task_id"):
+            for task in group_df.itertuples():
+                plt.barh(
+                    task.resource_id,
+                    left=task.interval_start,
+                    width=task.interval_end - task.interval_start,
+                    color=color_dict[task_id],
+                    edgecolor="black",
+                )
+                plt.text(
+                    x=(task.interval_start + task.interval_end)
+                    / 2,  # x position, in the middle of task bar
+                    y=task.resource_id,  # y position, on the resource line
+                    s=task.task_id,  # text string, which is task_id here
+                    va="center",  # vertical alignment
+                    ha="center",  # horizontal alignment
+                    color="black",  # text color
+                    fontsize=10,
+                )  # font size
+
+        plt.xlabel("Time")
+        plt.ylabel("Resource")
+        plt.title("Resource Plan")
+        plt.yticks(df["resource_id"].unique())
+        plt.tight_layout()  # adjusts subplot params so that the subplot(s) fits into the figure area.
+        plt.show()
+
+    def get_resource_intervals_df(self) -> pd.DataFrame:
+        df = self.to_dataframe()
+        df = df.explode(["assigned_resource_ids", "resource_intervals"]).explode(
+            "resource_intervals"
+        )
+        df = df.dropna()
+        df["interval_start"] = df.resource_intervals.apply(lambda x: x[0])
+        df["interval_end"] = df.resource_intervals.apply(lambda x: x[1])
+        df = df.rename(columns={"assigned_resource_ids": "resource_id"})
+        df = df[["task_id", "resource_id", "interval_start", "interval_end"]]
+        df = df.infer_objects()
+        return df
```

### Comparing `planbee-0.0.0/src/planbee.egg-info/SOURCES.txt` & `planbee-0.1.3/src/planbee.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/planbee/__init__.py
+src/planbee/_version.py
 src/planbee.egg-info/PKG-INFO
 src/planbee.egg-info/SOURCES.txt
 src/planbee.egg-info/dependency_links.txt
 src/planbee.egg-info/not-zip-safe
 src/planbee.egg-info/requires.txt
 src/planbee.egg-info/top_level.txt
 src/planbee/models/__init__.py
```

