# Comparing `tmp/arq-django-admin-0.3.0.tar.gz` & `tmp/arq-django-admin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arq-django-admin-0.3.0.tar", last modified: Thu Jun 29 11:44:17 2023, max compression
+gzip compressed data, was "arq-django-admin-0.3.1.tar", last modified: Tue Jul 11 10:21:22 2023, max compression
```

## Comparing `arq-django-admin-0.3.0.tar` & `arq-django-admin-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_abort.html
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/jobs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/queues.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_django_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-29 11:44:17.114884 arq-django-admin-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.608548 arq-django-admin-0.3.1/arq_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_abort.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/queues.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_django_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/setup.py
```

### Comparing `arq-django-admin-0.3.0/LICENSE` & `arq-django-admin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/PKG-INFO` & `arq-django-admin-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.3.0
+Version: 0.3.1
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.3.0/README.md` & `arq-django-admin-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/job.py` & `arq-django-admin-0.3.1/arq_admin/job.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/queue.py` & `arq-django-admin-0.3.1/arq_admin/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
+import re
 from contextlib import suppress
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional
 
 from arq import ArqRedis
 from arq.connections import RedisSettings, create_pool
 from arq.jobs import DeserializationError, Job as ArqJob, JobDef, JobStatus
 from arq.utils import timestamp_ms
 from django.utils import timezone
 
 from arq_admin import settings
 from arq_admin.job import JobInfo
 
 ARQ_PREFIX = 'arq:'
+ARQ_KEY_REGEX = re.compile(r'arq\:(?P<prefix>.+?)\:(?P<job_id>.+)')
 PREFIX_PRIORITY = {prefix: i for i, prefix in enumerate(['job', 'in-progress', 'result'])}
 
 
 @dataclass
 class QueueStats:
     name: str
     host: str
@@ -149,24 +151,24 @@
             return self._cached_job_id_to_status_map
 
         async with self._redis.pipeline(transaction=True) as pipe:
             await pipe.keys(f'{ARQ_PREFIX}*:*')
             await pipe.zrange(self.name, withscores=True, start=0, end=-1)
             all_arq_keys, job_ids_with_scores = await pipe.execute()
 
-        # iter over lists of type [job_id, prefix];
-        # can't use dict here because we can have multiple keys for one job and need to use the more specific one
-        job_ids_with_prefixes = (
-            key.decode('utf-8')[len(ARQ_PREFIX):].split(':')[::-1] for key in all_arq_keys
-        )
+        regex_matches_from_arq_keys = (ARQ_KEY_REGEX.match(key.decode('utf-8')) for key in all_arq_keys)
+        # iter over dicts with job ids and their keys' prefixes
+        # can't create mapping from ids to prefixes right away here
+        # because we can have multiple keys with different prefixes for one job and need to use the more specific one
+        job_ids_with_prefixes = (match.groupdict() for match in regex_matches_from_arq_keys if match is not None)
 
         job_ids_to_scores = {key[0].decode('utf-8'): key[1] for key in job_ids_with_scores}
         job_ids_to_prefixes = dict(sorted(
             # not only ensure that we don't get key error but also filter out stuff that's not a client job
-            ([job_id, prefix] for job_id, prefix in job_ids_with_prefixes if prefix in PREFIX_PRIORITY),
+            ([key['job_id'], key['prefix']] for key in job_ids_with_prefixes if key['prefix'] in PREFIX_PRIORITY),
             # make sure that more specific indices go after less specific ones
             key=lambda job_id_with_prefix: PREFIX_PRIORITY[job_id_with_prefix[-1]],
         ))
 
         self._cached_job_id_to_status_map = {
             job_id: self._get_job_status_from_raw_data(prefix, job_ids_to_scores.get(job_id))
             for job_id, prefix in job_ids_to_prefixes.items()
```

### Comparing `arq-django-admin-0.3.0/arq_admin/settings.py` & `arq-django-admin-0.3.1/arq_admin/settings.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_abort.html` & `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_abort.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_detail.html` & `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_detail.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/jobs.html` & `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/jobs.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/queues.html` & `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/queues.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/urls.py` & `arq-django-admin-0.3.1/arq_admin/urls.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_admin/views.py` & `arq-django-admin-0.3.1/arq_admin/views.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/arq_django_admin.egg-info/PKG-INFO` & `arq-django-admin-0.3.1/arq_django_admin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.3.0
+Version: 0.3.1
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.3.0/arq_django_admin.egg-info/SOURCES.txt` & `arq-django-admin-0.3.1/arq_django_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/setup.cfg` & `arq-django-admin-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.0/setup.py` & `arq-django-admin-0.3.1/setup.py`

 * *Files identical despite different names*

