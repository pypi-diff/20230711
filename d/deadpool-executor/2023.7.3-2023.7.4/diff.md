# Comparing `tmp/deadpool_executor-2023.7.3.tar.gz` & `tmp/deadpool_executor-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool_executor-2023.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deadpool_executor-2023.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool_executor-2023.7.3.tar` & `deadpool_executor-2023.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/.coveragerc
--rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.3/LICENSE
--rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.3/README.rst
--rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/covstart.pth
--rw-r--r--   0        0        0    24011 2023-07-11 08:20:31.621096 deadpool_executor-2023.7.3/deadpool.py
--rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/examples/callbacks.py
--rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.3/examples/entrypoint.py
--rw-r--r--   0        0        0      961 2023-07-11 08:20:11.089233 deadpool_executor-2023.7.3/examples/leftover.py
--rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/examples/priorities.py
--rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/noxfile.py
--rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.3/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/tests/conftest.py
--rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/tests/test_deadpool.py
--rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.4/LICENSE
+-rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.4/README.rst
+-rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/covstart.pth
+-rw-r--r--   0        0        0    23912 2023-07-11 09:24:29.569757 deadpool_executor-2023.7.4/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/examples/callbacks.py
+-rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.4/examples/entrypoint.py
+-rw-r--r--   0        0        0      961 2023-07-11 08:20:11.089233 deadpool_executor-2023.7.4/examples/leftover.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/examples/priorities.py
+-rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/noxfile.py
+-rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.4/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/tests/conftest.py
+-rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/tests/test_deadpool.py
+-rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.4/PKG-INFO
```

### Comparing `deadpool_executor-2023.7.3/LICENSE` & `deadpool_executor-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/README.rst` & `deadpool_executor-2023.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/deadpool.py` & `deadpool_executor-2023.7.4/deadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dataclasses import dataclass, field
 from multiprocessing.connection import Connection
 from queue import Empty, PriorityQueue, Queue, SimpleQueue
 from typing import Callable, Optional, Tuple
 
 import psutil
 
-__version__ = "2023.7.3"
+__version__ = "2023.7.4"
 __all__ = [
     "Deadpool",
     "Future",
     "CancelledError",
     "TimeoutError",
     "ProcessError",
     "PoolClosed",
@@ -570,21 +570,18 @@
     tparent.start()
 
     def deactivate_parentless_self_destruct():
         evt.set()
 
     proc = psutil.Process()
     pid = proc.pid
-    lock = threading.Lock()
 
     def conn_send_safe(obj):
         try:
-            # TODO: this may not be necessary
-            with lock:
-                conn.send(obj)
+            conn.send(obj)
         except BrokenPipeError:  # pragma: no cover
             logger.debug("Pipe not usable")
         except BaseException:
             logger.exception("Unexpected pipe error")
 
     def timed_out():
         """Action to fire when the timeout given to ``threading.Timer``
@@ -673,15 +670,15 @@
     # synchronization controls are needed to tell the threads
     # to exit, which we don't have. However, we do have a kill
     # switch. Since this process worker will process no more
     # work, and since we've already fun the finalizer, we may
     # as well just nuke it. That will remove its memory space
     # and all its threads too.
     deactivate_parentless_self_destruct()
-    logger.debug(f"Nuking worker {pid=}")
+    logger.debug(f"Deleting worker {pid=}")
     kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
 
 
 def kill_proc_tree_in_process_daemon(pid, sig):  # pragma: no cover
     mp.Process(target=kill_proc_tree, args=(pid, sig), daemon=True).start()
```

### Comparing `deadpool_executor-2023.7.3/examples/entrypoint.py` & `deadpool_executor-2023.7.4/examples/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/examples/leftover.py` & `deadpool_executor-2023.7.4/examples/leftover.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/examples/priorities.py` & `deadpool_executor-2023.7.4/examples/priorities.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/noxfile.py` & `deadpool_executor-2023.7.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/pyproject.toml` & `deadpool_executor-2023.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/tests/test_deadpool.py` & `deadpool_executor-2023.7.4/tests/test_deadpool.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.3/PKG-INFO` & `deadpool_executor-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

