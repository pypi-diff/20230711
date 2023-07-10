# Comparing `tmp/bullmq-1.6.0.tar.gz` & `tmp/bullmq-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.6.0.tar", last modified: Thu Jul  6 19:16:03 2023, max compression
+gzip compressed data, was "bullmq-1.6.1.tar", last modified: Mon Jul 10 23:38:04 2023, max compression
```

## Comparing `bullmq-1.6.0.tar` & `bullmq-1.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.517049 bullmq-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 19:16:03.517049 bullmq-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 19:14:58.000000 bullmq-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.509049 bullmq-1.6.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-06 19:16:01.000000 bullmq-1.6.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.513049 bullmq-1.6.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/updateProgress-2.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.513049 bullmq-1.6.0/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.517049 bullmq-1.6.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.509049 bullmq-1.6.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-06 19:16:01.000000 bullmq-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:16:03.517049 bullmq-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 19:14:58.000000 bullmq-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.380847 bullmq-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 23:38:04.376846 bullmq-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 23:36:30.000000 bullmq-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.368847 bullmq-1.6.1/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-10 23:38:01.000000 bullmq-1.6.1/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/updateProgress-2.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.368847 bullmq-1.6.1/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-10 23:38:01.000000 bullmq-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:04.380847 bullmq-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 23:36:30.000000 bullmq-1.6.1/setup.py
```

### Comparing `bullmq-1.6.0/PKG-INFO` & `bullmq-1.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.6.0
+Version: 1.6.1
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BullMQ For Python
 
 This is the official BullMQ Python library. It is a close port of the NodeJS version of the library.
 Python Queues are interoperable with NodeJS Queues, as both libraries use the same .lua scripts that
@@ -26,23 +25,23 @@
 
 Currently, the library does not support all the features available in the NodeJS version. The following
 have been ported so far:
 
 - [ ] Add jobs to queues.
 
   - [x] Regular jobs.
-  - [ ] Delayed jobs.
+  - [x] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
 - [x] Job progress.
 - [ ] Job retries.
-- [ ] Job backoff.
+- [x] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
 pip install bullmq
 ```
```

### Comparing `bullmq-1.6.0/README.md` & `bullmq-1.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 Currently, the library does not support all the features available in the NodeJS version. The following
 have been ported so far:
 
 - [ ] Add jobs to queues.
 
   - [x] Regular jobs.
-  - [ ] Delayed jobs.
+  - [x] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
 - [x] Job progress.
 - [ ] Job retries.
-- [ ] Job backoff.
+- [x] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
 pip install bullmq
 ```
```

### Comparing `bullmq-1.6.0/bullmq/backoffs.py` & `bullmq-1.6.1/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/addJob-9.lua` & `bullmq-1.6.1/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.6.1/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.6.1/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.6.1/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/drain-4.lua` & `bullmq-1.6.1/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.6.1/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.6.1/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/getState-8.lua` & `bullmq-1.6.1/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.6.1/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.6.1/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.6.1/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.6.1/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.6.1/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.6.1/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.6.1/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.6.1/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.6.1/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/pause-5.lua` & `bullmq-1.6.1/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/promote-7.lua` & `bullmq-1.6.1/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.6.1/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.6.1/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.6.1/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.6.1/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.6.1/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/event_emitter.py` & `bullmq-1.6.1/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/job.py` & `bullmq-1.6.1/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/queue.py` & `bullmq-1.6.1/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/redis_connection.py` & `bullmq-1.6.1/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/scripts.py` & `bullmq-1.6.1/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/timer.py` & `bullmq-1.6.1/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/types/job_options.py` & `bullmq-1.6.1/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/types/worker_options.py` & `bullmq-1.6.1/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/utils.py` & `bullmq-1.6.1/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq/worker.py` & `bullmq-1.6.1/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.6.1/bullmq.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.6.0
+Version: 1.6.1
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BullMQ For Python
 
 This is the official BullMQ Python library. It is a close port of the NodeJS version of the library.
 Python Queues are interoperable with NodeJS Queues, as both libraries use the same .lua scripts that
@@ -26,23 +25,23 @@
 
 Currently, the library does not support all the features available in the NodeJS version. The following
 have been ported so far:
 
 - [ ] Add jobs to queues.
 
   - [x] Regular jobs.
-  - [ ] Delayed jobs.
+  - [x] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
 - [x] Job progress.
 - [ ] Job retries.
-- [ ] Job backoff.
+- [x] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
 pip install bullmq
 ```
```

### Comparing `bullmq-1.6.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.6.1/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.0/pyproject.toml` & `bullmq-1.6.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.6.0"
+version = "1.6.1"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
+requires-python = ">=3.10.0"
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
+    'Programming Language :: Python :: 3.10',
 ]
 keywords = ["python", "bullmq", "queues"]
 dependencies = [
     "redis >= 4.5.0, < 5",
     "msgpack >= 1.0.0, < 2",
     "semver >= 2.13.0, < 3"
 ]
 
 [project.optional-dependencies]
 dev = [
     "setuptools==63.1.0",
     "pre-commit==3.3.3",
     "build==0.8.0",
     "python-semantic-release==7.28.1",
-    "types-redis==4.6.0.1"
+    "types-redis==4.6.0.2"
 ]
 
 [project.urls]
 "Homepage" = "https://bullmq.io"
 "Bug Tracker" = "https://github.com/taskforcesh/bullmq/issues"
 
 [tool.setuptools.packages.find]
```

