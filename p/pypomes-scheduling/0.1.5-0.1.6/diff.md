# Comparing `tmp/pypomes_scheduling-0.1.5.tar.gz` & `tmp/pypomes_scheduling-0.1.6.tar.gz`

## Comparing `pypomes_scheduling-0.1.5.tar` & `pypomes_scheduling-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.6/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.5/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.1.6/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
-from pypomes_core.env_pomes import APP_PREFIX, env_get_str, env_get_int
-from pypomes_core.exception_pomes import exc_format
+from pypomes_core import exc_format
 from typing import Final
 import logging
 import pytz
 import re
 import sys
 from .threaded_scheduler import __ThreadedScheduler
 
@@ -36,39 +35,39 @@
     except Exception as e:
         errors.append(f"Error creating the job scheduler: {exc_format(e, sys.exc_info())}")
 
     return result
 
 
 def scheduler_schedule(errors: list[str],
-                       jobs: list[tuple[callable, str, str, tuple, str]], start: datetime) -> int:
+                       jobs: list[tuple[callable, str, str, str, datetime, tuple, dict]]) -> int:
     """
-    Schedule the jobs in *jobs*, starting at the given *start*. Each element in the job list is a *tuple* with
-    the corresponding job data: *(callable function, job id, job name, job arguments, CRON expression)*.
+    Schedule the jobs in *jobs*, starting at the given *start*. Each element in the job list
+    is a *tuple* with the corresponding job data:
+    *(callable function, job id, job name, CRON expression, job start timestamp, job args, job kwargs)*.
 
     :param errors: Resulting errors, if any
     :param jobs: List of tuples with jobs to schedule
-    :param start: Optional start timestamp for the scheduler
     :return: The number of jobs effectively scheduled
     """
     global __scheduler
     # inicializa a variável de retorno
     result: int = 0
 
     # traverse the job list and do the scheduling
     for job in jobs:
 
         # is it a valid CRON expression ?
-        if re.search(__REGEX_VERIFY_CRON, job[4]) is None:
+        if re.search(__REGEX_VERIFY_CRON, job[3]) is None:
             # no, report the error
             errors.append(f"Invalid CRON expression: '{job[4]}'")
         else:
             # yes, proceed with the scheduling
             try:
-                __scheduler.schedule_job(job[0], job[1], job[2], job[4], job[3], start)
+                __scheduler.schedule_job(job[0], job[1], job[2], job[3], job[4], job[5], job[6])
                 result += 1
             except Exception as e:
                 errors.append(f"Error scheduling the job '{job[2]}', id '{job[1]}', "
                               f"with CRON '{job[3]}': {exc_format(e, sys.exc_info())}")
 
     return result
```

### Comparing `pypomes_scheduling-0.1.5/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.6/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.5/LICENSE` & `pypomes_scheduling-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.5/pyproject.toml` & `pypomes_scheduling-0.1.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.5/PKG-INFO` & `pypomes_scheduling-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

