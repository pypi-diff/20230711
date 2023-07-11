# Comparing `tmp/cdk-monitoring-constructs-5.3.1.tar.gz` & `tmp/cdk-monitoring-constructs-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-monitoring-constructs-5.3.1.tar", last modified: Mon Jul 10 00:40:21 2023, max compression
+gzip compressed data, was "cdk-monitoring-constructs-5.3.2.tar", last modified: Tue Jul 11 16:41:20 2023, max compression
```

## Comparing `cdk-monitoring-constructs-5.3.1.tar` & `cdk-monitoring-constructs-5.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:40:21.535379 cdk-monitoring-constructs-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-07-10 00:40:21.535379 cdk-monitoring-constructs-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 00:40:21.535379 cdk-monitoring-constructs-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:40:21.523378 cdk-monitoring-constructs-5.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:40:21.531379 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)  4575968 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:40:21.531379 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   788628 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.3.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:40:06.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:40:21.531379 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-07-10 00:40:21.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 00:40:21.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:40:21.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 00:40:21.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 00:40:21.000000 cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:41:20.228724 cdk-monitoring-constructs-5.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)  4575968 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   788629 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.3.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:41:05.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:41:20.236725 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-07-11 16:41:20.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-11 16:41:20.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:41:20.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 16:41:20.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 16:41:20.000000 cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/top_level.txt
```

### Comparing `cdk-monitoring-constructs-5.3.1/LICENSE` & `cdk-monitoring-constructs-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.3.1/PKG-INFO` & `cdk-monitoring-constructs-5.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.3.1
+Version: 5.3.2
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-5.3.1/README.md` & `cdk-monitoring-constructs-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.3.1/setup.py` & `cdk-monitoring-constructs-5.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-monitoring-constructs",
-    "version": "5.3.1",
+    "version": "5.3.2",
     "description": "cdk-monitoring-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-monitoring-constructs",
     "long_description_content_type": "text/markdown",
     "author": "CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_monitoring_constructs",
         "cdk_monitoring_constructs._jsii"
     ],
     "package_data": {
         "cdk_monitoring_constructs._jsii": [
-            "cdk-monitoring-constructs@5.3.1.jsii.tgz"
+            "cdk-monitoring-constructs@5.3.2.jsii.tgz"
         ],
         "cdk_monitoring_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/__init__.py` & `cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs/_jsii/__init__.py` & `cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_redshift_alpha._jsii
 import aws_cdk.aws_synthetics_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-monitoring-constructs",
-    "5.3.1",
+    "5.3.2",
     __name__[0:-6],
-    "cdk-monitoring-constructs@5.3.1.jsii.tgz",
+    "cdk-monitoring-constructs@5.3.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/PKG-INFO` & `cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.3.1
+Version: 5.3.2
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-5.3.1/src/cdk_monitoring_constructs.egg-info/SOURCES.txt` & `cdk-monitoring-constructs-5.3.2/src/cdk_monitoring_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_monitoring_constructs/py.typed
 src/cdk_monitoring_constructs.egg-info/PKG-INFO
 src/cdk_monitoring_constructs.egg-info/SOURCES.txt
 src/cdk_monitoring_constructs.egg-info/dependency_links.txt
 src/cdk_monitoring_constructs.egg-info/requires.txt
 src/cdk_monitoring_constructs.egg-info/top_level.txt
 src/cdk_monitoring_constructs/_jsii/__init__.py
-src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.3.1.jsii.tgz
+src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.3.2.jsii.tgz
```

