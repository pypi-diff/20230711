# Comparing `tmp/deadpool_executor-2023.7.2.tar.gz` & `tmp/deadpool_executor-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool_executor-2023.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deadpool_executor-2023.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool_executor-2023.7.2.tar` & `deadpool_executor-2023.7.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/.coveragerc
--rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.2/LICENSE
--rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.2/README.rst
--rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/covstart.pth
--rw-r--r--   0        0        0    22394 2023-07-10 00:01:01.439799 deadpool_executor-2023.7.2/deadpool.py
--rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/examples/callbacks.py
--rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.2/examples/entrypoint.py
--rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/examples/priorities.py
--rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/noxfile.py
--rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/tests/conftest.py
--rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/tests/test_deadpool.py
--rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.3/LICENSE
+-rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.3/README.rst
+-rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/covstart.pth
+-rw-r--r--   0        0        0    24011 2023-07-11 08:20:31.621096 deadpool_executor-2023.7.3/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/examples/callbacks.py
+-rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.3/examples/entrypoint.py
+-rw-r--r--   0        0        0      961 2023-07-11 08:20:11.089233 deadpool_executor-2023.7.3/examples/leftover.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/examples/priorities.py
+-rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/noxfile.py
+-rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.3/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/tests/conftest.py
+-rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.3/tests/test_deadpool.py
+-rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.3/PKG-INFO
```

### Comparing `deadpool_executor-2023.7.2/LICENSE` & `deadpool_executor-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/README.rst` & `deadpool_executor-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/deadpool.py` & `deadpool_executor-2023.7.3/deadpool.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,43 @@
 from dataclasses import dataclass, field
 from multiprocessing.connection import Connection
 from queue import Empty, PriorityQueue, Queue, SimpleQueue
 from typing import Callable, Optional, Tuple
 
 import psutil
 
-__version__ = "2023.7.2"
+__version__ = "2023.7.3"
 __all__ = [
     "Deadpool",
     "Future",
     "CancelledError",
     "TimeoutError",
     "ProcessError",
     "PoolClosed",
     "as_completed",
 ]
 logger = logging.getLogger("deadpool")
 
 
+# Does not work. Hangs the process on exit.
+# There currently isn't an official way to clean up the
+# resource tracker process. It is an open issue on the
+# Python issue tracker.
+# @atexit.register
+# def stop_resource_tracker():
+#     from multiprocessing import resource_tracker
+#     tracker = resource_tracker._resource_tracker
+#     try:
+#         import time
+#         time.sleep(5)
+#         tracker._stop()
+#     except Exception:
+#         logger.info("Error stopping the multiprocessing resource tracker")
+
+
 @dataclass(order=True)
 class PrioritizedItem:
     priority: int
     item: typing.Any = field(compare=False)
 
 
 @dataclass(init=False)
@@ -313,30 +329,31 @@
             wp.shutdown(wait=False)
             return
 
         if not wp.is_alive():
             self.add_worker_to_pool()
             return
 
+        if not wp.ok:
+            self.add_worker_to_pool()
+            return
+
         if self.max_tasks_per_child is not None:
             if wp.tasks_ran_counter >= self.max_tasks_per_child:
+                logger.debug(f"Worker {wp.pid} hit max tasks per child.")
                 wp.shutdown(wait=False)
                 self.add_worker_to_pool()
                 return
 
         if self.max_worker_memory_bytes is not None:
             if wp.get_rss_bytes() >= self.max_worker_memory_bytes:
                 wp.shutdown(wait=False)
                 self.add_worker_to_pool()
                 return
 
-        if not wp.ok:
-            self.add_worker_to_pool()
-            return
-
         self.workers.put(wp)
 
     def run_task(self, fn, args, kwargs, timeout, fut: Future):
         try:
             worker: WorkerProcess = self.get_process()
             worker.submit_job((fn, args, kwargs, timeout))
             fut.pid = worker.pid
@@ -366,15 +383,15 @@
                             worker.ok = False
                     finally:
                         break
                 elif not worker.is_alive():
                     logger.debug(f"p is no longer alive: {worker.process}")
                     try:
                         signame = signal.strsignal(-worker.process.exitcode)
-                    except ValueError:  # pragma: no cover
+                    except (ValueError, TypeError):  # pragma: no cover
                         signame = "Unknown"
 
                     if not fut.done():
                         # It is possible that fut has already had a result set on
                         # it. If that's the case we'll do nothing. Otherwise, put
                         # an exception reporting the unexpected situation.
                         msg = (
@@ -527,30 +544,58 @@
     parent_pid,
     initializer,
     initargs,
     finitializer: Optional[Callable] = None,
     finitargs: Optional[Tuple] = None,
     mem_clear_threshold_bytes: Optional[int] = None,
 ):
+    # This event is used to signal that the "parent"
+    # monitor thread should be deactivated.
+    evt = threading.Event()
+
+    def self_destruct_if_parent_disappers():
+        """Poll every 5 seconds to see whether the parent is still
+        alive.
+        """
+        while True:
+            if evt.wait(2.0):
+                return
+
+            if not psutil.pid_exists(parent_pid):
+                logger.warning(f"Parent {parent_pid} is gone, self-destructing.")
+                evt.set()
+                kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
+                return
+
+    tparent = threading.Thread(target=self_destruct_if_parent_disappers, daemon=True)
+    tparent.start()
+
+    def deactivate_parentless_self_destruct():
+        evt.set()
+
     proc = psutil.Process()
     pid = proc.pid
     lock = threading.Lock()
 
     def conn_send_safe(obj):
         try:
+            # TODO: this may not be necessary
             with lock:
                 conn.send(obj)
         except BrokenPipeError:  # pragma: no cover
             logger.debug("Pipe not usable")
         except BaseException:
             logger.exception("Unexpected pipe error")
 
     def timed_out():
+        """Action to fire when the timeout given to ``threading.Timer``
+        is reached. It kills this process with SIGKILL."""
         # First things first. Set a self-destruct timer for ourselves.
         # If we don't finish up in time, boom.
+        deactivate_parentless_self_destruct()
         conn_send_safe(TimeoutError(f"Process {pid} timed out, self-destructing."))
         # kill_proc_tree_in_process_daemon(pid, signal.SIGKILL)
         kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
 
     if initializer:
         initargs = initargs or ()
         try:
@@ -561,14 +606,20 @@
     while True:
         # Wait for some work.
         try:
             job = conn_receiver.recv()
         except EOFError:
             logger.debug("Received EOF, exiting.")
             break
+        except KeyboardInterrupt:
+            logger.debug("Received KeyboardInterrupt, exiting.")
+            break
+        except BaseException:
+            logger.exception("Received unexpected exception, exiting.")
+            break
 
         if job is None:
             logger.debug("Received None, exiting.")
             break
 
         # Real work, unpack.
         fn, args, kwargs, timeout = job
@@ -576,39 +627,14 @@
         if timeout:
             t = threading.Timer(timeout, timed_out)
             t.start()
             deactivate_timer = lambda: t.cancel()  # noqa: E731
         else:
             deactivate_timer = lambda: None  # noqa: E731
 
-        evt = threading.Event()
-
-        def self_destruct_if_parent_disappers():
-            """Poll every 5 seconds to see whether the parent is still
-            alive.
-            """
-            while True:
-                if evt.wait(2.0):
-                    return
-
-                if not psutil.pid_exists(parent_pid):
-                    logger.warning(f"Parent {parent_pid} is gone, self-destructing.")
-                    evt.set()
-                    # kill_proc_tree_in_process_daemon(pid, signal.SIGKILL)
-                    kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
-                    return
-
-        tparent = threading.Thread(
-            target=self_destruct_if_parent_disappers, daemon=True
-        )
-        tparent.start()
-
-        def deactivate_parentless_self_destruct():
-            evt.set()
-
         try:
             results = fn(*args, **kwargs)
         except BaseException as e:
             # Check whether the exception can be pickled. If not we're going
             # to wrap it. Why do this? It turns out that mp.Connection.send
             # will try to pickle the exception, and if it can't, it will
             # lose its mind. I've gotten segfaults in Python with this.
@@ -624,28 +650,40 @@
                 )
                 e = ProcessError(msg)
             conn_send_safe(e)
         else:
             conn_send_safe(results)
         finally:
             deactivate_timer()
-            deactivate_parentless_self_destruct()
 
             if mem_clear_threshold_bytes is not None:
                 mem = proc.memory_info().rss
                 if mem > mem_clear_threshold_bytes:
                     trim_memory()
 
     if finitializer:
         finitargs = finitargs or ()
         try:
             finitializer(*finitargs)
         except BaseException:
             logger.exception("finitializer failed")
 
+    # We've reached the end of this function which means this
+    # process must exit. However, we started a couple threads
+    # in here and they don't magically exit. Additional
+    # synchronization controls are needed to tell the threads
+    # to exit, which we don't have. However, we do have a kill
+    # switch. Since this process worker will process no more
+    # work, and since we've already fun the finalizer, we may
+    # as well just nuke it. That will remove its memory space
+    # and all its threads too.
+    deactivate_parentless_self_destruct()
+    logger.debug(f"Nuking worker {pid=}")
+    kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
+
 
 def kill_proc_tree_in_process_daemon(pid, sig):  # pragma: no cover
     mp.Process(target=kill_proc_tree, args=(pid, sig), daemon=True).start()
 
 
 # Taken from
 # https://psutil.readthedocs.io/en/latest/index.html?highlight=children#kill-process-tree
```

### Comparing `deadpool_executor-2023.7.2/examples/entrypoint.py` & `deadpool_executor-2023.7.3/examples/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/examples/priorities.py` & `deadpool_executor-2023.7.3/examples/priorities.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/noxfile.py` & `deadpool_executor-2023.7.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/pyproject.toml` & `deadpool_executor-2023.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/tests/test_deadpool.py` & `deadpool_executor-2023.7.3/tests/test_deadpool.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.2/PKG-INFO` & `deadpool_executor-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

