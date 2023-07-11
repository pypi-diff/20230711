# Comparing `tmp/papertronics-sdk-0.0.18.tar.gz` & `tmp/papertronics-sdk-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.18.tar", last modified: Mon Jul 10 14:10:53 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.19.tar", last modified: Tue Jul 11 08:59:12 2023, max compression
```

## Comparing `papertronics-sdk-0.0.18.tar` & `papertronics-sdk-0.0.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.18/LICENSE
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      975 2023-07-10 08:17:39.000000 papertronics-sdk-0.0.18/README.md
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.18/papertronics_sdk/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5319 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/admin_client.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1469 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/base_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/StatusException.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/config.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/database.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/generic.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/station_protocol.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9139 2023-07-10 12:23:51.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/user_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/requires.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/zip-safe
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/pyproject.toml
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.247716 papertronics-sdk-0.0.19/papertronics_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/StatusException.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/models/station_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/papertronics_sdk/lab/user_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:59:12.247716 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:59:12.000000 papertronics-sdk-0.0.19/papertronics_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 08:59:00.000000 papertronics-sdk-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 08:59:12.251716 papertronics-sdk-0.0.19/setup.cfg
```

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/admin_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,89 +8,89 @@
 
 
 class AdminLabClient(BaseClient):
 
     def __init__(self, url, token):
         super().__init__(url, token)
 
-    async def login_user(self, user_id: uuid.UUID) -> str:
+    def login_user(self, user_id: uuid.UUID) -> str:
         response = self.post(f"{self.url}/admin/auth/token?user_id={user_id}",
                              headers={"Authorization": f"Bearer {self.token}"})
         return response.json().get("access_token")
 
-    async def get_users(self, user_id: Optional[uuid.UUID] = None) -> Union[List[UserModel], UserModel]:
+    def get_users(self, user_id: Optional[uuid.UUID] = None) -> Union[List[UserModel], UserModel]:
         response = self.get(f"{self.url}/admin/user?user_id={user_id}",
                             headers={"Authorization": f"Bearer {self.token}"})
         response_dict = response.json()
         if type(response_dict) == list:
             return [UserModel.parse_obj(r) for r in response_dict]
         else:
             return UserModel.parse_obj(response_dict)
 
-    async def add_user(self, add_user_request: UserRequest) -> UserModel:
+    def add_user(self, add_user_request: UserRequest) -> UserModel:
         response = self.post(f"{self.url}/admin/user", json=add_user_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return UserModel.parse_obj(response.json())
 
-    async def delete_user(self, user_id: uuid.UUID):
+    def delete_user(self, user_id: uuid.UUID):
         self.delete(f"{self.url}/admin/user?user_id={user_id}",
                     headers={"Authorization": f"Bearer {self.token}"})
 
-    async def update_user(self, user_id: uuid.UUID, add_user_request: UserRequest) -> UserModel:
+    def update_user(self, user_id: uuid.UUID, add_user_request: UserRequest) -> UserModel:
         response = self.post(f"{self.url}/admin/user/update?user_id={user_id}", json=add_user_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return UserModel.parse_obj(response.json())
 
-    async def get_protocol(self, protocol_id: Optional[uuid.UUID] = None) -> Union[ProtocolModel, List[ProtocolModel]]:
+    def get_protocol(self, protocol_id: Optional[uuid.UUID] = None) -> Union[ProtocolModel, List[ProtocolModel]]:
         response = self.get(f"{self.url}/admin/protocol?protocol_id={protocol_id}",
                             headers={"Authorization": f"Bearer {self.token}"})
         response_dict = response.json()
         if type(response_dict) == list:
             return [ProtocolModel.parse_obj(r) for r in response_dict]
         else:
             return ProtocolModel.parse_obj(response_dict)
 
-    async def link_protocol(self, protocol_id: uuid.UUID, user_id: uuid.UUID) -> ProtocolLinkModel:
+    def link_protocol(self, protocol_id: uuid.UUID, user_id: uuid.UUID) -> ProtocolLinkModel:
         response = self.post(f"{self.url}/admin/protocol/link?protocol_id={protocol_id}&user_id={user_id}",
                              headers={"Authorization": f"Bearer {self.token}"})
         return ProtocolLinkModel.parse_obj(response.json())
 
-    async def remove_link_protocol(self, protocol_link_id: uuid.UUID):
+    def remove_link_protocol(self, protocol_link_id: uuid.UUID):
         self.delete(f"{self.url}/admin/protocol/link?protocol_link_id={protocol_link_id}",
                     headers={"Authorization": f"Bearer {self.token}"})
 
-    async def get_devices(self, device_id: Optional[uuid.UUID] = None) -> Union[List[DeviceModel], DeviceModel]:
+    def get_devices(self, device_id: Optional[uuid.UUID] = None) -> Union[List[DeviceModel], DeviceModel]:
         response = self.get(f"{self.url}/admin/device?device_id={device_id}",
                             headers={"Authorization": f"Bearer {self.token}"})
         response_dict = response.json()
         if type(response_dict) == list:
             return [DeviceModel.parse_obj(r) for r in response_dict]
         else:
             return DeviceModel.parse_obj(response_dict)
 
-    async def add_device(self, add_device_request: DeviceRequest) -> DeviceModel:
+    def add_device(self, add_device_request: DeviceRequest) -> DeviceModel:
         response = self.post(f"{self.url}/admin/device", json=add_device_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return DeviceModel.parse_obj(response.json())
 
-    async def delete_device(self, device_id: uuid.UUID):
+    def delete_device(self, device_id: uuid.UUID):
         self.delete(f"{self.url}/admin/device?device_id={device_id}",
                     headers={"Authorization": f"Bearer {self.token}"})
 
-    async def update_device(self, device_id: uuid.UUID, add_device_request: DeviceRequest) -> DeviceModel:
+    def update_device(self, device_id: uuid.UUID, add_device_request: DeviceRequest) -> DeviceModel:
         response = self.post(f"{self.url}/admin/device/update?device_id={device_id}", json=add_device_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return DeviceModel.parse_obj(response.json())
 
-    async def link_device(self, device_id: uuid.UUID, user_id: uuid.UUID) -> DeviceLinkModel:
+    def link_device(self, device_id: uuid.UUID, user_id: uuid.UUID) -> DeviceLinkModel:
         response = self.post(f"{self.url}/admin/device/link?device_id={device_id}&user_id={user_id}",
                              headers={"Authorization": f"Bearer {self.token}"})
         return DeviceLinkModel.parse_obj(response.json())
 
-    async def remove_link_device(self, device_link_id: uuid.UUID):
+    def remove_link_device(self, device_link_id: uuid.UUID):
         self.delete(f"{self.url}/admin/device/link?device_link_id={device_link_id}",
                     headers={"Authorization": f"Bearer {self.token}"})
 
-    async def get_device_statistics(self, device_id: Optional[uuid.UUID] = None) -> List[DeviceStatisticModel]:
+    def get_device_statistics(self, device_id: Optional[uuid.UUID] = None) -> List[DeviceStatisticModel]:
         response = self.get(f"{self.url}/admin/device/statistic?device_id={device_id}",
                             headers={"Authorization": f"Bearer {self.token}"})
         return [DeviceStatisticModel.parse_obj(r) for r in response.json()]
```

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/base_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 
 class BaseClient:
 
     def __init__(self, url, token=None):
         self.url = url
         self.token = token
+        try:
+            response = self.get(f"{self.url}")
+            if response.status_code != 200:
+                raise Exception(response.status_code)
+        except Exception as e:
+            raise Exception(f"could not connect to {url}: {e}")
 
     def http_request(self, func):
         def wrap(path, **kwargs):
             if self.token is None:
                 raise Exception("Client is not Authenticated")
 
             url = f"{self.url}{path}"
```

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.19/papertronics_sdk/lab/user_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
                              headers={"Authorization": f"Bearer {self.token}"})
         self.token = response.json().get("access_token")
         return self.token
 
     def download_data(self):
         return "not implemented"
 
-    async def download_image(self,
+    def download_image(self,
                              blob_name: str):
         return "not implemented"
 
-    async def get_device_info(self) -> DeviceModel:
+    def get_device_info(self) -> DeviceModel:
         response = self.get(f"{self.url}/device",
                             headers={"Authorization": f"Bearer {self.token}"})
         return DeviceModel.parse_obj(response.json())
 
-    async def get_devices(self) -> List[DeviceModel]:
+    def get_devices(self) -> List[DeviceModel]:
         response = self.get(f"{self.url}/device/all",
                             headers={"Authorization": f"Bearer {self.token}"})
         return [DeviceModel.parse_obj(r) for r in response.json()]
 
-    async def get_user_info(self) -> UserModel:
+    def get_user_info(self) -> UserModel:
         response = self.get(f"{self.url}/user",
                             headers={"Authorization": f"Bearer {self.token}"})
         return UserModel.parse_obj(response.json())
 
     def store_protocol(self, protocol_request: SaveProtocolRequest) -> ProtocolModel:
         response = self.post(f"{self.url}/protocol",
                              headers={"Authorization": f"Bearer {self.token}"},
@@ -97,15 +97,15 @@
             return ProtocolTestResponse.parse_obj(response.json())
 
     def invalidate_protocol(self, protocol_id: uuid.UUID) -> ProtocolModel:
         response = self.delete(f"{self.url}/protocol?protocol_id={protocol_id}",
                                headers={"Authorization": f"Bearer {self.token}"})
         return ProtocolModel.parse_obj(response.json())
 
-    async def start_experiment(self, request: ExperimentStartRequest) -> ExperimentModel:
+    def start_experiment(self, request: ExperimentStartRequest) -> ExperimentModel:
         response = self.post(f"{self.url}/experiment/start",
                              headers={"Authorization": f"Bearer {self.token}"},
                              json=request.dict())
         return ExperimentModel.parse_obj(response.json())
 
     def cancel_experiment(self,
                           experiment_id: uuid.UUID):
```

### Comparing `papertronics-sdk-0.0.18/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.19/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.18/setup.cfg` & `papertronics-sdk-0.0.19/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.18
+version = 0.0.19
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

