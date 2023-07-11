# Comparing `tmp/pypomes_scheduling-0.1.4.tar.gz` & `tmp/pypomes_scheduling-0.1.5.tar.gz`

## Comparing `pypomes_scheduling-0.1.4.tar` & `pypomes_scheduling-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.4/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.1.5/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.4/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.5/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,29 +40,30 @@
             # start the scheduler, blocking until it is interrupted
             self._scheduler.start()
 
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
-    def schedule_job(self, job: callable, job_id: str, job_name: str,
-                     cron_expr: str, job_args: tuple = None, start: datetime = None):
+    def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str,
+                     job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None):
         """
         Schedule the given *job*, with the parameters
         :param job: the callable object to be scheduled
         :param job_id: the id of the scheduled job
         :param job_name: the name of the scheduled job
-        :param cron_expr: the CRON expression directing the execution times
-        :param job_args: the arguments to be passed to the scheduled job
-        :param start: the start timestamp for the scheduling process
+        :param job_cron: the CRON expression directing the execution times
+        :param job_start: the start timestamp for the scheduling process
+        :param job_args: the '*args' arguments to be passed to the scheduled job
+        :param job_kwargs: the '**kwargs' arguments to be passed to the scheduled job
         :return:
         """
         # approximately, convert symbols to CRON expression
         expr: str
-        match cron_expr:
+        match job_cron:
             case "@reboot":
                 expr = "1 0 * * *"                      # daily, at 00h01
             case "@midnight":
                 expr = "0 0 * * *"                      # daily, at 00h00
             case "@hourly":
                 expr = "0 * * * *"                      # every hour, at minute 0 (??h00)
             case "@daily":
@@ -70,32 +71,33 @@
             case "@weekly":
                 expr = "0 0 * * 0"                      # on sundays, at 00h00
             case "@monthly":
                 expr = "0 0 1 * *"                      # on the first day of the month, at 00h00
             case "@yearly" | "@annually":
                 expr = "0 0 1 1 *"                      # on January 1st, at 00h00
             case _:
-                expr = cron_expr
+                expr = job_cron
 
         # CRON expression: <minute> <hour> <day-of-month> <month> <day-of-week>
         vals: list[str] = expr.split()
         vals = [None if val == '?' else val for val in vals]
         aps_trigger = CronTrigger(minute=vals[0],
                                   hour=vals[1],
                                   day=vals[2],
                                   month=vals[3],
                                   day_of_week=vals[4],
-                                  start_date=start)
+                                  start_date=job_start)
         self._scheduler.add_job(func=job,
                                 trigger=aps_trigger,
                                 args=job_args,
+                                kwargs=job_kwargs,
                                 id=job_id,
                                 name=job_name)
         if self._logger is not None:
-            self._logger.info(f"Job '{job_name}' scheduled, with CRON '{cron_expr}'")
+            self._logger.info(f"Job '{job_name}' scheduled, with CRON '{job_cron}'")
 
     def stop(self):
         """
         Stop the scheduler.
         :return:
         """
         if self._logger is not None:
```

### Comparing `pypomes_scheduling-0.1.4/LICENSE` & `pypomes_scheduling-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.4/pyproject.toml` & `pypomes_scheduling-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.4/PKG-INFO` & `pypomes_scheduling-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

