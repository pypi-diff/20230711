# Comparing `tmp/sekm-pump-1.0.0.tar.gz` & `tmp/sekm-pump-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekm-pump-1.0.0.tar", last modified: Thu Apr 20 18:21:35 2023, max compression
+gzip compressed data, was "sekm-pump-1.0.0.9.tar", last modified: Tue Jul 11 07:52:57 2023, max compression
```

## Comparing `sekm-pump-1.0.0.tar` & `sekm-pump-1.0.0.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.080248 sekm-pump-1.0.0/
--rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sekm-pump-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    18878 2023-04-20 18:21:35.080248 sekm-pump-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4752 2023-04-20 18:15:16.000000 sekm-pump-1.0.0/README.md
--rw-rw-rw-   0        0        0      859 2023-04-20 18:15:16.000000 sekm-pump-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.060117 sekm-pump-1.0.0/sekm_pump/
--rw-rw-rw-   0        0        0      508 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.075741 sekm-pump-1.0.0/sekm_pump/api/
--rw-rw-rw-   0        0        0      134 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/api/__init__.py
--rw-rw-rw-   0        0        0    15052 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/api/public_api.py
--rw-rw-rw-   0        0        0    25008 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/api_client.py
--rw-rw-rw-   0        0        0     8208 2023-04-20 17:55:17.000000 sekm-pump-1.0.0/sekm_pump/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.080248 sekm-pump-1.0.0/sekm_pump/models/
--rw-rw-rw-   0        0        0      319 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/models/__init__.py
--rw-rw-rw-   0        0        0    12980 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/sekm_pump/rest.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.060117 sekm-pump-1.0.0/sekm_pump.egg-info/
--rw-rw-rw-   0        0        0    18878 2023-04-20 18:21:35.000000 sekm-pump-1.0.0/sekm_pump.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-04-20 18:21:35.000000 sekm-pump-1.0.0/sekm_pump.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 18:21:35.000000 sekm-pump-1.0.0/sekm_pump.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 18:21:35.000000 sekm-pump-1.0.0/sekm_pump.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 18:21:35.000000 sekm-pump-1.0.0/sekm_pump.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 18:21:35.080248 sekm-pump-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:21:35.080248 sekm-pump-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-19 12:27:47.000000 sekm-pump-1.0.0/test/test_public_api.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:57.015493 sekm-pump-1.0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sekm-pump-1.0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    19032 2023-07-11 07:52:57.015493 sekm-pump-1.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4902 2023-07-11 07:51:25.000000 sekm-pump-1.0.0.9/README.md
+-rw-rw-rw-   0        0        0      863 2023-07-11 07:43:49.000000 sekm-pump-1.0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:56.979035 sekm-pump-1.0.0.9/sekm_pump/
+-rw-rw-rw-   0        0        0      569 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/sekm_pump/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:56.994655 sekm-pump-1.0.0.9/sekm_pump/api/
+-rw-rw-rw-   0        0        0      134 2023-04-19 12:27:47.000000 sekm-pump-1.0.0.9/sekm_pump/api/__init__.py
+-rw-rw-rw-   0        0        0    15212 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/sekm_pump/api/public_api.py
+-rw-rw-rw-   0        0        0    25008 2023-04-19 12:27:47.000000 sekm-pump-1.0.0.9/sekm_pump/api_client.py
+-rw-rw-rw-   0        0        0     8208 2023-07-11 07:51:25.000000 sekm-pump-1.0.0.9/sekm_pump/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:56.994655 sekm-pump-1.0.0.9/sekm_pump/models/
+-rw-rw-rw-   0        0        0      380 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/sekm_pump/models/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/sekm_pump/models/three_state_type.py
+-rw-rw-rw-   0        0        0    12980 2023-04-19 12:27:47.000000 sekm-pump-1.0.0.9/sekm_pump/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:56.994655 sekm-pump-1.0.0.9/sekm_pump.egg-info/
+-rw-rw-rw-   0        0        0    19032 2023-07-11 07:52:56.000000 sekm-pump-1.0.0.9/sekm_pump.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-07-11 07:52:56.000000 sekm-pump-1.0.0.9/sekm_pump.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 07:52:56.000000 sekm-pump-1.0.0.9/sekm_pump.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-11 07:52:56.000000 sekm-pump-1.0.0.9/sekm_pump.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-11 07:52:56.000000 sekm-pump-1.0.0.9/sekm_pump.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 07:52:57.015493 sekm-pump-1.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-04-19 12:27:47.000000 sekm-pump-1.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:52:57.015493 sekm-pump-1.0.0.9/test/
+-rw-rw-rw-   0        0        0       15 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/test/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-04-19 12:27:47.000000 sekm-pump-1.0.0.9/test/test_public_api.py
+-rw-rw-rw-   0        0        0      873 2023-07-10 19:27:36.000000 sekm-pump-1.0.0.9/test/test_three_state_type.py
```

### Comparing `sekm-pump-1.0.0/LICENSE` & `sekm-pump-1.0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sekm-pump-1.0.0/PKG-INFO` & `sekm-pump-1.0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekm-pump
-Version: 1.0.0
+Version: 1.0.0.9
 Summary: SYSNET SEKM Pump REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,23 +223,22 @@
 
 # sekm-pump
 SEKM analytical data API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0.009
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
-
 If the python package is hosted on PyPi, you can install directly
 
 ```sh
 pip install sekm-pump
 ```
 
 Then import the package:
@@ -263,18 +262,18 @@
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 out_format = 'out_format_example' # str | Formát výstupního datasetu
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to false)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to false)
-excluded = False # bool | Vyloučené lokality (optional) (default to false)
-indications = False # bool | Indicie (optional) (default to false)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá analytická data lokalit
@@ -285,24 +284,21 @@
 
 # Configure API key authorization: apiKey
 configuration = sekm_pump.Configuration()
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
-# Configure endpoint
-configuration.host = 'YOUR_ENDPOINT'
-
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 geom = 'geom_example' # str | geometrie vrstvy (bod/polygon)
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to False)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to False)
-excluded = False # bool | Vyloučené lokality (optional) (default to False)
-indications = False # bool | Indicie (optional) (default to False)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá vrstvu lokalit v GeoJson
@@ -328,14 +324,20 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *PublicApi* | [**get_location**](docs/PublicApi.md#get_location) | **GET** /location/{out_format} | Získá analytická data lokalit
 *PublicApi* | [**get_location_geo_json**](docs/PublicApi.md#get_location_geo_json) | **GET** /location_layer/{geom} | Získá vrstvu lokalit v GeoJson
 *PublicApi* | [**get_status**](docs/PublicApi.md#get_status) | **GET** /status | Získá status klienta
 
+## Documentation For Models
+
+ - [ThreeStateType](docs/ThreeStateType.md)
+
+## Documentation For Authorization
+
 
 ## apiKey
 
 - **Type**: API key
 - **API key parameter name**: X-API-KEY
 - **Location**: HTTP header
```

### Comparing `sekm-pump-1.0.0/README.md` & `sekm-pump-1.0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # sekm-pump
 SEKM analytical data API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0.009
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
-
 If the python package is hosted on PyPi, you can install directly
 
 ```sh
 pip install sekm-pump
 ```
 
 Then import the package:
@@ -40,18 +39,18 @@
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 out_format = 'out_format_example' # str | Formát výstupního datasetu
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to false)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to false)
-excluded = False # bool | Vyloučené lokality (optional) (default to false)
-indications = False # bool | Indicie (optional) (default to false)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá analytická data lokalit
@@ -62,24 +61,21 @@
 
 # Configure API key authorization: apiKey
 configuration = sekm_pump.Configuration()
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
-# Configure endpoint
-configuration.host = 'YOUR_ENDPOINT'
-
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 geom = 'geom_example' # str | geometrie vrstvy (bod/polygon)
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to False)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to False)
-excluded = False # bool | Vyloučené lokality (optional) (default to False)
-indications = False # bool | Indicie (optional) (default to False)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá vrstvu lokalit v GeoJson
@@ -105,14 +101,20 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *PublicApi* | [**get_location**](docs/PublicApi.md#get_location) | **GET** /location/{out_format} | Získá analytická data lokalit
 *PublicApi* | [**get_location_geo_json**](docs/PublicApi.md#get_location_geo_json) | **GET** /location_layer/{geom} | Získá vrstvu lokalit v GeoJson
 *PublicApi* | [**get_status**](docs/PublicApi.md#get_status) | **GET** /status | Získá status klienta
 
+## Documentation For Models
+
+ - [ThreeStateType](docs/ThreeStateType.md)
+
+## Documentation For Authorization
+
 
 ## apiKey
 
 - **Type**: API key
 - **API key parameter name**: X-API-KEY
 - **Location**: HTTP header
```

### Comparing `sekm-pump-1.0.0/pyproject.toml` & `sekm-pump-1.0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sekm-pump"
-version = "1.0.0"
+version = "1.0.0.009"
 authors = [
   { name="Radim Jaeger", email="rjaeger@sysnet.cz" },
 ]
 description = "SYSNET SEKM Pump REST API client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `sekm-pump-1.0.0/sekm_pump/api/public_api.py` & `sekm-pump-1.0.0.9/sekm_pump/api/public_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,18 +39,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_location(out_format, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str out_format: Formát výstupního datasetu (required)
-        :param bool a3p4: Lokality s prioritou pro průzkum a pro sanaci
-        :param bool sa: Lokality poškozené Sovětskou armádou
-        :param bool excluded: Vyloučené lokality
-        :param bool indications: Indicie
+        :param ThreeStateType a3p4: Lokality s prioritou pro průzkum a pro sanaci
+        :param ThreeStateType sa: Lokality poškozené Sovětskou armádou
+        :param ThreeStateType excluded: Vyloučené lokality
+        :param ThreeStateType indications: Indicie
         :param str name: Název lokality
         :param str territory: katastrální území (cadastral territory)
         :param str region: Kraj (VÚSC)
         :param str municipality: Obec s rozšířenou působností (ORP)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
@@ -69,18 +69,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_location_with_http_info(out_format, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str out_format: Formát výstupního datasetu (required)
-        :param bool a3p4: Lokality s prioritou pro průzkum a pro sanaci
-        :param bool sa: Lokality poškozené Sovětskou armádou
-        :param bool excluded: Vyloučené lokality
-        :param bool indications: Indicie
+        :param ThreeStateType a3p4: Lokality s prioritou pro průzkum a pro sanaci
+        :param ThreeStateType sa: Lokality poškozené Sovětskou armádou
+        :param ThreeStateType excluded: Vyloučené lokality
+        :param ThreeStateType indications: Indicie
         :param str name: Název lokality
         :param str territory: katastrální území (cadastral territory)
         :param str region: Kraj (VÚSC)
         :param str municipality: Obec s rozšířenou působností (ORP)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
@@ -166,18 +166,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_location_geo_json(geom, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str geom: geometrie vrstvy (bod/polygon) (required)
-        :param bool a3p4: Lokality s prioritou pro průzkum a pro sanaci
-        :param bool sa: Lokality poškozené Sovětskou armádou
-        :param bool excluded: Vyloučené lokality
-        :param bool indications: Indicie
+        :param ThreeStateType a3p4: Lokality s prioritou pro průzkum a pro sanaci
+        :param ThreeStateType sa: Lokality poškozené Sovětskou armádou
+        :param ThreeStateType excluded: Vyloučené lokality
+        :param ThreeStateType indications: Indicie
         :param str name: Název lokality
         :param str territory: katastrální území (cadastral territory)
         :param str region: Kraj (VÚSC)
         :param str municipality: Obec s rozšířenou působností (ORP)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
@@ -196,18 +196,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_location_geo_json_with_http_info(geom, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str geom: geometrie vrstvy (bod/polygon) (required)
-        :param bool a3p4: Lokality s prioritou pro průzkum a pro sanaci
-        :param bool sa: Lokality poškozené Sovětskou armádou
-        :param bool excluded: Vyloučené lokality
-        :param bool indications: Indicie
+        :param ThreeStateType a3p4: Lokality s prioritou pro průzkum a pro sanaci
+        :param ThreeStateType sa: Lokality poškozené Sovětskou armádou
+        :param ThreeStateType excluded: Vyloučené lokality
+        :param ThreeStateType indications: Indicie
         :param str name: Název lokality
         :param str territory: katastrální území (cadastral territory)
         :param str region: Kraj (VÚSC)
         :param str municipality: Obec s rozšířenou působností (ORP)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
```

### Comparing `sekm-pump-1.0.0/sekm_pump/api_client.py` & `sekm-pump-1.0.0.9/sekm_pump/api_client.py`

 * *Files identical despite different names*

### Comparing `sekm-pump-1.0.0/sekm_pump/configuration.py` & `sekm-pump-1.0.0.9/sekm_pump/configuration.py`

 * *Files identical despite different names*

### Comparing `sekm-pump-1.0.0/sekm_pump/rest.py` & `sekm-pump-1.0.0.9/sekm_pump/rest.py`

 * *Files identical despite different names*

### Comparing `sekm-pump-1.0.0/sekm_pump.egg-info/PKG-INFO` & `sekm-pump-1.0.0.9/sekm_pump.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekm-pump
-Version: 1.0.0
+Version: 1.0.0.9
 Summary: SYSNET SEKM Pump REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,23 +223,22 @@
 
 # sekm-pump
 SEKM analytical data API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0.009
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
-
 If the python package is hosted on PyPi, you can install directly
 
 ```sh
 pip install sekm-pump
 ```
 
 Then import the package:
@@ -263,18 +262,18 @@
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 out_format = 'out_format_example' # str | Formát výstupního datasetu
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to false)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to false)
-excluded = False # bool | Vyloučené lokality (optional) (default to false)
-indications = False # bool | Indicie (optional) (default to false)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá analytická data lokalit
@@ -285,24 +284,21 @@
 
 # Configure API key authorization: apiKey
 configuration = sekm_pump.Configuration()
 configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['X-API-KEY'] = 'Bearer'
 
-# Configure endpoint
-configuration.host = 'YOUR_ENDPOINT'
-
 # create an instance of the API class
 api_instance = sekm_pump.PublicApi(sekm_pump.ApiClient(configuration))
 geom = 'geom_example' # str | geometrie vrstvy (bod/polygon)
-a3p4 = False # bool | Lokality s prioritou pro průzkum a pro sanaci (optional) (default to False)
-sa = False # bool | Lokality poškozené Sovětskou armádou (optional) (default to False)
-excluded = False # bool | Vyloučené lokality (optional) (default to False)
-indications = False # bool | Indicie (optional) (default to False)
+a3p4 = sekm_pump.ThreeStateType() # ThreeStateType | Lokality s prioritou pro průzkum a pro sanaci (optional)
+sa = sekm_pump.ThreeStateType() # ThreeStateType | Lokality poškozené Sovětskou armádou (optional)
+excluded = sekm_pump.ThreeStateType() # ThreeStateType | Vyloučené lokality (optional)
+indications = sekm_pump.ThreeStateType() # ThreeStateType | Indicie (optional)
 name = 'name_example' # str | Název lokality (optional)
 territory = 'territory_example' # str | katastrální území (cadastral territory) (optional)
 region = 'region_example' # str | Kraj (VÚSC) (optional)
 municipality = 'municipality_example' # str | Obec s rozšířenou působností (ORP) (optional)
 
 try:
     # Získá vrstvu lokalit v GeoJson
@@ -328,14 +324,20 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *PublicApi* | [**get_location**](docs/PublicApi.md#get_location) | **GET** /location/{out_format} | Získá analytická data lokalit
 *PublicApi* | [**get_location_geo_json**](docs/PublicApi.md#get_location_geo_json) | **GET** /location_layer/{geom} | Získá vrstvu lokalit v GeoJson
 *PublicApi* | [**get_status**](docs/PublicApi.md#get_status) | **GET** /status | Získá status klienta
 
+## Documentation For Models
+
+ - [ThreeStateType](docs/ThreeStateType.md)
+
+## Documentation For Authorization
+
 
 ## apiKey
 
 - **Type**: API key
 - **API key parameter name**: X-API-KEY
 - **Location**: HTTP header
```

### Comparing `sekm-pump-1.0.0/setup.py` & `sekm-pump-1.0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sekm-pump-1.0.0/test/test_public_api.py` & `sekm-pump-1.0.0.9/test/test_public_api.py`

 * *Files identical despite different names*

