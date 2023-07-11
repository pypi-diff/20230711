# Comparing `tmp/iam_actions-1.2.20230710.tar.gz` & `tmp/iam_actions-1.2.20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230710.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230711.tar", max compression
```

## Comparing `iam_actions-1.2.20230710.tar` & `iam_actions-1.2.20230711.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/README.md
--rw-r--r--   0        0        0      228 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/__init__.py
--rw-r--r--   0        0        0  4363235 2023-07-10 02:57:38.165626 iam_actions-1.2.20230710/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-10 02:56:04.556356 iam_actions-1.2.20230710/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560950 2023-07-10 02:57:38.165626 iam_actions-1.2.20230710/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-10 02:57:38.165626 iam_actions-1.2.20230710/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544067 2023-07-10 02:57:38.165626 iam_actions-1.2.20230710/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-10 02:57:38.945635 iam_actions-1.2.20230710/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230710/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230710/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/README.md
+-rw-r--r--   0        0        0      228 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4363235 2023-07-11 02:47:27.007415 iam_actions-1.2.20230711/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-11 02:45:26.667064 iam_actions-1.2.20230711/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-11 02:45:26.671065 iam_actions-1.2.20230711/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-11 02:45:26.671065 iam_actions-1.2.20230711/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-11 02:45:26.671065 iam_actions-1.2.20230711/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-11 02:45:26.671065 iam_actions-1.2.20230711/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560950 2023-07-11 02:47:27.007415 iam_actions-1.2.20230711/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-11 02:47:27.007415 iam_actions-1.2.20230711/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544067 2023-07-11 02:47:27.007415 iam_actions-1.2.20230711/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-11 02:47:27.927470 iam_actions-1.2.20230711/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230711/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230711/PKG-INFO
```

### Comparing `iam_actions-1.2.20230710/LICENSE` & `iam_actions-1.2.20230711/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/README.md` & `iam_actions-1.2.20230711/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/actions.json` & `iam_actions-1.2.20230711/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4135,217 +4135,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "CreateIngestionDestination": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetIngestionDestination": {
             "access_level": "Undocumented",
             "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAppBundles": {
             "access_level": "Undocumented",
             "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -17622,305 +17622,305 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "UpdateConfiguredTableAnalysisRule": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -25323,129 +25323,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "GetMetricsSummary": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
             "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -33019,25 +33019,25 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
@@ -33473,41 +33473,41 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "GetCustomerVerificationEligibility": {
+        "GetCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCustomerVerificationDetails": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -35151,41 +35151,41 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "ListUserProjects": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "ListUserProjects",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "ListUserProjects": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "ListUserProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectConfiguration": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProjectCredentials": {
             "access_level": "Undocumented",
@@ -35201,145 +35201,145 @@
             "access_level": "Undocumented",
             "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceByEnvironment": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceByEnvironment",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllAssociatedAccountsForEnvironment": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListAllAssociatedAccountsForEnvironment",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "ListMetadataCollectorRuns": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectorRuns": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectorRuns",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAssociatedDomain": {
             "access_level": "Undocumented",
             "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListMetadataCollectors": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectors": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectors",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDataSource": {
             "access_level": "Undocumented",
@@ -35353,81 +35353,81 @@
             "access_level": "Undocumented",
             "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -57160,225 +57160,225 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "ModifyTargetGroupAttributes": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RegisterTargets": {
             "access_level": "Undocumented",
             "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateTargetGroup": {
             "access_level": "Undocumented",
             "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyListener": {
             "access_level": "Undocumented",
             "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -63928,33 +63928,33 @@
             "condition_keys": [],
             "description": "Grants permission to verify the email for FreeRTOS extended maintenance plan (EMP)",
             "orphan": false,
             "resources": []
         }
     },
     "freetier": {
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -72425,1377 +72425,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "PassRole": {
-            "access_level": "Undocumented",
-            "action": "PassRole",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetAccountName": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AttachGroupPolicy": {
             "access_level": "Undocumented",
             "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateInstanceProfile": {
             "access_level": "Undocumented",
             "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListGroupPolicies": {
             "access_level": "Undocumented",
             "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "PutUserPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreatePolicyVersion": {
+            "access_level": "Undocumented",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateServerCertificate": {
             "access_level": "Undocumented",
             "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -75620,33 +75620,33 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "GetInvoiceEmailDeliveryPreferences": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListInvoiceSummaries": {
             "access_level": "Undocumented",
             "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetInvoicePDF": {
             "access_level": "Undocumented",
@@ -81561,889 +81561,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "DeleteDeviceProfile": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -85251,315 +85251,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRescoreExecutionPlans": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "DescribeStreamConsumer": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -88145,169 +88145,169 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "ListProvisionedApps": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSettingsSet": {
             "access_level": "Undocumented",
             "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -96971,225 +96971,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "ListChannelGroups": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutObject": {
             "access_level": "Undocumented",
             "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -104269,251 +104269,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "UpdateEventRule": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListEventRules": {
             "access_level": "Undocumented",
             "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "ListEmailContacts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteEmailContact": {
             "access_level": "Undocumented",
             "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -106886,129 +106886,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "ListPipelines": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeletePipeline": {
             "access_level": "Undocumented",
             "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPipeline": {
             "access_level": "Undocumented",
             "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -107623,267 +107623,267 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payment-cryptography": {
-        "ExportKey": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "ListPaymentPreferences": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPaymentStatus": {
             "access_level": "Undocumented",
@@ -107897,41 +107897,41 @@
             "access_level": "Undocumented",
             "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -113368,281 +113368,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "ListResourceTypes": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
             "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicies": {
             "access_level": "Undocumented",
             "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131219,113 +131219,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "UntagResource": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAdminUsers": {
             "access_level": "Undocumented",
             "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -146331,265 +146331,265 @@
             "access_level": "Undocumented",
             "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -148424,201 +148424,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "ListIdentitySources": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPolicies": {
             "access_level": "Undocumented",
             "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
```

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230711/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230711/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/generate.py` & `iam_actions-1.2.20230711/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230711/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230711/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/generate/services.py` & `iam_actions-1.2.20230711/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/policies.json` & `iam_actions-1.2.20230711/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230711/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/iam_actions/services.json` & `iam_actions-1.2.20230711/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230710/pyproject.toml` & `iam_actions-1.2.20230711/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230710"
+version = "1.2.20230711"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230710/setup.py` & `iam_actions-1.2.20230711/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230710',
+    'version': '1.2.20230711',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230710/PKG-INFO` & `iam_actions-1.2.20230711/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230710
+Version: 1.2.20230711
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

