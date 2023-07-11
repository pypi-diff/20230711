# Comparing `tmp/amplify_aws_utils-0.4.3.tar.gz` & `tmp/amplify_aws_utils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amplify_aws_utils-0.4.3.tar", last modified: Fri Jun 30 16:08:13 2023, max compression
+gzip compressed data, was "dist/amplify_aws_utils-0.4.4.tar", last modified: Tue Jul 11 17:34:36 2023, max compression
```

## Comparing `amplify_aws_utils-0.4.3.tar` & `amplify_aws_utils-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/spotinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/sts.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/resource_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/s3_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 16:08:12.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/requirements.pip
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/test-requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/spotinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/clients/sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/resource_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/s3_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:34:35.000000 amplify_aws_utils-0.4.4/amplify_aws_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/requirements.pip
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:34:36.000000 amplify_aws_utils-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-11 17:34:34.000000 amplify_aws_utils-0.4.4/test-requirements.pip
```

### Comparing `amplify_aws_utils-0.4.3/PKG-INFO` & `amplify_aws_utils-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: amplify_aws_utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Utility functions for working with AWS resources
 Home-page: https://github.com/amplify-education/amplify_aws_utils/
 Author: Amplify Education
 Author-email: astronauts.core@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Grade)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Coverage)
```

### Comparing `amplify_aws_utils-0.4.3/README.md` & `amplify_aws_utils-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/config.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/clients/config.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/ec2.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/clients/ec2.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/s3.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/clients/s3.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/spotinst.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/clients/spotinst.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/sts.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/clients/sts.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/exceptions.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/jitter.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/jitter.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/resource_helper.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/resource_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         print group
     # [0, 1, 2, 3, 4]
     # [5, 6, 7, 8, 9]
     # [10, 11, 12, 13, 14]
     # [15, 16, 17, 18, 19]
     """
     return (
-        sequence[position : position + size]
+        sequence[position: position + size]
         for position in range(0, len(sequence), size)
     )
 
 
 def dynamodb_record_to_dict(record: Dict[str, Dict[str, str]]) -> Dict[str, str]:
     """
     Converts a DynamoDB Record into a normal Python dictionary.
@@ -453,7 +453,18 @@
             # exception, but necessary to retain the exception chaining info b/c exception
             # chaining will be lost once an exception propagates out of a lambda function
             raise CatchAllExceptionError(
                 f"Catchall exception. err_mssg: {err_mssg}, stack_trace: {stack_trace}"
             ) from exc
 
     return None
+
+
+def to_bool(value: Any) -> bool:
+    """
+    Convert `value` to the lower string and compare with the list ["yes", "y", "true", "t", "on", "1"]
+    If in the list then `true` else `false`
+    """
+    if str(value).lower() in ["yes", "y", "true", "t", "on", "1"]:
+        return True
+
+    return False
```

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils/s3_uri.py` & `amplify_aws_utils-0.4.4/amplify_aws_utils/s3_uri.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/PKG-INFO` & `amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: amplify-aws-utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Utility functions for working with AWS resources
 Home-page: https://github.com/amplify-education/amplify_aws_utils/
 Author: Amplify Education
 Author-email: astronauts.core@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Grade)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Coverage)
```

### Comparing `amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/SOURCES.txt` & `amplify_aws_utils-0.4.4/amplify_aws_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.3/setup.py` & `amplify_aws_utils-0.4.4/setup.py`

 * *Files identical despite different names*

