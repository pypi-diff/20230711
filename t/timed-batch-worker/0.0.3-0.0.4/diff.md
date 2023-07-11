# Comparing `tmp/timed-batch-worker-0.0.3.tar.gz` & `tmp/timed-batch-worker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/brams/dev/abrams/timed-batch-worker/dist/tmpnobgwaes/timed-batch-worker-0.0.3.tar", last modified: Tue Sep  6 13:16:37 2022, max compression
+gzip compressed data, was "timed-batch-worker-0.0.4.tar", last modified: Tue Jul 11 21:07:54 2023, max compression
```

## Comparing `timed-batch-worker-0.0.3.tar` & `timed-batch-worker-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brams      (501) staff       (20)        0 2022-09-06 13:16:37.448744 timed-batch-worker-0.0.3/
--rw-r--r--   0 brams      (501) staff       (20)     1069 2022-09-06 10:23:28.000000 timed-batch-worker-0.0.3/LICENSE
--rw-r--r--   0 brams      (501) staff       (20)     1572 2022-09-06 13:16:37.448396 timed-batch-worker-0.0.3/PKG-INFO
--rw-r--r--   0 brams      (501) staff       (20)      995 2022-09-06 10:27:04.000000 timed-batch-worker-0.0.3/README.md
--rw-r--r--   0 brams      (501) staff       (20)       97 2022-09-06 13:05:11.000000 timed-batch-worker-0.0.3/pyproject.toml
--rw-r--r--   0 brams      (501) staff       (20)       38 2022-09-06 13:16:37.448860 timed-batch-worker-0.0.3/setup.cfg
--rw-r--r--   0 brams      (501) staff       (20)      933 2022-09-06 13:16:11.000000 timed-batch-worker-0.0.3/setup.py
-drwxr-xr-x   0 brams      (501) staff       (20)        0 2022-09-06 13:16:37.443299 timed-batch-worker-0.0.3/src/
-drwxr-xr-x   0 brams      (501) staff       (20)        0 2022-09-06 13:16:37.446082 timed-batch-worker-0.0.3/src/timed_batch_worker/
--rw-r--r--   0 brams      (501) staff       (20)       22 2022-09-06 13:13:58.000000 timed-batch-worker-0.0.3/src/timed_batch_worker/__init__.py
--rw-r--r--   0 brams      (501) staff       (20)     3976 2022-09-06 12:51:41.000000 timed-batch-worker-0.0.3/src/timed_batch_worker/worker.py
-drwxr-xr-x   0 brams      (501) staff       (20)        0 2022-09-06 13:16:37.447935 timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/
--rw-r--r--   0 brams      (501) staff       (20)     1572 2022-09-06 13:16:37.000000 timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/PKG-INFO
--rw-r--r--   0 brams      (501) staff       (20)      293 2022-09-06 13:16:37.000000 timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/SOURCES.txt
--rw-r--r--   0 brams      (501) staff       (20)        1 2022-09-06 13:16:37.000000 timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/dependency_links.txt
--rw-r--r--   0 brams      (501) staff       (20)       19 2022-09-06 13:16:37.000000 timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/top_level.txt
+drwxr-xr-x   0 brams      (501) staff       (20)        0 2023-07-11 21:07:54.561357 timed-batch-worker-0.0.4/
+-rw-r--r--   0 brams      (501) staff       (20)     1069 2023-07-11 19:25:15.000000 timed-batch-worker-0.0.4/LICENSE
+-rw-r--r--   0 brams      (501) staff       (20)     1821 2023-07-11 21:07:54.561229 timed-batch-worker-0.0.4/PKG-INFO
+-rw-r--r--   0 brams      (501) staff       (20)     1244 2023-07-11 21:06:57.000000 timed-batch-worker-0.0.4/README.md
+-rw-r--r--   0 brams      (501) staff       (20)       97 2023-07-11 19:25:15.000000 timed-batch-worker-0.0.4/pyproject.toml
+-rw-r--r--   0 brams      (501) staff       (20)       38 2023-07-11 21:07:54.561395 timed-batch-worker-0.0.4/setup.cfg
+-rw-r--r--   0 brams      (501) staff       (20)      933 2023-07-11 21:02:55.000000 timed-batch-worker-0.0.4/setup.py
+drwxr-xr-x   0 brams      (501) staff       (20)        0 2023-07-11 21:07:54.559896 timed-batch-worker-0.0.4/src/
+drwxr-xr-x   0 brams      (501) staff       (20)        0 2023-07-11 21:07:54.560607 timed-batch-worker-0.0.4/src/timed_batch_worker/
+-rw-r--r--   0 brams      (501) staff       (20)       22 2023-07-11 21:02:34.000000 timed-batch-worker-0.0.4/src/timed_batch_worker/__init__.py
+-rw-r--r--   0 brams      (501) staff       (20)     5575 2023-07-11 21:00:39.000000 timed-batch-worker-0.0.4/src/timed_batch_worker/worker.py
+drwxr-xr-x   0 brams      (501) staff       (20)        0 2023-07-11 21:07:54.561079 timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/
+-rw-r--r--   0 brams      (501) staff       (20)     1821 2023-07-11 21:07:54.000000 timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/PKG-INFO
+-rw-r--r--   0 brams      (501) staff       (20)      293 2023-07-11 21:07:54.000000 timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 brams      (501) staff       (20)        1 2023-07-11 21:07:54.000000 timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 brams      (501) staff       (20)       19 2023-07-11 21:07:54.000000 timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/top_level.txt
```

### Comparing `timed-batch-worker-0.0.3/LICENSE` & `timed-batch-worker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timed-batch-worker-0.0.3/PKG-INFO` & `timed-batch-worker-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-batch-worker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for efficiently batch-processing workloads asynchronously with batch-size- and time-based flushes.
 Home-page: https://github.com/Minibrams/timed-batch-worker
 Author: Anders Brams
 Author-email: anders@brams.dk
 Keywords: batch,worker,asynchronous,threading,timed
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,20 @@
   flush_batch_size=20,
 )
 
 # Worker started in separate thread to avoid throttling main event loop
 # in case the batch handler includes synchronous workloads.
 worker.start()
 
+# The worker can be stopped by calling stop(), but
+# it's important to note that only the flushing and batch-size-checking
+# workers stop immediately. The worker checking for the flush interval
+# will stop at the next flush interval.
+worker.stop()
+
 
 # Add objects to the current batch at any time
 @app.get('/users/create')
 def create_user():
   ...
 
   # Hand off an object to the worker
```

### Comparing `timed-batch-worker-0.0.3/README.md` & `timed-batch-worker-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,20 @@
   flush_batch_size=20,
 )
 
 # Worker started in separate thread to avoid throttling main event loop
 # in case the batch handler includes synchronous workloads.
 worker.start()
 
+# The worker can be stopped by calling stop(), but
+# it's important to note that only the flushing and batch-size-checking
+# workers stop immediately. The worker checking for the flush interval
+# will stop at the next flush interval.
+worker.stop()
+
 
 # Add objects to the current batch at any time
 @app.get('/users/create')
 def create_user():
   ...
 
   # Hand off an object to the worker
```

### Comparing `timed-batch-worker-0.0.3/setup.py` & `timed-batch-worker-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name="timed-batch-worker",
-    version="0.0.3",
+    version="0.0.4",
     author="Anders Brams",
     author_email="anders@brams.dk",
     description="Python library for efficiently batch-processing workloads asynchronously with batch-size- and time-based flushes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "batch",
```

### Comparing `timed-batch-worker-0.0.3/src/timed_batch_worker/worker.py` & `timed-batch-worker-0.0.4/src/timed_batch_worker/worker.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # flush the batch when either 
 # 1) the "batch is full" event fires, or 
 # 2) the "5 seconds have passed" event fires
 # ... without having to spend CPU on constant polling for either.
 #
 # Credit @ SO/Claudiu
 
+class InterruptableEvent(Event):
+    is_interrupted = False
+
 def or_set(self):
     self._set()
     self.changed()
 
 
 def or_clear(self):
     self._clear()
@@ -27,20 +30,29 @@
     e._set = e.set
     e._clear = e.clear
     e.changed = changed_callback
     e.set = lambda: or_set(e)
     e.clear = lambda: or_clear(e)
 
 
-def any_event(*events):
-    or_event = Event()
+def any_event(*events: InterruptableEvent):
+    or_event = InterruptableEvent()
 
     def changed():
-        bools = [e.is_set() for e in events]
-        if any(bools):
+        found_set_event = False
+        for e in events:
+            if e.is_set():
+                found_set_event = True
+
+                if e.is_interrupted:
+                    or_event.is_interrupted = True
+
+                break
+
+        if found_set_event:
             or_event.set()
         else:
             or_event.clear()
 
     for e in events:
         anyfy(e, changed)
 
@@ -68,38 +80,51 @@
         self.is_running = False
 
         self._queue = Queue()
         self._handler = handler
         self._flush_interval = flush_interval
         self._flush_batch_size = flush_batch_size
         self._item_enqueued_event = None
+        self._flush_timeout_event = None
+        self._flush_full_batch_event = None
 
         self._timed_worker_thread = None
         self._batch_worker_thread = None
         self._flush_worker_thread = None
 
-    def _timed_worker(self, flush_event: Event):
+    def _timed_worker(self, flush_event: InterruptableEvent, parent_worker: 'TimedBatchWorker'):
         while True:
             sleep(self._flush_interval)
+
+            if not parent_worker.is_running:
+                return
+
             flush_event.set()
 
-    def _batch_worker(self, log_created_event: Event, flush_event: Event):
+    def _batch_worker(self, log_created_event: InterruptableEvent, flush_event: InterruptableEvent):
         while True:
             log_created_event.wait()
+
+            if log_created_event.is_interrupted:
+                return
+
             if self._queue.unfinished_tasks > self._flush_batch_size:
                 flush_event.set()
 
             log_created_event.clear()
 
-    def _flush_worker(self, do_flush_event: Event):
+    def _flush_worker(self, do_flush_event: InterruptableEvent):
         batch = []
 
         while True:
             do_flush_event.wait()
 
+            if do_flush_event.is_interrupted:
+                return
+
             while not self._queue.empty():
                 batch.append(self._queue.get())
                 self._queue.task_done()
 
             try:
                 self._handler(batch)
             except Exception as e:
@@ -107,33 +132,65 @@
                     f'TimedBatchWorker encountered an error while calling handler: {e}'
                 )
 
             batch = []
             do_flush_event.clear()
 
     def start(self):
-        self._item_enqueued_event = Event()
-
-        flush_timeout_event = Event()
-        flush_full_batch_event = Event()
+        self._item_enqueued_event = InterruptableEvent()
+        self._flush_timeout_event = InterruptableEvent()
+        self._flush_full_batch_event = InterruptableEvent()
 
         do_flush_event = any_event(
-            flush_timeout_event,
-            flush_full_batch_event
+            self._flush_timeout_event,
+            self._flush_full_batch_event
         )
 
-        self._batch_worker_thread = Thread(target=self._batch_worker, args=(
-            self._item_enqueued_event, flush_full_batch_event,), daemon=True)
-        self._timed_worker_thread = Thread(target=self._timed_worker, args=(
-            flush_timeout_event,), daemon=True)
-        self._flush_worker_thread = Thread(target=self._flush_worker, args=(
-            do_flush_event,), daemon=True)
+        self._batch_worker_thread = Thread(
+            target=self._batch_worker, 
+            args=(self._item_enqueued_event, self._flush_full_batch_event,), 
+            daemon=True
+        )
+
+        self._timed_worker_thread = Thread(
+            target=self._timed_worker, 
+            args=(self._flush_timeout_event, self),
+            daemon=True
+        )
+
+        self._flush_worker_thread = Thread(
+            target=self._flush_worker, 
+            args=(do_flush_event,),
+            daemon=True
+        )
 
         self._timed_worker_thread.start()
         self._batch_worker_thread.start()
         self._flush_worker_thread.start()
 
         self.is_running = True
 
     def enqueue(self, item):
+        if not self.is_running:
+            return
+
         self._queue.put(item)
         self._item_enqueued_event.set()
+
+    def stop(self):
+        """
+        Stops flush and bash worker threads immediately.
+        The timed worker thread will stop after the next flush interval.
+        """
+        self.is_running = False
+        self._item_enqueued_event.is_interrupted = True
+        self._flush_timeout_event.is_interrupted = True
+        self._flush_full_batch_event.is_interrupted = True
+
+        # Set all events to force the worker threads to exit
+        self._item_enqueued_event.set()
+        self._flush_timeout_event.set()
+        self._flush_full_batch_event.set()
+
+        self._timed_worker_thread.join()
+        self._batch_worker_thread.join()
+        self._flush_worker_thread.join()
```

### Comparing `timed-batch-worker-0.0.3/src/timed_batch_worker.egg-info/PKG-INFO` & `timed-batch-worker-0.0.4/src/timed_batch_worker.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-batch-worker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for efficiently batch-processing workloads asynchronously with batch-size- and time-based flushes.
 Home-page: https://github.com/Minibrams/timed-batch-worker
 Author: Anders Brams
 Author-email: anders@brams.dk
 Keywords: batch,worker,asynchronous,threading,timed
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,20 @@
   flush_batch_size=20,
 )
 
 # Worker started in separate thread to avoid throttling main event loop
 # in case the batch handler includes synchronous workloads.
 worker.start()
 
+# The worker can be stopped by calling stop(), but
+# it's important to note that only the flushing and batch-size-checking
+# workers stop immediately. The worker checking for the flush interval
+# will stop at the next flush interval.
+worker.stop()
+
 
 # Add objects to the current batch at any time
 @app.get('/users/create')
 def create_user():
   ...
 
   # Hand off an object to the worker
```

