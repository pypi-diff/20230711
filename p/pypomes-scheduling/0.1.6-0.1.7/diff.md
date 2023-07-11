# Comparing `tmp/pypomes_scheduling-0.1.6.tar.gz` & `tmp/pypomes_scheduling-0.1.7.tar.gz`

## Comparing `pypomes_scheduling-0.1.6.tar` & `pypomes_scheduling-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.6/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.7/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,63 +33,67 @@
         Start the scheduler in itas own thread.
         """
         # stay in loop until 'stop()' is invoked
         while not self._stopped:
             if self._logger is not None:
                 self._logger.info("Started")
 
-            # start the scheduler, blocking until it is interrupted
+            # start the scheduler, blocking the thread until it is interrupted
             self._scheduler.start()
 
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
-    def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str,
+    def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str = None,
                      job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None):
         """
         Schedule the given *job*, with the parameters
         :param job: the callable object to be scheduled
         :param job_id: the id of the scheduled job
         :param job_name: the name of the scheduled job
         :param job_cron: the CRON expression directing the execution times
         :param job_start: the start timestamp for the scheduling process
         :param job_args: the '*args' arguments to be passed to the scheduled job
         :param job_kwargs: the '**kwargs' arguments to be passed to the scheduled job
-        :return:
         """
         # approximately, convert symbols to CRON expression
-        expr: str
+        cron_expr: str | None
         match job_cron:
             case "@reboot":
-                expr = "1 0 * * *"                      # daily, at 00h01
+                cron_expr = "1 0 * * *"                      # daily, at 00h01
             case "@midnight":
-                expr = "0 0 * * *"                      # daily, at 00h00
+                cron_expr = "0 0 * * *"                      # daily, at 00h00
             case "@hourly":
-                expr = "0 * * * *"                      # every hour, at minute 0 (??h00)
+                cron_expr = "0 * * * *"                      # every hour, at minute 0 (??h00)
             case "@daily":
-                expr = "1 0 * * *"                      # daily, at 00h01
+                cron_expr = "1 0 * * *"                      # daily, at 00h01
             case "@weekly":
-                expr = "0 0 * * 0"                      # on sundays, at 00h00
+                cron_expr = "0 0 * * 0"                      # on sundays, at 00h00
             case "@monthly":
-                expr = "0 0 1 * *"                      # on the first day of the month, at 00h00
+                cron_expr = "0 0 1 * *"                      # on the first day of the month, at 00h00
             case "@yearly" | "@annually":
-                expr = "0 0 1 1 *"                      # on January 1st, at 00h00
+                cron_expr = "0 0 1 1 *"                      # on January 1st, at 00h00
+            case None:
+                cron_expr = None
             case _:
-                expr = job_cron
+                cron_expr = job_cron
 
-        # CRON expression: <minute> <hour> <day-of-month> <month> <day-of-week>
-        vals: list[str] = expr.split()
-        vals = [None if val == '?' else val for val in vals]
-        aps_trigger = CronTrigger(minute=vals[0],
-                                  hour=vals[1],
-                                  day=vals[2],
-                                  month=vals[3],
-                                  day_of_week=vals[4],
-                                  start_date=job_start)
+        aps_trigger: CronTrigger | None = None
+        # has the CRON expression been defined ?
+        if cron_expr is not None:
+            # yes, build the trigger: <minute> <hour> <day-of-month> <month> <day-of-week>
+            vals: list[str] = cron_expr.split()
+            vals = [None if val == '?' else val for val in vals]
+            aps_trigger = CronTrigger(minute=vals[0],
+                                      hour=vals[1],
+                                      day=vals[2],
+                                      month=vals[3],
+                                      day_of_week=vals[4],
+                                      start_date=job_start)
         self._scheduler.add_job(func=job,
                                 trigger=aps_trigger,
                                 args=job_args,
                                 kwargs=job_kwargs,
                                 id=job_id,
                                 name=job_name)
         if self._logger is not None:
```

### Comparing `pypomes_scheduling-0.1.6/LICENSE` & `pypomes_scheduling-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.6/pyproject.toml` & `pypomes_scheduling-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.6/PKG-INFO` & `pypomes_scheduling-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

