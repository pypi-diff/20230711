# Comparing `tmp/mdast_cli-2023.7.1.tar.gz` & `tmp/mdast_cli-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.7.1.tar", last modified: Wed Jul  5 14:26:48 2023, max compression
+gzip compressed data, was "mdast_cli-2023.7.2.tar", last modified: Mon Jul 10 23:46:09 2023, max compression
```

## Comparing `mdast_cli-2023.7.1.tar` & `mdast_cli-2023.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.494159 mdast_cli-2023.7.2/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/setup.py
```

### Comparing `mdast_cli-2023.7.1/PKG-INFO` & `mdast_cli-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.7.1/README.md` & `mdast_cli-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/app_center.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appgallery.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import logging
 import os
+import time
 
 import requests
 
 logger = logging.getLogger(__name__)
 
 
 def get_app_info(app_id):
-    req = requests.get(f'https://web-dre.hispace.dbankcloud.cn/uowap/index?method='
-                       f'internal.getTabDetail&serviceType=20&reqPageNum=1&maxResults=25&uri=app|{app_id}')
+    get_interface_code_resp = requests.post('https://web-drru.hispace.dbankcloud.ru/webedge/getInterfaceCode')
+    if get_interface_code_resp.status_code != 200:
+        raise RuntimeError('Appgallery - Cannot get interface code, connection error')
+    interface_code = get_interface_code_resp.json()
+    timestamp = time.time()
+    timestamp = str(timestamp).replace('.', '')
+    headers = {
+        'Interface-Code': f'{interface_code}_{timestamp}'
+    }
+    req = requests.get(f'https://web-drru.hispace.dbankcloud.ru/uowap/index?'
+                       f'method=internal.getTabDetail&uri=app%7C{app_id}', headers=headers)
     if req.status_code == 200:
         resp_info = req.json()
     else:
         raise RuntimeError(f'Appgallery - Failed to get application info. '
                            f'Request return status code: {req.status_code}')
     app_info = {}
 
-    layoutData = resp_info.get('layoutData', [])
-    for element in layoutData:
+    layout_data = resp_info.get('layoutData', [])
+    for element in layout_data:
         if 'dataList' not in element.keys():
             continue
 
         for item in element.get('dataList', []):
             if 'package' not in item.keys():
                 continue
             if app_id != item.get('appid'):
```

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/firebase.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/firebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,29 @@
 
 def firebase_download_app(download_path, project_number, app_id, account_info, file_name=None,
                           file_extension='apk'):
     logger.info(f'Firebase - Try to download {file_extension} from latest release in project - '
                 f'{project_number} with app id {app_id}')
     app_info = get_app_info(project_number, app_id, account_info)
     app_download_link = app_info['download_link']
-    app_file = requests.get(app_download_link, allow_redirects=True)
+    app_file_resp = requests.get(app_download_link, allow_redirects=True)
+    if app_file_resp != 200:
+        raise RuntimeError(f'Firebase - Failed to download application, status code - {app_file_resp.status_code} ')
 
     if file_name is None:
         file_name = app_info['version_name']
 
     path_to_file = f'{download_path}/{file_name}.{file_extension}'
 
     if not os.path.exists(download_path):
         os.mkdir(download_path)
         logger.info(f'Firebase - Creating directory {download_path} for downloading app from Firebase')
 
     with open(path_to_file, 'wb') as file:
-        file.write(app_file.content)
+        file.write(app_file_resp.content)
 
     if os.path.exists(path_to_file):
         logger.info(f'Firebase - Application successfully downloaded to {path_to_file}')
     else:
         logger.info('Firebase - Failed to download application. '
                     'Seems like something is wrong with your file path or app file is broken')
```

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/google_play.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.7.2/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/helpers/const.py` & `mdast_cli-2023.7.2/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli/mdast_scan.py` & `mdast_cli-2023.7.2/mdast_cli/mdast_scan.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.7.2/mdast_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.7.1/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.7.2/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.7.2/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli_core/api.py` & `mdast_cli-2023.7.2/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli_core/base.py` & `mdast_cli-2023.7.2/mdast_cli_core/base.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/mdast_cli_core/token.py` & `mdast_cli-2023.7.2/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.1/setup.py` & `mdast_cli-2023.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.07.01',
+    version='2023.07.02',
 
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

