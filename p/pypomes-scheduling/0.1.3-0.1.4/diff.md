# Comparing `tmp/pypomes_scheduling-0.1.3.tar.gz` & `tmp/pypomes_scheduling-0.1.4.tar.gz`

## Comparing `pypomes_scheduling-0.1.3.tar` & `pypomes_scheduling-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.3/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.1.4/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.3/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.4/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,30 +25,41 @@
                                             timezone=timezone,
                                             jobstore_retry_interval=retry_interval)
         if self._logger is not None:
             self._logger.info("Instanced, with timezone "
                               f"'{timezone}' and retry interval '{retry_interval}'")
 
     def run(self):
-
+        """
+        Start the scheduler in itas own thread.
+        """
         # stay in loop until 'stop()' is invoked
         while not self._stopped:
             if self._logger is not None:
                 self._logger.info("Started")
 
             # start the scheduler, blocking until it is interrupted
             self._scheduler.start()
 
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
     def schedule_job(self, job: callable, job_id: str, job_name: str,
                      cron_expr: str, job_args: tuple = None, start: datetime = None):
-
+        """
+        Schedule the given *job*, with the parameters
+        :param job: the callable object to be scheduled
+        :param job_id: the id of the scheduled job
+        :param job_name: the name of the scheduled job
+        :param cron_expr: the CRON expression directing the execution times
+        :param job_args: the arguments to be passed to the scheduled job
+        :param start: the start timestamp for the scheduling process
+        :return:
+        """
         # approximately, convert symbols to CRON expression
         expr: str
         match cron_expr:
             case "@reboot":
                 expr = "1 0 * * *"                      # daily, at 00h01
             case "@midnight":
                 expr = "0 0 * * *"                      # daily, at 00h00
@@ -79,11 +90,14 @@
                                 args=job_args,
                                 id=job_id,
                                 name=job_name)
         if self._logger is not None:
             self._logger.info(f"Job '{job_name}' scheduled, with CRON '{cron_expr}'")
 
     def stop(self):
-
+        """
+        Stop the scheduler.
+        :return:
+        """
         if self._logger is not None:
             self._logger.info("Finishing...")
         self._stopped = True
```

### Comparing `pypomes_scheduling-0.1.3/LICENSE` & `pypomes_scheduling-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.3/pyproject.toml` & `pypomes_scheduling-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.3/PKG-INFO` & `pypomes_scheduling-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

