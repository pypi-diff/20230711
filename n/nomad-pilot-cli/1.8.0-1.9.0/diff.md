# Comparing `tmp/nomad_pilot_cli-1.8.0.tar.gz` & `tmp/nomad_pilot_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nomad_pilot_cli-1.8.0.tar", last modified: Thu Sep 12 01:08:14 2019, max compression
+gzip compressed data, was "dist/nomad_pilot_cli-1.9.0.tar", last modified: Thu Sep 12 09:02:33 2019, max compression
```

## Comparing `nomad_pilot_cli-1.8.0.tar` & `nomad_pilot_cli-1.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/
--rw-r--r--   0 dev        (501) staff       (20)      381 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/PKG-INFO
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      381 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)     1134 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)       67 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 dev        (501) staff       (20)       21 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/dependency_links.txt
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/test/
--rw-r--r--   0 dev        (501) staff       (20)     1079 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_api_response_connector_response.py
--rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_package.py
--rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_address.py
--rw-r--r--   0 dev        (501) staff       (20)      921 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_dimension.py
--rw-r--r--   0 dev        (501) staff       (20)     1105 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/test/test_ship_api.py
--rw-r--r--   0 dev        (501) staff       (20)      939 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_api_response.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/test/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_goldjet.py
--rw-r--r--   0 dev        (501) staff       (20)      973 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/test/test_api_response_data.py
--rw-r--r--   0 dev        (501) staff       (20)      939 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/test/test_package_item.py
--rw-r--r--   0 dev        (501) staff       (20)     3185 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/README.md
--rw-r--r--   0 dev        (501) staff       (20)     1083 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/setup.py
--rw-r--r--   0 dev        (501) staff       (20)       38 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/
--rw-r--r--   0 dev        (501) staff       (20)     9936 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/configuration.py
--rw-r--r--   0 dev        (501) staff       (20)     6161 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/swagger_validator.py
--rw-r--r--   0 dev        (501) staff       (20)     9598 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/append_alibaba_headers.py
--rw-r--r--   0 dev        (501) staff       (20)    12815 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/rest.py
--rw-r--r--   0 dev        (501) staff       (20)     1372 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/
--rw-r--r--   0 dev        (501) staff       (20)    22852 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/package.py
--rw-r--r--   0 dev        (501) staff       (20)    13178 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/address.py
--rw-r--r--   0 dev        (501) staff       (20)    12436 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/package_item.py
--rw-r--r--   0 dev        (501) staff       (20)    10903 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response_connector_response.py
--rw-r--r--   0 dev        (501) staff       (20)      880 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)     8739 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response_data.py
--rw-r--r--   0 dev        (501) staff       (20)     6169 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response.py
--rw-r--r--   0 dev        (501) staff       (20)     3071 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/goldjet.py
--rw-r--r--   0 dev        (501) staff       (20)     4767 2019-09-11 19:30:24.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/dimension.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 01:08:14.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/api/
--rw-r--r--   0 dev        (501) staff       (20)    14627 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/api/ship_api.py
--rw-r--r--   0 dev        (501) staff       (20)      136 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/api/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)     3819 2019-09-11 19:30:25.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/exceptions.py
--rw-r--r--   0 dev        (501) staff       (20)    26706 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/api_client.py
--rw-r--r--   0 dev        (501) staff       (20)    12529 2019-09-11 19:30:28.000000 nomad_pilot_cli-1.8.0/nomad_pilot_cli/rest_bak.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/
+-rw-r--r--   0 dev        (501) staff       (20)      381 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/PKG-INFO
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      381 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)     1134 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)       67 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 dev        (501) staff       (20)       21 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/dependency_links.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/test/
+-rw-r--r--   0 dev        (501) staff       (20)     1079 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_api_response_connector_response.py
+-rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_package.py
+-rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_address.py
+-rw-r--r--   0 dev        (501) staff       (20)      921 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_dimension.py
+-rw-r--r--   0 dev        (501) staff       (20)     1105 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/test/test_ship_api.py
+-rw-r--r--   0 dev        (501) staff       (20)      939 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_api_response.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/test/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)      905 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_goldjet.py
+-rw-r--r--   0 dev        (501) staff       (20)      973 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_api_response_data.py
+-rw-r--r--   0 dev        (501) staff       (20)      939 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/test/test_package_item.py
+-rw-r--r--   0 dev        (501) staff       (20)     3185 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/README.md
+-rw-r--r--   0 dev        (501) staff       (20)     1083 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/setup.py
+-rw-r--r--   0 dev        (501) staff       (20)       38 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/
+-rw-r--r--   0 dev        (501) staff       (20)     9936 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/configuration.py
+-rw-r--r--   0 dev        (501) staff       (20)     6161 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/swagger_validator.py
+-rw-r--r--   0 dev        (501) staff       (20)     9598 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/append_alibaba_headers.py
+-rw-r--r--   0 dev        (501) staff       (20)    12815 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/rest.py
+-rw-r--r--   0 dev        (501) staff       (20)     1372 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/
+-rw-r--r--   0 dev        (501) staff       (20)    22852 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/package.py
+-rw-r--r--   0 dev        (501) staff       (20)    13178 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/address.py
+-rw-r--r--   0 dev        (501) staff       (20)    13110 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/package_item.py
+-rw-r--r--   0 dev        (501) staff       (20)    10903 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response_connector_response.py
+-rw-r--r--   0 dev        (501) staff       (20)      880 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)     8739 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response_data.py
+-rw-r--r--   0 dev        (501) staff       (20)     6169 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response.py
+-rw-r--r--   0 dev        (501) staff       (20)     3071 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/goldjet.py
+-rw-r--r--   0 dev        (501) staff       (20)     4767 2019-09-12 09:00:48.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/dimension.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2019-09-12 09:02:33.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/api/
+-rw-r--r--   0 dev        (501) staff       (20)    14627 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/api/ship_api.py
+-rw-r--r--   0 dev        (501) staff       (20)      136 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/api/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)     3819 2019-09-12 09:00:49.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/exceptions.py
+-rw-r--r--   0 dev        (501) staff       (20)    26706 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/api_client.py
+-rw-r--r--   0 dev        (501) staff       (20)    12529 2019-09-12 09:00:53.000000 nomad_pilot_cli-1.9.0/nomad_pilot_cli/rest_bak.py
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli.egg-info/SOURCES.txt` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_api_response_connector_response.py` & `nomad_pilot_cli-1.9.0/test/test_api_response_connector_response.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_package.py` & `nomad_pilot_cli-1.9.0/test/test_package.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_address.py` & `nomad_pilot_cli-1.9.0/test/test_address.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_dimension.py` & `nomad_pilot_cli-1.9.0/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_ship_api.py` & `nomad_pilot_cli-1.9.0/test/test_ship_api.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_api_response.py` & `nomad_pilot_cli-1.9.0/test/test_api_response.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_goldjet.py` & `nomad_pilot_cli-1.9.0/test/test_goldjet.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_api_response_data.py` & `nomad_pilot_cli-1.9.0/test/test_api_response_data.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/test/test_package_item.py` & `nomad_pilot_cli-1.9.0/test/test_package_item.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/README.md` & `nomad_pilot_cli-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # nomad_pilot_cli
 This is the API descriptor for the Nomad Pilot API, responsible for shipping and logistics processing.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.8.0
+- Package version: 1.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `nomad_pilot_cli-1.8.0/setup.py` & `nomad_pilot_cli-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "nomad_pilot_cli"
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/configuration.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.8.0".\
+               "SDK Package Version: 1.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/swagger_validator.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/swagger_validator.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/append_alibaba_headers.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/append_alibaba_headers.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/rest.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/rest.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/__init__.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: paul@samarkand.global
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 # import apis into sdk package
 from nomad_pilot_cli.api.ship_api import ShipApi
 
 # import ApiClient
 from nomad_pilot_cli.api_client import ApiClient
 from nomad_pilot_cli.configuration import Configuration
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/package.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/package.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/address.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/address.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/package_item.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/package_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,35 +41,37 @@
         'brand': 'str',
         'quantity_uom': 'str',
         'hs_code': 'str',
         'country_of_origin': 'str',
         'goldjet': 'Goldjet',
         'gross_weight': 'float',
         'net_weight': 'float',
-        'customs_unit_code': 'str'
+        'customs_unit_code': 'str',
+        'spec': 'str'
     }
 
     attribute_map = {
         'name': 'name',
-        'name_cn': 'name_cn',
+        'name_cn': 'nameCn',
         'barcode': 'barcode',
         'sku_number': 'skuNumber',
         'quantity': 'quantity',
         'price': 'price',
         'brand': 'brand',
         'quantity_uom': 'quantityUom',
         'hs_code': 'hsCode',
         'country_of_origin': 'countryOfOrigin',
         'goldjet': 'goldjet',
         'gross_weight': 'gross_weight',
         'net_weight': 'net_weight',
-        'customs_unit_code': 'customs_unit_code'
+        'customs_unit_code': 'customs_unit_code',
+        'spec': 'spec'
     }
 
-    def __init__(self, name=None, name_cn=None, barcode=None, sku_number=None, quantity=None, price=None, brand=None, quantity_uom=None, hs_code=None, country_of_origin=None, goldjet=None, gross_weight=None, net_weight=None, customs_unit_code=None):  # noqa: E501
+    def __init__(self, name=None, name_cn=None, barcode=None, sku_number=None, quantity=None, price=None, brand=None, quantity_uom=None, hs_code=None, country_of_origin=None, goldjet=None, gross_weight=None, net_weight=None, customs_unit_code=None, spec=None):  # noqa: E501
         """PackageItem - a model defined in OpenAPI"""  # noqa: E501
 
         self._name = None
         self._name_cn = None
         self._barcode = None
         self._sku_number = None
         self._quantity = None
@@ -78,14 +80,15 @@
         self._quantity_uom = None
         self._hs_code = None
         self._country_of_origin = None
         self._goldjet = None
         self._gross_weight = None
         self._net_weight = None
         self._customs_unit_code = None
+        self._spec = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
         if name_cn is not None:
             self.name_cn = name_cn
         if barcode is not None:
@@ -108,14 +111,16 @@
             self.goldjet = goldjet
         if gross_weight is not None:
             self.gross_weight = gross_weight
         if net_weight is not None:
             self.net_weight = net_weight
         if customs_unit_code is not None:
             self.customs_unit_code = customs_unit_code
+        if spec is not None:
+            self.spec = spec
 
     @property
     def name(self):
         """Gets the name of this PackageItem.  # noqa: E501
 
 
         :return: The name of this PackageItem.  # noqa: E501
@@ -411,14 +416,37 @@
 
         :param customs_unit_code: The customs_unit_code of this PackageItem.  # noqa: E501
         :type: str
         """
 
         self._customs_unit_code = customs_unit_code
 
+    @property
+    def spec(self):
+        """Gets the spec of this PackageItem.  # noqa: E501
+
+        The spec of current product.  # noqa: E501
+
+        :return: The spec of this PackageItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._spec
+
+    @spec.setter
+    def spec(self, spec):
+        """Sets the spec of this PackageItem.
+
+        The spec of current product.  # noqa: E501
+
+        :param spec: The spec of this PackageItem.  # noqa: E501
+        :type: str
+        """
+
+        self._spec = spec
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response_connector_response.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response_connector_response.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/__init__.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response_data.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response_data.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/api_response.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/api_response.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/goldjet.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/goldjet.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/models/dimension.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/models/dimension.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/api/ship_api.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/api/ship_api.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/exceptions.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/api_client.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.9.0/python'
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

### Comparing `nomad_pilot_cli-1.8.0/nomad_pilot_cli/rest_bak.py` & `nomad_pilot_cli-1.9.0/nomad_pilot_cli/rest_bak.py`

 * *Files identical despite different names*

