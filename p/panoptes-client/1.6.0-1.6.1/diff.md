# Comparing `tmp/panoptes_client-1.6.0.tar.gz` & `tmp/panoptes_client-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptes_client-1.6.0.tar", last modified: Fri Dec  2 20:12:39 2022, max compression
+gzip compressed data, was "panoptes_client-1.6.1.tar", last modified: Tue Jul 11 18:56:00 2023, max compression
```

## Comparing `panoptes_client-1.6.0.tar` & `panoptes_client-1.6.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/panoptes_client/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/caesar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/collection_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/exportable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/inaturalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    33577 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/panoptes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/project_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/project_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/set_member_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/subject_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/subject_workflow_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/panoptes_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_bearer_expiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_http_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_inaturalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_linkcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_linkresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_set_member_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_subject_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/panoptes_client/workflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/panoptes_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2022-12-02 20:12:39.000000 panoptes_client-1.6.0/panoptes_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2022-12-02 20:12:39.000000 panoptes_client-1.6.0/panoptes_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 20:12:39.000000 panoptes_client-1.6.0/panoptes_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-02 20:12:39.000000 panoptes_client-1.6.0/panoptes_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-02 20:12:39.000000 panoptes_client-1.6.0/panoptes_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 20:12:39.758709 panoptes_client-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-02 20:12:36.000000 panoptes_client-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/panoptes_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/caesar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/collection_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/exportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/inaturalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33577 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/panoptes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/project_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/project_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/set_member_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/subject_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/subject_workflow_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/panoptes_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_bearer_expiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_http_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_inaturalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_linkcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_linkresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_set_member_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_subject_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/panoptes_client/workflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/panoptes_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 18:55:59.000000 panoptes_client-1.6.1/panoptes_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 18:56:00.000000 panoptes_client-1.6.1/panoptes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:55:59.000000 panoptes_client-1.6.1/panoptes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 18:55:59.000000 panoptes_client-1.6.1/panoptes_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 18:55:59.000000 panoptes_client-1.6.1/panoptes_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:56:00.047169 panoptes_client-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 18:55:54.000000 panoptes_client-1.6.1/setup.py
```

### Comparing `panoptes_client-1.6.0/LICENSE` & `panoptes_client-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/PKG-INFO` & `panoptes_client-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes_client
-Version: 1.6.0
+Version: 1.6.1
 Summary: This package is the Python SDK for Panoptes, the platform behind the Zooniverse. This module is intended to allow programmatic management of projects, providing high level access to the API for common project management tasks.
 Home-page: https://github.com/zooniverse/panoptes-python-client
 Author: Adam McMaster / Zooniverse
 Author-email: contact@zooniverse.org
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `panoptes_client-1.6.0/README.md` & `panoptes_client-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/__init__.py` & `panoptes_client-1.6.1/panoptes_client/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/caesar.py` & `panoptes_client-1.6.1/panoptes_client/caesar.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     EXTRACTOR_TYPES = ['blank', 'external', 'question', 'survey', 'who', 'pluck_field', 'shape']
     REDUCER_TYPES = [
         'consensus', 'count', 'placeholder', 'external', 'first_extract', 'stats',
         'unique_count', 'rectangle', 'sqs'
     ]
     RULE_TO_ACTION_TYPES = {
-        'subject': ['retire_subject', 'add_subject_to_set', 'add_to_collection', 'external'],
+        'subject': ['retire_subject', 'add_subject_to_set', 'add_to_collection', 'external', 'external_with_basic_auth'],
         'user': ['promote_user']
     }
 
     def __init__(
         self,
         endpoint='https://caesar.zooniverse.org',
         redirect_url='https://caesar.zooniverse.org/auth/zooniverse/callback'
```

### Comparing `panoptes_client-1.6.0/panoptes_client/classification.py` & `panoptes_client-1.6.1/panoptes_client/classification.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/collection.py` & `panoptes_client-1.6.1/panoptes_client/collection.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/exportable.py` & `panoptes_client-1.6.1/panoptes_client/exportable.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/inaturalist.py` & `panoptes_client-1.6.1/panoptes_client/inaturalist.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/organization.py` & `panoptes_client-1.6.1/panoptes_client/organization.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/panoptes.py` & `panoptes_client-1.6.1/panoptes_client/panoptes.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/project.py` & `panoptes_client-1.6.1/panoptes_client/project.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/project_preferences.py` & `panoptes_client-1.6.1/panoptes_client/project_preferences.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/subject.py` & `panoptes_client-1.6.1/panoptes_client/subject.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/subject_set.py` & `panoptes_client-1.6.1/panoptes_client/subject_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     def add(self, subjects):
         """
         A wrapper around :py:meth:`.LinkCollection.add`. Equivalent to::
 
             subject_set.links.add(subjects)
         """
 
+        # reload the subject set to make sure the online version not stale
+        self.reload()
+
         return self.links.subjects.add(subjects)
 
     def remove(self, subjects):
         """
         A wrapper around :py:meth:`.LinkCollection.remove`. Equivalent to::
 
             subject_set.links.remove(subjects)
```

### Comparing `panoptes_client-1.6.0/panoptes_client/subject_workflow_status.py` & `panoptes_client-1.6.1/panoptes_client/subject_workflow_status.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_bearer_expiry.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_bearer_expiry.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_http_retries.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_http_retries.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_inaturalist.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_inaturalist.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_linkcollection.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_linkcollection.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_linkresolver.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_linkresolver.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_project.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_subject_set.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_subject_set.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/tests/test_workflow.py` & `panoptes_client-1.6.1/panoptes_client/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/user.py` & `panoptes_client-1.6.1/panoptes_client/user.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/utils.py` & `panoptes_client-1.6.1/panoptes_client/utils.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/workflow.py` & `panoptes_client-1.6.1/panoptes_client/workflow.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client/workflow_version.py` & `panoptes_client-1.6.1/panoptes_client/workflow_version.py`

 * *Files identical despite different names*

### Comparing `panoptes_client-1.6.0/panoptes_client.egg-info/PKG-INFO` & `panoptes_client-1.6.1/panoptes_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: This package is the Python SDK for Panoptes, the platform behind the Zooniverse. This module is intended to allow programmatic management of projects, providing high level access to the API for common project management tasks.
 Home-page: https://github.com/zooniverse/panoptes-python-client
 Author: Adam McMaster / Zooniverse
 Author-email: contact@zooniverse.org
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `panoptes_client-1.6.0/panoptes_client.egg-info/SOURCES.txt` & `panoptes_client-1.6.1/panoptes_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 panoptes_client/__init__.py
 panoptes_client/caesar.py
 panoptes_client/classification.py
 panoptes_client/collection.py
 panoptes_client/collection_role.py
```

### Comparing `panoptes_client-1.6.0/setup.py` & `panoptes_client-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     author='Adam McMaster / Zooniverse',
     author_email='contact@zooniverse.org',
     description=(
         'This package is the Python SDK for Panoptes, the platform behind the Zooniverse. This module is intended to allow programmatic management of projects, providing high level access to the API for common project management tasks.'
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.6.0',
+    version='1.6.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'requests>=2.4.2,<2.29',
         'future>=0.16,<0.19',
         'python-magic>=0.4,<0.5',
         'redo>=1.7',
         'six>=1.9',
     ],
     extras_require={
         'testing': [
-            'mock>=2.0,<4.1',
+            'mock>=2.0,<5.2',
         ],
         'docs': [
             'sphinx',
         ],
         ':python_version == "2.7"': ['futures'],
     }
 )
```

