# Comparing `tmp/pysigma_backend_carbonblack-0.1.2.tar.gz` & `tmp/pysigma_backend_carbonblack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_carbonblack-0.1.2.tar", max compression
+gzip compressed data, was "pysigma_backend_carbonblack-0.1.3.tar", max compression
```

## Comparing `pysigma_backend_carbonblack-0.1.2.tar` & `pysigma_backend_carbonblack-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/LICENSE
--rw-r--r--   0        0        0      575 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      371 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0     6915 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      315 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/__init__.py
--rw-r--r--   0        0        0    13283 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0     6915 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      315 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/__init__.py
+-rw-r--r--   0        0        0    13828 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.3/PKG-INFO
```

### Comparing `pysigma_backend_carbonblack-0.1.2/LICENSE` & `pysigma_backend_carbonblack-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.2/pyproject.toml` & `pysigma_backend_carbonblack-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-carbonblack"
-version = "0.1.2"
+version = "0.1.3"
 description = "pySigma carbonblack backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-carbonblack"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/carbonblack.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,25 +124,25 @@
     ]
 
     unsupported_rule_types = [
         # Show error if unsupported option
         ProcessingItem(
             identifier="cbr_fail_rule_not_supported",
             rule_condition_linking=any,
-            transformation=RuleFailureTransformation("Rule type not yet supported by the SentinelOne Sigma backend"),
+            transformation=RuleFailureTransformation("Rule type not yet supported by the Carbon Black Response Sigma backend"),
             rule_condition_negation=True,
             rule_conditions=[
                 RuleProcessingItemAppliedCondition("cbr_logsource")
             ]
         )
     ]
 
     unsupported_field_names = [
         ProcessingItem(
-            identifier="cb_fail_field_name_not_supported",
+            identifier="cbr_fail_field_name_not_supported",
             transformation=InvalidFieldTransformation("The supported fields are: {" + 
                 "}, {".join(sorted(list(translation_dict.keys()))) + '}'),
             field_name_conditions=[
                 ExcludeFieldCondition(fields=list(translation_dict.keys()))
             ],
             field_name_condition_linking=any
         )
@@ -269,18 +269,33 @@
                 "sha256":"modload_hash",
                 "md5": "modload_hash",
             }),
             rule_conditions=[
                 LogsourceCondition(category="image_load")
             ]
         ),
+        # File Changes Hashes
+        ProcessingItem(
+            identifier="cb_filemod_fieldmapping",
+            transformation=FieldMappingTransformation({
+                "sha256":"filemod_hash",
+                "md5": "filemod_hash",
+            }),
+            rule_condition_linking=any,
+            rule_conditions=[
+                LogsourceCondition(category="file_change"),
+                LogsourceCondition(category="file_rename"),
+                LogsourceCondition(category="file_delete"),
+                LogsourceCondition(category="file_event"),
+            ]
+        ),
     ]
 
     change_logsource_info = [
-        # Add service to be SentinelOne for pretty much everything
+        # Add service to be CarbonBlack for pretty much everything
         ProcessingItem(
             identifier="cb_logsource",
             transformation=ChangeLogsourceTransformation(
                 service="carbonblack"
             ),
             rule_condition_linking=any,
             rule_conditions=[
@@ -301,15 +316,15 @@
     ]
 
     unsupported_rule_types = [
         # Show error if unsupported option
         ProcessingItem(
             identifier="cb_fail_rule_not_supported",
             rule_condition_linking=any,
-            transformation=RuleFailureTransformation("Rule type not yet supported by the SentinelOne Sigma backend"),
+            transformation=RuleFailureTransformation("Rule type not yet supported by the Carbon Black Sigma backend"),
             rule_condition_negation=True,
             rule_conditions=[
                 RuleProcessingItemAppliedCondition("cb_logsource")
             ]
         )
     ]
 
@@ -323,16 +338,16 @@
             ],
             field_name_condition_linking=any
         )
     ]
 
     return ProcessingPipeline(
         name="carbonblack pipeline",
-        allowed_backends=frozenset(),                                               # Set of identifiers of backends (from the backends mapping) that are allowed to use this processing pipeline. This can be used by frontends like Sigma CLI to warn the user about inappropriate usage.
-        priority=50,            # The priority defines the order pipelines are applied. See documentation for common values.
+        allowed_backends=frozenset(), # Set of identifiers of backends (from the backends mapping) that are allowed to use this processing pipeline. This can be used by frontends like Sigma CLI to warn the user about inappropriate usage.
+        priority=50, # The priority defines the order pipelines are applied. See documentation for common values.
         items=[
             *unsupported_field_names,
             *os_filters,
             *field_mappings,
             *change_logsource_info,
             *unsupported_rule_types
         ]
```

### Comparing `pysigma_backend_carbonblack-0.1.2/PKG-INFO` & `pysigma_backend_carbonblack-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-carbonblack
-Version: 0.1.2
+Version: 0.1.3
 Summary: pySigma carbonblack backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-carbonblack
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

