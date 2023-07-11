# Comparing `tmp/tzspace-0.0.4.tar.gz` & `tmp/tzspace-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzspace-0.0.4.tar", last modified: Tue Jul 11 07:03:25 2023, max compression
+gzip compressed data, was "tzspace-0.0.5.tar", last modified: Tue Jul 11 07:22:53 2023, max compression
```

## Comparing `tzspace-0.0.4.tar` & `tzspace-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.522627 tzspace-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      530 2023-07-11 07:03:25.521621 tzspace-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-07-08 13:47:46.000000 tzspace-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.497249 tzspace-0.0.4/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.4/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.499286 tzspace-0.0.4/ior/config/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.4/ior/config/__init__.py
--rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.4/ior/config/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.509507 tzspace-0.0.4/ior/core/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.4/ior/core/__init__.py
--rw-rw-rw-   0        0        0     6241 2023-07-11 06:38:39.000000 tzspace-0.0.4/ior/core/certificate_service.py
--rw-rw-rw-   0        0        0     1657 2023-07-08 15:09:13.000000 tzspace-0.0.4/ior/core/exchange_service.py
--rw-rw-rw-   0        0        0     3706 2023-07-08 15:08:37.000000 tzspace-0.0.4/ior/core/permission_control_service.py
--rw-rw-rw-   0        0        0     4546 2023-07-08 15:08:23.000000 tzspace-0.0.4/ior/core/role_control_service.py
--rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.4/ior/core/stored_nft_service.py
--rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.4/ior/core/tz_contract_template_service.py
--rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.4/ior/core/tz_template_control_service.py
--rw-rw-rw-   0        0        0     1355 2023-07-08 15:14:38.000000 tzspace-0.0.4/ior/iorconfig.py
--rw-rw-rw-   0        0        0     2634 2023-07-11 07:02:50.000000 tzspace-0.0.4/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.515567 tzspace-0.0.4/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.4/ior/util/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.4/ior/util/certificate_utils.py
--rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.4/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.4/ior/util/web3_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-11 07:03:25.522627 tzspace-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-11 07:03:22.000000 tzspace-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:03:25.520608 tzspace-0.0.4/tzspace.egg-info/
--rw-rw-rw-   0        0        0      530 2023-07-11 07:03:25.000000 tzspace-0.0.4/tzspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-07-11 07:03:25.000000 tzspace-0.0.4/tzspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 07:03:25.000000 tzspace-0.0.4/tzspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 07:03:25.000000 tzspace-0.0.4/tzspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.789003 tzspace-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 tzspace-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      530 2023-07-11 07:22:53.788000 tzspace-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-07-08 13:47:46.000000 tzspace-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.745126 tzspace-0.0.5/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.5/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.747126 tzspace-0.0.5/ior/config/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.5/ior/config/__init__.py
+-rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.5/ior/config/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.759993 tzspace-0.0.5/ior/config/contracts/
+-rw-rw-rw-   0        0        0    90537 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/Certificate.json
+-rw-rw-rw-   0        0        0    29114 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/Exchange.json
+-rw-rw-rw-   0        0        0    26608 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/PermissionControl.json
+-rw-rw-rw-   0        0        0    29186 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/RoleControl.json
+-rw-rw-rw-   0        0        0    71651 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/StoredNFT.json
+-rw-rw-rw-   0        0        0    35700 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/TZContractTemplate.json
+-rw-rw-rw-   0        0        0    38166 2023-03-26 16:06:07.000000 tzspace-0.0.5/ior/config/contracts/TZTemplateControl.json
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.773003 tzspace-0.0.5/ior/core/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.5/ior/core/__init__.py
+-rw-rw-rw-   0        0        0     6241 2023-07-11 06:38:39.000000 tzspace-0.0.5/ior/core/certificate_service.py
+-rw-rw-rw-   0        0        0     1657 2023-07-08 15:09:13.000000 tzspace-0.0.5/ior/core/exchange_service.py
+-rw-rw-rw-   0        0        0     3706 2023-07-08 15:08:37.000000 tzspace-0.0.5/ior/core/permission_control_service.py
+-rw-rw-rw-   0        0        0     4546 2023-07-08 15:08:23.000000 tzspace-0.0.5/ior/core/role_control_service.py
+-rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.5/ior/core/stored_nft_service.py
+-rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.5/ior/core/tz_contract_template_service.py
+-rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.5/ior/core/tz_template_control_service.py
+-rw-rw-rw-   0        0        0     1355 2023-07-08 15:14:38.000000 tzspace-0.0.5/ior/iorconfig.py
+-rw-rw-rw-   0        0        0     2634 2023-07-11 07:02:50.000000 tzspace-0.0.5/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.779003 tzspace-0.0.5/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.5/ior/util/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.5/ior/util/certificate_utils.py
+-rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.5/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.5/ior/util/web3_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 07:22:53.789003 tzspace-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-07-11 07:19:06.000000 tzspace-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:22:53.787000 tzspace-0.0.5/tzspace.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-07-11 07:22:53.000000 tzspace-0.0.5/tzspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-07-11 07:22:53.000000 tzspace-0.0.5/tzspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 07:22:53.000000 tzspace-0.0.5/tzspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 07:22:53.000000 tzspace-0.0.5/tzspace.egg-info/top_level.txt
```

### Comparing `tzspace-0.0.4/LICENSE` & `tzspace-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/PKG-INFO` & `tzspace-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzspace
-Version: 0.0.4
+Version: 0.0.5
 Summary: tzspace sdk for ior standard
 Home-page: https://github.com/tzspace
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tzspace-0.0.4/ior/config/consts.py` & `tzspace-0.0.5/ior/config/consts.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/certificate_service.py` & `tzspace-0.0.5/ior/core/certificate_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/exchange_service.py` & `tzspace-0.0.5/ior/core/exchange_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/permission_control_service.py` & `tzspace-0.0.5/ior/core/permission_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/role_control_service.py` & `tzspace-0.0.5/ior/core/role_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/stored_nft_service.py` & `tzspace-0.0.5/ior/core/stored_nft_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/tz_contract_template_service.py` & `tzspace-0.0.5/ior/core/tz_contract_template_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/core/tz_template_control_service.py` & `tzspace-0.0.5/ior/core/tz_template_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/iorconfig.py` & `tzspace-0.0.5/ior/iorconfig.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/iorsdk.py` & `tzspace-0.0.5/ior/iorsdk.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/util/certificate_utils.py` & `tzspace-0.0.5/ior/util/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/util/result_utils.py` & `tzspace-0.0.5/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/ior/util/web3_utils.py` & `tzspace-0.0.5/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.4/tzspace.egg-info/PKG-INFO` & `tzspace-0.0.5/tzspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzspace
-Version: 0.0.4
+Version: 0.0.5
 Summary: tzspace sdk for ior standard
 Home-page: https://github.com/tzspace
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

