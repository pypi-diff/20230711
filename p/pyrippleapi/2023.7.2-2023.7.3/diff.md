# Comparing `tmp/pyrippleapi-2023.7.2.tar.gz` & `tmp/pyrippleapi-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2023.7.2.tar", last modified: Tue Jul 11 12:44:17 2023, max compression
+gzip compressed data, was "pyrippleapi-2023.7.3.tar", last modified: Tue Jul 11 13:50:54 2023, max compression
```

## Comparing `pyrippleapi-2023.7.2.tar` & `pyrippleapi-2023.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.307006 pyrippleapi-2023.7.2/
--rw-rw-rw-   0        0        0      418 2023-07-11 12:44:17.308005 pyrippleapi-2023.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.2/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-11 12:44:17.312007 pyrippleapi-2023.7.2/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-07-11 12:43:00.000000 pyrippleapi-2023.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.251990 pyrippleapi-2023.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.273005 pyrippleapi-2023.7.2/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.2/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-07-11 12:39:48.000000 pyrippleapi-2023.7.2/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.2/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5671 2023-07-11 12:42:42.000000 pyrippleapi-2023.7.2/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:44:17.305007 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 12:44:17.000000 pyrippleapi-2023.7.2/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 13:50:54.002374 pyrippleapi-2023.7.3/
+-rw-rw-rw-   0        0        0      418 2023-07-11 13:50:54.002374 pyrippleapi-2023.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.3/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-11 13:50:54.005376 pyrippleapi-2023.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-11 13:50:12.000000 pyrippleapi-2023.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:50:53.952379 pyrippleapi-2023.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 13:50:53.976376 pyrippleapi-2023.7.3/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.3/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-07-11 12:39:48.000000 pyrippleapi-2023.7.3/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.3/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5738 2023-07-11 13:50:05.000000 pyrippleapi-2023.7.3/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:50:54.000375 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2023.7.2/setup.py` & `pyrippleapi-2023.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2023.7.2",
+    version="2023.7.3",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2023.7.2/src/pyrippleapi/api.py` & `pyrippleapi-2023.7.3/src/pyrippleapi/api.py`

 * *Files identical despite different names*

### Comparing `pyrippleapi-2023.7.2/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2023.7.3/src/pyrippleapi/generation_asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,44 +100,52 @@
     def latest_telemetry(self) -> dict:
         return self._latest_telemetry
 
     @property
     def generation_data(self) -> dict[str:str]:
         return self._generation_data
 
-    def update_asset_info(self, data) -> None:
+    async def update_asset_info(self, data) -> None:
         self._status = data["status"]
         self._member_capacity = data["member_capacity"]
         self._member_capacity_units = data["member_capacity_units"]
         self._member_expected_annual_generation = data[
             "member_expected_annual_generation"
         ]
         self._member_expected_annual_generation_units = data[
             "member_expected_annual_generation_units"
         ]
 
-    def get_telemetry(self, data) -> None:
+    async def get_telemetry(self, data) -> None:
         self._latest_telemetry = data["latest_telemetry"]
 
         self._latest_telemetry["timestamp"] = datetime.datetime.strptime(
             self._latest_telemetry["timestamp"],
             "%Y-%m-%dT%H:%M:%SZ",
         ).strftime("%Y/%m/%d %H:%M:%S")
 
-    def get_generation(self, data) -> None:
-        self._generation_data["latest"] = data["latest"]
-        self._generation_data["today"] = data["today"]
-        self._generation_data["yesterday"] = data["yesterday"]
-        self._generation_data["this_week"] = data["this_week"]
-        self._generation_data["last_week"] = data["last_week"]
-        self._generation_data["this_month"] = data["this_month"]
-        self._generation_data["last_month"] = data["last_month"]
-        self._generation_data["this_year"] = data["this_year"]
-        self._generation_data["last_year"] = data["last_year"]
-        self._generation_data["total"] = data["total"]
+    async def get_generation(self, data) -> None:
+        for time_scale in [
+            "today",
+            "yesterday",
+            "this_week",
+            "last_week",
+            "this_month",
+            "last_month",
+            "this_year",
+            "last_year",
+            "total",
+        ]:
+            self._generation_data[time_scale + "_earned"] = data[time_scale]["earned"]
+            self._generation_data[time_scale + "_generated"] = data[time_scale][
+                "generated"
+            ]
+
+        self._generation_data["latest_earned"] = data["latest"]["estimated_savings"]
+        self._generation_data["latest_generated"] = data["latest"]["generation"]
 
     async def update_data(
         self,
     ) -> dict:
         """
         Calls the Ripple api to update the properties and then returns the raw response dict, the formatted dict from
         normalise_properties and any new api tokens if they have changed
@@ -159,15 +167,15 @@
         generation_data = {}
 
         for asset in data:
             if asset["name"] == self._name:
                 generation_data = asset
                 break
 
-        self.update_asset_info(generation_data)
-        self.get_telemetry(generation_data["generation"])
-        self.get_generation(generation_data["generation"])
+        await self.update_asset_info(generation_data)
+        await self.get_telemetry(generation_data["generation"])
+        await self.get_generation(generation_data["generation"])
 
         return {
             "telemetry": self._latest_telemetry,
             "generation_data": self._generation_data,
         }
```

