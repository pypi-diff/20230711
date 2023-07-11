# Comparing `tmp/pypomes_scheduling-0.1.2.tar.gz` & `tmp/pypomes_scheduling-0.1.3.tar.gz`

## Comparing `pypomes_scheduling-0.1.2.tar` & `pypomes_scheduling-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.3/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.2/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.1.3/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,40 +35,40 @@
         result = True
     except Exception as e:
         errors.append(f"Error creating the job scheduler: {exc_format(e, sys.exc_info())}")
 
     return result
 
 
-# jobs: callable function, job id, job name, CRON expression
-def scheduler_schedule(errors: list[str], jobs: list[tuple[callable, str, str, str]], start: datetime) -> int:
+def scheduler_schedule(errors: list[str],
+                       jobs: list[tuple[callable, str, str, tuple, str]], start: datetime) -> int:
     """
     Schedule the jobs in *jobs*, starting at the given *start*. Each element in the job list is a *tuple* with
-    the corresponding job data: *(callable function, job id, job name, CRON expression)*.
+    the corresponding job data: *(callable function, job id, job name, job arguments, CRON expression)*.
 
     :param errors: Resulting errors, if any
     :param jobs: List of tuples with jobs to schedule
     :param start: Optional start timestamp for the scheduler
     :return: The number of jobs effectively scheduled
     """
     global __scheduler
     # inicializa a variável de retorno
     result: int = 0
 
     # traverse the job list and do the scheduling
     for job in jobs:
 
         # is it a valid CRON expression ?
-        if re.search(__REGEX_VERIFY_CRON, job[3]) is None:
+        if re.search(__REGEX_VERIFY_CRON, job[4]) is None:
             # no, report the error
-            errors.append(f"Invalid CRON expression: '{job[3]}'")
+            errors.append(f"Invalid CRON expression: '{job[4]}'")
         else:
             # yes, proceed with the scheduling
             try:
-                __scheduler.schedule_job(job[0], job[1], job[2], job[3], start)
+                __scheduler.schedule_job(job[0], job[1], job[2], job[4], job[3], start)
                 result += 1
             except Exception as e:
                 errors.append(f"Error scheduling the job '{job[2]}', id '{job[1]}', "
                               f"with CRON '{job[3]}': {exc_format(e, sys.exc_info())}")
 
     return result
```

### Comparing `pypomes_scheduling-0.1.2/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.3/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from apscheduler.triggers.cron import CronTrigger
 import logging
 import pytz
 import threading
 
 
 class __ThreadedScheduler(threading.Thread):
-
+    """
+    A scalable implementation of *APScheduler*'s *BlockingScheduler*, running as single or multiple instances,
+    each on its own thread.
+    """
     _scheduler: BlockingScheduler
     _logger: logging.Logger
     _stopped: bool
 
     def __init__(self, timezone: pytz.timezone, retry_interval: int, logger: logging.Logger = None):
 
         threading.Thread.__init__(self)
@@ -23,28 +26,28 @@
                                             jobstore_retry_interval=retry_interval)
         if self._logger is not None:
             self._logger.info("Instanced, with timezone "
                               f"'{timezone}' and retry interval '{retry_interval}'")
 
     def run(self):
 
-        # permanece no laço até que 'stop()' seja invocado
+        # stay in loop until 'stop()' is invoked
         while not self._stopped:
             if self._logger is not None:
                 self._logger.info("Started")
 
-            # inicia o agendador, bloqueando até que ele seja interrompido
+            # start the scheduler, blocking until it is interrupted
             self._scheduler.start()
 
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
-    def schedule_job(self, job: callable, job_id: str,
-                     job_name: str, cron_expr: str, start: datetime = None):
+    def schedule_job(self, job: callable, job_id: str, job_name: str,
+                     cron_expr: str, job_args: tuple = None, start: datetime = None):
 
         # approximately, convert symbols to CRON expression
         expr: str
         match cron_expr:
             case "@reboot":
                 expr = "1 0 * * *"                      # daily, at 00h01
             case "@midnight":
@@ -69,14 +72,15 @@
                                   hour=vals[1],
                                   day=vals[2],
                                   month=vals[3],
                                   day_of_week=vals[4],
                                   start_date=start)
         self._scheduler.add_job(func=job,
                                 trigger=aps_trigger,
+                                args=job_args,
                                 id=job_id,
                                 name=job_name)
         if self._logger is not None:
             self._logger.info(f"Job '{job_name}' scheduled, with CRON '{cron_expr}'")
 
     def stop(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_scheduling-0.1.2/LICENSE` & `pypomes_scheduling-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.2/pyproject.toml` & `pypomes_scheduling-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.2/PKG-INFO` & `pypomes_scheduling-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

