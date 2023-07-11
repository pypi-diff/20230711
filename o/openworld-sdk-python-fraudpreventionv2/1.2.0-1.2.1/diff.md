# Comparing `tmp/openworld-sdk-python-fraudpreventionv2-1.2.0.tar.gz` & `tmp/openworld-sdk-python-fraudpreventionv2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.2.0.tar", last modified: Tue Jul 11 14:09:49 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.2.1.tar", last modified: Tue Jul 11 14:33:07 2023, max compression
```

## Comparing `openworld-sdk-python-fraudpreventionv2-1.2.0.tar` & `openworld-sdk-python-fraudpreventionv2-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    99892 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-11 14:09:31.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.957057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.957057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99892 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-11 14:32:53.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/setup.py
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/__init__.py` & `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/client.py` & `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 from openworld.sdk.core.client.openworld_auth_client import _OpenWorldAuthClient
 from openworld.sdk.core.configuration.client_config import ClientConfig
 from openworld.sdk.core.constant import header
 
 from .model import *
 
 
-class Fraudpreventionv2Client:
+class FraudPreventionV2Client:
     def __init__(self, client_config: ClientConfig):
-        r"""fraudPreventionV2 API Client.
+        r"""F r a u d P r e v e n t i o n V 2 API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.2.0'
+        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.2.1'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(
         self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/model.py` & `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/model.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.0/setup.py` & `openworld-sdk-python-fraudpreventionv2-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudpreventionv2',
-    version='1.2.0',
+    version='1.2.1',
     packages=['openworld.sdk.fraudpreventionv2'],
     package_dir={'openworld-sdk-python-fraudpreventionv2': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
@@ -33,10 +33,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.8',
     install_requires=['uri', 'furl', 'openworld-sdk-python-core', 'pydantic', 'pydantic[email]', 'email-validator'],
-    description='Open World fraudPreventionV2 SDK for Python',
-    long_description='Open World fraudPreventionV2 SDK for Python',
+    description='Open World F r a u d P r e v e n t i o n V 2 SDK for Python',
+    long_description='Open World F r a u d P r e v e n t i o n V 2 SDK for Python',
 )
```

