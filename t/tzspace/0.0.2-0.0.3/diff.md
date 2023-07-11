# Comparing `tmp/tzspace-0.0.2.tar.gz` & `tmp/tzspace-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzspace-0.0.2.tar", last modified: Sat Jul  8 15:19:55 2023, max compression
+gzip compressed data, was "tzspace-0.0.3.tar", last modified: Tue Jul 11 06:58:14 2023, max compression
```

## Comparing `tzspace-0.0.2.tar` & `tzspace-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.628903 tzspace-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      530 2023-07-08 15:19:55.628903 tzspace-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-07-08 13:47:46.000000 tzspace-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.603985 tzspace-0.0.2/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.2/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.607798 tzspace-0.0.2/ior/config/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.2/ior/config/__init__.py
--rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.2/ior/config/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.617778 tzspace-0.0.2/ior/core/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.2/ior/core/__init__.py
--rw-rw-rw-   0        0        0     6401 2023-07-08 15:04:51.000000 tzspace-0.0.2/ior/core/certificate_service.py
--rw-rw-rw-   0        0        0     1657 2023-07-08 15:09:13.000000 tzspace-0.0.2/ior/core/exchange_service.py
--rw-rw-rw-   0        0        0     3706 2023-07-08 15:08:37.000000 tzspace-0.0.2/ior/core/permission_control_service.py
--rw-rw-rw-   0        0        0     4546 2023-07-08 15:08:23.000000 tzspace-0.0.2/ior/core/role_control_service.py
--rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.2/ior/core/stored_nft_service.py
--rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.2/ior/core/tz_contract_template_service.py
--rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.2/ior/core/tz_template_control_service.py
--rw-rw-rw-   0        0        0     1355 2023-07-08 15:14:38.000000 tzspace-0.0.2/ior/iorconfig.py
--rw-rw-rw-   0        0        0     2652 2023-07-08 15:18:10.000000 tzspace-0.0.2/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.622878 tzspace-0.0.2/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.2/ior/util/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.2/ior/util/certificate_utils.py
--rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.2/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.2/ior/util/web3_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-08 15:19:55.628903 tzspace-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-08 15:19:13.000000 tzspace-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:19:55.627894 tzspace-0.0.2/tzspace.egg-info/
--rw-rw-rw-   0        0        0      530 2023-07-08 15:19:55.000000 tzspace-0.0.2/tzspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-07-08 15:19:55.000000 tzspace-0.0.2/tzspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:19:55.000000 tzspace-0.0.2/tzspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 15:19:55.000000 tzspace-0.0.2/tzspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.417156 tzspace-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      530 2023-07-11 06:58:14.417156 tzspace-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-07-08 13:47:46.000000 tzspace-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.393154 tzspace-0.0.3/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.3/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.395152 tzspace-0.0.3/ior/config/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.3/ior/config/__init__.py
+-rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.3/ior/config/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.404152 tzspace-0.0.3/ior/core/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.3/ior/core/__init__.py
+-rw-rw-rw-   0        0        0     6241 2023-07-11 06:38:39.000000 tzspace-0.0.3/ior/core/certificate_service.py
+-rw-rw-rw-   0        0        0     1657 2023-07-08 15:09:13.000000 tzspace-0.0.3/ior/core/exchange_service.py
+-rw-rw-rw-   0        0        0     3706 2023-07-08 15:08:37.000000 tzspace-0.0.3/ior/core/permission_control_service.py
+-rw-rw-rw-   0        0        0     4546 2023-07-08 15:08:23.000000 tzspace-0.0.3/ior/core/role_control_service.py
+-rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.3/ior/core/stored_nft_service.py
+-rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.3/ior/core/tz_contract_template_service.py
+-rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.3/ior/core/tz_template_control_service.py
+-rw-rw-rw-   0        0        0     1355 2023-07-08 15:14:38.000000 tzspace-0.0.3/ior/iorconfig.py
+-rw-rw-rw-   0        0        0     2709 2023-07-11 06:37:49.000000 tzspace-0.0.3/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.411152 tzspace-0.0.3/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.3/ior/util/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.3/ior/util/certificate_utils.py
+-rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.3/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.3/ior/util/web3_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 06:58:14.417156 tzspace-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-07-11 06:58:10.000000 tzspace-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:58:14.416152 tzspace-0.0.3/tzspace.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-07-11 06:58:14.000000 tzspace-0.0.3/tzspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-07-11 06:58:14.000000 tzspace-0.0.3/tzspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 06:58:14.000000 tzspace-0.0.3/tzspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 06:58:14.000000 tzspace-0.0.3/tzspace.egg-info/top_level.txt
```

### Comparing `tzspace-0.0.2/LICENSE` & `tzspace-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/PKG-INFO` & `tzspace-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzspace
-Version: 0.0.2
+Version: 0.0.3
 Summary: tzspace sdk for ior standard
 Home-page: https://github.com/tzspace
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tzspace-0.0.2/ior/config/consts.py` & `tzspace-0.0.3/ior/config/consts.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/certificate_service.py` & `tzspace-0.0.3/ior/core/certificate_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+
 from ..config.consts import certificate_path
-from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions, \
-    create_account
+from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions
 from hexbytes import (
     HexBytes,
 )
 
 
 class CertificateService(object):
     def __init__(self, w3, config, address):
@@ -15,21 +15,14 @@
 
     @property
     def functions(self):
         if not self.certificate_contract_instance:
             raise RuntimeError("合约获取失败【certificate_contract】")
         return contract_functions(self.certificate_contract_instance)
 
-    def create_account(self):
-        """
-        创建账户
-        :return:
-        """
-        return create_account(self.w3)
-
     def token_id_mapping_item(self, key):
         """
         合约属性 mapping(uint256 => uint256) public tokenIdMapping
         :param key:
         :return:
         """
         res = self.functions.tokenIdMapping(key).call()
```

### Comparing `tzspace-0.0.2/ior/core/exchange_service.py` & `tzspace-0.0.3/ior/core/exchange_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/permission_control_service.py` & `tzspace-0.0.3/ior/core/permission_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/role_control_service.py` & `tzspace-0.0.3/ior/core/role_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/stored_nft_service.py` & `tzspace-0.0.3/ior/core/stored_nft_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/tz_contract_template_service.py` & `tzspace-0.0.3/ior/core/tz_contract_template_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/core/tz_template_control_service.py` & `tzspace-0.0.3/ior/core/tz_template_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/iorconfig.py` & `tzspace-0.0.3/ior/iorconfig.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/util/certificate_utils.py` & `tzspace-0.0.3/ior/util/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/util/result_utils.py` & `tzspace-0.0.3/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/ior/util/web3_utils.py` & `tzspace-0.0.3/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.2/setup.py` & `tzspace-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="tzspace",
-  version="0.0.2",
+  version="0.0.3",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="tzspace sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace",
   packages=setuptools.find_packages(),
```

### Comparing `tzspace-0.0.2/tzspace.egg-info/PKG-INFO` & `tzspace-0.0.3/tzspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzspace
-Version: 0.0.2
+Version: 0.0.3
 Summary: tzspace sdk for ior standard
 Home-page: https://github.com/tzspace
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tzspace-0.0.2/tzspace.egg-info/SOURCES.txt` & `tzspace-0.0.3/tzspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

