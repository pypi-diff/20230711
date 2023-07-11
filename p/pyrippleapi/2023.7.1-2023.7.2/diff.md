# Comparing `tmp/pyrippleapi-2023.7.1.tar.gz` & `tmp/pyrippleapi-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2023.7.1.tar", last modified: Tue Jul 11 12:20:23 2023, max compression
+gzip compressed data, was "pyrippleapi-2023.7.2.tar", last modified: Tue Jul 11 12:44:17 2023, max compression
```

## Comparing `pyrippleapi-2023.7.1.tar` & `pyrippleapi-2023.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.386056 pyrippleapi-2023.7.1/
--rw-rw-rw-   0        0        0      418 2023-07-11 12:20:23.386056 pyrippleapi-2023.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.1/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-11 12:20:23.395056 pyrippleapi-2023.7.1/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-07-11 12:19:20.000000 pyrippleapi-2023.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.326057 pyrippleapi-2023.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.346059 pyrippleapi-2023.7.1/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.1/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-07-11 12:19:13.000000 pyrippleapi-2023.7.1/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.1/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5032 2023-07-11 11:11:06.000000 pyrippleapi-2023.7.1/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.384057 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.307006 pyrippleapi-2023.7.2/
+-rw-rw-rw-   0        0        0      418 2023-07-11 12:44:17.308005 pyrippleapi-2023.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-11 12:44:17.312007 pyrippleapi-2023.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-11 12:43:00.000000 pyrippleapi-2023.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.251990 pyrippleapi-2023.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.273005 pyrippleapi-2023.7.2/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.2/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-07-11 12:39:48.000000 pyrippleapi-2023.7.2/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.2/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5671 2023-07-11 12:42:42.000000 pyrippleapi-2023.7.2/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.305007 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2023.7.1/setup.py` & `pyrippleapi-2023.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2023.7.1",
+    version="2023.7.2",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2023.7.1/src/pyrippleapi/api.py` & `pyrippleapi-2023.7.2/src/pyrippleapi/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,11 +78,11 @@
                 raise RippleConnectionError("Error sending request")
 
             response = await response.json()
 
             if "error" in response:
                 raise RippleAuthenticationError("Invalid API Key")
 
-            if len(response["generation_assets"] < 1):
+            if len(response["generation_assets"])<1:
                 raise RippleDevicesError("No generation assets found")
 
             return response
```

### Comparing `pyrippleapi-2023.7.1/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2023.7.2/src/pyrippleapi/generation_asset.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,26 @@
     get_generation:
         sets the latest generation data
     update_properties
         usees the RippleAPI object to call the ripple server and return the current properties of the device.
     """
 
     def __init__(
-        self, api: RippleAPI, data: dict[str : Union[str, int, bool, list]]
+        self, api: RippleAPI, data: dict[str : Union[str, int, bool, list]], email: str
     ) -> None:
         """
         Constructs an Ripple generation asset object representing the generation asset
 
         Parameters
         ----------
         api (RippleAPI):RippleAPI object used to call the Ripple API
         data (dict):Data returned from the Ripple API showing the details of the generation assets
         """
         self._api = api
+        self._email = email
         self._name = data["name"]
         self._type = data["type"]
         self._status = data["status"]
         self._member_capacity = data["member_capacity"]
         self._member_capacity_units = data["member_capacity_units"]
         self._member_expected_annual_generation = data[
             "member_expected_annual_generation"
@@ -48,14 +49,18 @@
         self._generation_units = data["generation"]["generation_unit"]
         self._estimated_savings_unit = "£"
 
         self._latest_telemetry = {}
         self._generation_data = {}
 
     @property
+    def email(self) -> str:
+        return self._email
+
+    @property
     def generation_unit(self) -> str:
         return self._generation_units
 
     @property
     def estimated_savings_unit(self) -> str:
         return self._estimated_savings_unit
 
@@ -95,14 +100,25 @@
     def latest_telemetry(self) -> dict:
         return self._latest_telemetry
 
     @property
     def generation_data(self) -> dict[str:str]:
         return self._generation_data
 
+    def update_asset_info(self, data) -> None:
+        self._status = data["status"]
+        self._member_capacity = data["member_capacity"]
+        self._member_capacity_units = data["member_capacity_units"]
+        self._member_expected_annual_generation = data[
+            "member_expected_annual_generation"
+        ]
+        self._member_expected_annual_generation_units = data[
+            "member_expected_annual_generation_units"
+        ]
+
     def get_telemetry(self, data) -> None:
         self._latest_telemetry = data["latest_telemetry"]
 
         self._latest_telemetry["timestamp"] = datetime.datetime.strptime(
             self._latest_telemetry["timestamp"],
             "%Y-%m-%dT%H:%M:%SZ",
         ).strftime("%Y/%m/%d %H:%M:%S")
@@ -140,17 +156,18 @@
         if self._name not in names:
             return {{"telemetry": {}}, {"generation_data": {}}}
 
         generation_data = {}
 
         for asset in data:
             if asset["name"] == self._name:
-                generation_data = asset["generation"]
+                generation_data = asset
                 break
 
-        self.get_telemetry(generation_data)
-        self.get_generation(generation_data)
+        self.update_asset_info(generation_data)
+        self.get_telemetry(generation_data["generation"])
+        self.get_generation(generation_data["generation"])
 
         return {
             "telemetry": self._latest_telemetry,
             "generation_data": self._generation_data,
         }
```

