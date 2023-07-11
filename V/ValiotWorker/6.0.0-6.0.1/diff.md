# Comparing `tmp/ValiotWorker-6.0.0.tar.gz` & `tmp/ValiotWorker-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValiotWorker-6.0.0.tar", last modified: Thu Jun 29 22:45:13 2023, max compression
+gzip compressed data, was "ValiotWorker-6.0.1.tar", last modified: Tue Jul 11 21:34:59 2023, max compression
```

## Comparing `ValiotWorker-6.0.0.tar` & `ValiotWorker-6.0.1.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.611581 ValiotWorker-6.0.0/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-6.0.0/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-6.0.0/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-29 22:45:13.611381 ValiotWorker-6.0.0/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-6.0.0/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.607956 ValiotWorker-6.0.0/ValiotWorker/
--rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-6.0.0/ValiotWorker/Logging.py
--rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-6.0.0/ValiotWorker/Notifications.py
--rw-r--r--   0 baruc      (501) staff       (20)      294 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-06-29 18:09:35.000000 ValiotWorker-6.0.0/ValiotWorker/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/__version__.py
--rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-6.0.0/ValiotWorker/croniterHelpers.py
--rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-6.0.0/ValiotWorker/dateHelpers.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.609938 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/
--rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__main__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.610646 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/
--rw-r--r--   0 baruc      (501) staff       (20)        0 2023-06-16 19:03:59.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/http_server.py
--rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/mutations.py
--rw-r--r--   0 baruc      (501) staff       (20)     4393 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/queries.py
--rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/redis.py
--rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/subscriptions.py
--rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-6.0.0/ValiotWorker/uploaders.py
--rw-r--r--   0 baruc      (501) staff       (20)    70027 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/worker.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.609433 ValiotWorker-6.0.0/ValiotWorker.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      841 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       60 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)      233 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)       13 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-06-29 22:45:13.611650 ValiotWorker-6.0.0/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     2607 2023-06-16 19:03:59.000000 ValiotWorker-6.0.0/setup.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.611007 ValiotWorker-6.0.0/tests/
--rw-r--r--   0 baruc      (501) staff       (20)      106 2023-06-29 18:09:35.000000 ValiotWorker-6.0.0/tests/test_dummy.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-07-11 21:34:59.896316 ValiotWorker-6.0.1/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-6.0.1/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       37 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-07-11 21:34:59.896167 ValiotWorker-6.0.1/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-6.0.1/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-07-11 21:34:59.893524 ValiotWorker-6.0.1/ValiotWorker/
+-rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/Logging.py
+-rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-6.0.1/ValiotWorker/Notifications.py
+-rw-r--r--   0 baruc      (501) staff       (20)      294 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     3449 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-07-11 21:32:40.000000 ValiotWorker-6.0.1/ValiotWorker/__version__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      276 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/croniterHelpers.py
+-rw-r--r--   0 baruc      (501) staff       (20)      184 2023-07-11 21:32:40.000000 ValiotWorker-6.0.1/ValiotWorker/dateHelpers.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-07-11 21:34:59.895529 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/
+-rw-r--r--   0 baruc      (501) staff       (20)       41 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      963 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/__main__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-07-11 21:34:59.895922 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/modules/
+-rw-r--r--   0 baruc      (501) staff       (20)        0 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/modules/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/modules/http_server.py
+-rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/mutations.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4393 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/queries.py
+-rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/redis.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-07-11 17:01:47.000000 ValiotWorker-6.0.1/ValiotWorker/subscriptions.py
+-rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-6.0.1/ValiotWorker/uploaders.py
+-rw-r--r--   0 baruc      (501) staff       (20)    70027 2023-07-11 17:02:49.000000 ValiotWorker-6.0.1/ValiotWorker/worker.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-07-11 21:34:59.895282 ValiotWorker-6.0.1/ValiotWorker.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      821 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       60 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)      217 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       13 2023-07-11 21:34:59.000000 ValiotWorker-6.0.1/ValiotWorker.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-07-11 21:34:59.896353 ValiotWorker-6.0.1/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     2536 2023-07-11 21:32:40.000000 ValiotWorker-6.0.1/setup.py
```

### Comparing `ValiotWorker-6.0.0/LICENCE` & `ValiotWorker-6.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/PKG-INFO` & `ValiotWorker-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 6.0.0
+Version: 6.0.1
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-6.0.0/README.md` & `ValiotWorker-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/Logging.py` & `ValiotWorker-6.0.1/ValiotWorker/Logging.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/Notifications.py` & `ValiotWorker-6.0.1/ValiotWorker/Notifications.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/__main__.py` & `ValiotWorker-6.0.1/ValiotWorker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 @vw.job(
     name='TEST_JOB',
     alias='test job 1',
     description='',
     schedule='* * * * *',
     enabled=True,
-    queueType=QueueType.FREQUENCY,
+    queueType=QueueType.ON_DEMAND
 )
 def test_job(log, **_):
     log(LogLevel.INFO, "Hi, I'm test job #1")
     time.sleep(0.2)
     log(LogLevel.INFO, "Hi, I'm test job #1 again")
     return {'result': 'ok 1'}
 
@@ -123,12 +123,12 @@
 # def missing_job(log, **_):
 #     log(LogLevel.ERROR, "Hi, I should not be called, please comment me")
 #     return 'ok simple output'
 
 
 def main():
     print('main for valiot worker')
-    vw.run(interval=5.0)
+    vw.run(interval=1.0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__main__.py` & `ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/http_server.py` & `ValiotWorker-6.0.1/ValiotWorker/healthCheckProbe/modules/http_server.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/mutations.py` & `ValiotWorker-6.0.1/ValiotWorker/mutations.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/queries.py` & `ValiotWorker-6.0.1/ValiotWorker/queries.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/redis.py` & `ValiotWorker-6.0.1/ValiotWorker/redis.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/subscriptions.py` & `ValiotWorker-6.0.1/ValiotWorker/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker/worker.py` & `ValiotWorker-6.0.1/ValiotWorker/worker.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-6.0.0/ValiotWorker.egg-info/PKG-INFO` & `ValiotWorker-6.0.1/ValiotWorker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 6.0.0
+Version: 6.0.1
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-6.0.0/ValiotWorker.egg-info/SOURCES.txt` & `ValiotWorker-6.0.1/ValiotWorker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 ValiotWorker.egg-info/entry_points.txt
 ValiotWorker.egg-info/not-zip-safe
 ValiotWorker.egg-info/requires.txt
 ValiotWorker.egg-info/top_level.txt
 ValiotWorker/healthCheckProbe/__init__.py
 ValiotWorker/healthCheckProbe/__main__.py
 ValiotWorker/healthCheckProbe/modules/__init__.py
-ValiotWorker/healthCheckProbe/modules/http_server.py
-tests/test_dummy.py
+ValiotWorker/healthCheckProbe/modules/http_server.py
```

### Comparing `ValiotWorker-6.0.0/setup.py` & `ValiotWorker-6.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     'croniter>=1.3, <2.0',
     'pydash>=5.0, <7.0',  # Must be aligned with the version at gstorm
     'pygqlc>=3.0, <4.0',  # Must be aligned with the version at gstorm
     'python-dateutil>=2.8, <3.0',  # Must be aligned with the version at gstorm
     'pytz>=2022.2, <2022.8',  # Must be aligned with the version at gstorm
     'redis>=4.3, <5.0',
     'singleton-decorator>=1.0, <2.0',
-    'termcolor>=2.0, <3.0',  # Must be aligned with the version at gstorm
-    'tzlocal>=4.2, <5.0',  # Must be aligned with the version at gstorm
+    'termcolor>=2.0.1, <3.0', # Must be aligned with the version at gstorm
     'velebit-useful-logs>=1.0, <2.0'
 ]
 
 setup_requirements = [
     # TODO(alanbato): put setup requirements (distutils extensions, etc.) here
     'twine',
 ]
```

