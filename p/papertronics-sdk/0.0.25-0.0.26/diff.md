# Comparing `tmp/papertronics-sdk-0.0.25.tar.gz` & `tmp/papertronics-sdk-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.25.tar", last modified: Tue Jul 11 10:35:27 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.26.tar", last modified: Tue Jul 11 10:37:43 2023, max compression
```

## Comparing `papertronics-sdk-0.0.25.tar` & `papertronics-sdk-0.0.26.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.25/LICENSE
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.25/README.md
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/papertronics_sdk/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.25/papertronics_sdk/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/papertronics_sdk/lab/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5986 2023-07-11 10:35:19.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/admin_client.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1571 2023-07-11 10:35:19.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/base_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/papertronics_sdk/lab/exceptions/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/exceptions/StatusException.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/exceptions/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/config.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/database.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/generic.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/models/station_protocol.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9324 2023-07-11 10:35:19.000000 papertronics-sdk-0.0.25/papertronics_sdk/lab/user_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/requires.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:35:27.000000 papertronics-sdk-0.0.25/papertronics_sdk.egg-info/zip-safe
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.25/pyproject.toml
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:35:27.157292 papertronics-sdk-0.0.25/setup.cfg
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.26/LICENSE
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      496 2023-07-11 08:58:02.000000 papertronics-sdk-0.0.26/README.md
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.26/papertronics_sdk/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5836 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/admin_client.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1571 2023-07-11 10:35:19.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/base_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/StatusException.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/exceptions/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/config.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/database.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/generic.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/models/station_protocol.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9144 2023-07-11 10:37:30.000000 papertronics-sdk-0.0.26/papertronics_sdk/lab/user_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      946 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-11 10:37:43.000000 papertronics-sdk-0.0.26/papertronics_sdk.egg-info/zip-safe
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.26/pyproject.toml
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-11 10:37:43.422137 papertronics-sdk-0.0.26/setup.cfg
```

### Comparing `papertronics-sdk-0.0.25/PKG-INFO` & `papertronics-sdk-0.0.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.25
+Version: 0.0.26
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/admin_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,113 +9,113 @@
 
 class AdminLabClient(BaseClient):
 
     def __init__(self, url, token):
         super().__init__(url, token)
 
     def login_user(self, user_id: uuid.UUID) -> str:
-        response = self.post(f"{self.url}/admin/auth/token",
+        response = self.post(f"/admin/auth/token",
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"user_id": user_id})
         return response.json().get("access_token")
 
     def get_users(self, user_id: Optional[uuid.UUID] = None) -> Union[List[UserModel], UserModel]:
         params = {}
         if user_id:
             params["user_id"] = user_id
-        response = self.get(f"{self.url}/admin/user",
+        response = self.get(f"/admin/user",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=params)
         response_dict = response.json()
         if type(response_dict) == list:
             return [UserModel.parse_obj(r) for r in response_dict]
         else:
             return UserModel.parse_obj(response_dict)
 
     def add_user(self, add_user_request: UserRequest) -> UserModel:
-        response = self.post(f"{self.url}/admin/user", json=add_user_request.dict(),
+        response = self.post(f"/admin/user", json=add_user_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return UserModel.parse_obj(response.json())
 
     def delete_user(self, user_id: uuid.UUID):
-        self.delete(f"{self.url}/admin/user",
+        self.delete(f"/admin/user",
                     headers={"Authorization": f"Bearer {self.token}"},
                     params={"user_id": user_id})
 
     def update_user(self, user_id: uuid.UUID, add_user_request: UserRequest) -> UserModel:
-        response = self.post(f"{self.url}/admin/user/update", json=add_user_request.dict(),
+        response = self.post(f"/admin/user/update", json=add_user_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"user_id": user_id})
         return UserModel.parse_obj(response.json())
 
     def get_protocol(self, protocol_id: Optional[uuid.UUID] = None) -> Union[ProtocolModel, List[ProtocolModel]]:
         params = {}
         if protocol_id:
             params["protocol_id"] = protocol_id
-        response = self.get(f"{self.url}/admin/protocol",
+        response = self.get(f"/admin/protocol",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=params)
         response_dict = response.json()
         if type(response_dict) == list:
             return [ProtocolModel.parse_obj(r) for r in response_dict]
         else:
             return ProtocolModel.parse_obj(response_dict)
 
     def link_protocol(self, protocol_id: uuid.UUID, user_id: uuid.UUID) -> ProtocolLinkModel:
-        response = self.post(f"{self.url}/admin/protocol/link",
+        response = self.post(f"/admin/protocol/link",
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"protocol_id": protocol_id, "user_id": user_id})
         return ProtocolLinkModel.parse_obj(response.json())
 
     def remove_link_protocol(self, protocol_link_id: uuid.UUID):
-        self.delete(f"{self.url}/admin/protocol/link",
+        self.delete(f"/admin/protocol/link",
                     headers={"Authorization": f"Bearer {self.token}"},
                     params={"protocol_link_id": protocol_link_id})
 
     def get_devices(self, device_id: Optional[uuid.UUID] = None) -> Union[List[DeviceModel], DeviceModel]:
         params = {}
         if device_id:
             params["device_id"] = device_id
-        response = self.get(f"{self.url}/admin/device",
+        response = self.get(f"/admin/device",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=params)
         response_dict = response.json()
         if type(response_dict) == list:
             return [DeviceModel.parse_obj(r) for r in response_dict]
         else:
             return DeviceModel.parse_obj(response_dict)
 
     def add_device(self, add_device_request: DeviceRequest) -> DeviceModel:
-        response = self.post(f"{self.url}/admin/device", json=add_device_request.dict(),
+        response = self.post(f"/admin/device", json=add_device_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"})
         return DeviceModel.parse_obj(response.json())
 
     def delete_device(self, device_id: uuid.UUID):
-        self.delete(f"{self.url}/admin/device",
+        self.delete(f"/admin/device",
                     headers={"Authorization": f"Bearer {self.token}"},
                     params={"device_id": device_id})
 
     def update_device(self, device_id: uuid.UUID, add_device_request: DeviceRequest) -> DeviceModel:
-        response = self.post(f"{self.url}/admin/device/update", json=add_device_request.dict(),
+        response = self.post(f"/admin/device/update", json=add_device_request.dict(),
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"device_id": device_id})
         return DeviceModel.parse_obj(response.json())
 
     def link_device(self, device_id: uuid.UUID, user_id: uuid.UUID) -> DeviceLinkModel:
-        response = self.post(f"{self.url}/admin/device/link",
+        response = self.post(f"/admin/device/link",
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"device_id": device_id, "user_id": user_id})
         return DeviceLinkModel.parse_obj(response.json())
 
     def remove_link_device(self, device_link_id: uuid.UUID):
-        self.delete(f"{self.url}/admin/device/link",
+        self.delete(f"/admin/device/link",
                     headers={"Authorization": f"Bearer {self.token}"},
                     params={"device_link_id": device_link_id})
 
     def get_device_statistics(self, device_id: Optional[uuid.UUID] = None) -> List[DeviceStatisticModel]:
         params = {}
         if device_id:
             params["device_id"] = device_id
-        response = self.get(f"{self.url}/admin/device/statistic",
+        response = self.get(f"/admin/device/statistic",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=params)
         return [DeviceStatisticModel.parse_obj(r) for r in response.json()]
```

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/base_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.26/papertronics_sdk/lab/user_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,130 +7,130 @@
     ExperimentEditRequest
 from .base_client import BaseClient
 
 
 class UserLabClient(BaseClient):
 
     def authenticate(self, email, password):
-        response = self.post(f"{self.url}/auth/token", data=dict(username=email, password=password))
+        response = self.post(f"/auth/token", data=dict(username=email, password=password))
         self.token = response.json().get("access_token")
         return self.token
 
     def authenticate_device(self, device_id: uuid.UUID):
-        response = self.post(f"{self.url}/auth/device",
+        response = self.post(f"/auth/device",
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"device_id": device_id})
         self.token = response.json().get("access_token")
         return self.token
 
     def download_data(self):
         return "not implemented"
 
     def download_image(self,
                        blob_name: str):
         return "not implemented"
 
     def get_device_info(self) -> DeviceModel:
-        response = self.get(f"{self.url}/device",
+        response = self.get(f"/device",
                             headers={"Authorization": f"Bearer {self.token}"})
         return DeviceModel.parse_obj(response.json())
 
     def get_devices(self) -> List[DeviceModel]:
-        response = self.get(f"{self.url}/device/all",
+        response = self.get(f"/device/all",
                             headers={"Authorization": f"Bearer {self.token}"})
         return [DeviceModel.parse_obj(r) for r in response.json()]
 
     def get_user_info(self) -> UserModel:
-        response = self.get(f"{self.url}/user",
+        response = self.get(f"/user",
                             headers={"Authorization": f"Bearer {self.token}"})
         return UserModel.parse_obj(response.json())
 
     def store_protocol(self, protocol_request: SaveProtocolRequest) -> ProtocolModel:
-        response = self.post(f"{self.url}/protocol",
+        response = self.post(f"/protocol",
                              headers={"Authorization": f"Bearer {self.token}"},
                              json=protocol_request.dict())
         return ProtocolModel.parse_obj(response.json())
 
     def build_protocol(self,
                        protocol_request: SaveProtocolRequest,
                        duration: int,
                        interval: int,
                        flash: bool = True,
                        start_delay: int = 0) -> ProtocolModel:
         response = self.post(
-            f"{self.url}/protocol/build",
+            f"/protocol/build",
             headers={"Authorization": f"Bearer {self.token}"},
             json=protocol_request.dict(),
             params={"duration": duration, "interval": interval, "flash": flash, "start_delay": start_delay})
         return ProtocolModel.parse_obj(response.json())
 
     def get_protocol(self,
                      protocol_id: Optional[uuid.UUID] = None,
                      protocol_test_type: Optional[str] = None,
                      page_size: Optional[int] = None,
                      page: Optional[int] = None,
                      valid: Optional[bool] = True) -> Union[ProtocolModel, List[ProtocolModel]]:
-        response = self.get(f"{self.url}/protocol",
+        response = self.get(f"/protocol",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=dict(protocol_id=protocol_id,
                                         protocol_test_type=protocol_test_type,
                                         page_size=page_size,
                                         page=page,
                                         valid=valid))
         if type(response.json()) == list:
             return [ProtocolModel.parse_obj(r) for r in response.json()]
         else:
             return ProtocolModel.parse_obj(response.json())
 
     def count_protocol(self,
                        protocol_test_type: Optional[str] = None,
                        valid: Optional[bool] = True) -> int:
-        response = self.get(f"{self.url}/protocol/count",
+        response = self.get(f"/protocol/count",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=dict(protocol_test_type=protocol_test_type,
                                         valid=valid))
         return int(response.text)
 
     def get_protocol_test_def(self, protocol_id: uuid.UUID) -> Union[ProtocolTestResponse, str]:
-        response = self.get(f"{self.url}/protocol/test",
+        response = self.get(f"/protocol/test",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params={"protocol_id": protocol_id})
         if type(response.json()) == str:
             return response.json()
         else:
             return ProtocolTestResponse.parse_obj(response.json())
 
     def invalidate_protocol(self, protocol_id: uuid.UUID) -> ProtocolModel:
-        response = self.delete(f"{self.url}/protocol",
+        response = self.delete(f"/protocol",
                                headers={"Authorization": f"Bearer {self.token}"},
                                params={"protocol_id": protocol_id})
         return ProtocolModel.parse_obj(response.json())
 
     def start_experiment(self, request: ExperimentStartRequest) -> ExperimentModel:
-        response = self.post(f"{self.url}/experiment/start",
+        response = self.post(f"/experiment/start",
                              headers={"Authorization": f"Bearer {self.token}"},
                              json=request.dict())
         return ExperimentModel.parse_obj(response.json())
 
     def cancel_experiment(self,
                           experiment_id: uuid.UUID):
-        self.post(f"{self.url}/experiment/cancel",
+        self.post(f"/experiment/cancel",
                   headers={"Authorization": f"Bearer {self.token}"},
                   json=dict(experiment_id=experiment_id))
 
     def get_experiments(self,
                         experiment_id: Optional[List[uuid.UUID]] = None,
                         device_id: Optional[uuid.UUID] = None,
                         order_by: str = "start_time",
                         ascending_order: bool = False,
                         page_size: Optional[int] = None,
                         page: Optional[int] = None,
                         valid: Optional[bool] = None,
                         first=True) -> Union[List[ExperimentModel], ExperimentModel]:
-        response = self.get(f"{self.url}/experiment",
+        response = self.get(f"/experiment",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=dict(experiment_id=experiment_id,
                                         device_id=device_id,
                                         order_by=order_by,
                                         ascending_order=ascending_order,
                                         page_size=page_size,
                                         page=page,
@@ -139,37 +139,37 @@
             return ExperimentModel.parse_obj(response.json()[0])
         else:
             return [ExperimentModel.parse_obj(r) for r in response.json()]
 
     def count_experiments(self,
                           valid: Optional[bool] = None,
                           device_id: Optional[uuid.UUID] = None) -> int:
-        response = self.get(f"{self.url}/experiment/count",
+        response = self.get(f"/experiment/count",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=dict(device_id=device_id,
                                         valid=valid))
         return int(response.text)
 
     def edit_experiment_by_id(self,
                               experiment_id: uuid.UUID,
                               experiment_edit_request: ExperimentEditRequest):
-        response = self.post(f"{self.url}/experiment/edit",
+        response = self.post(f"/experiment/edit",
                              headers={"Authorization": f"Bearer {self.token}"},
                              json=experiment_edit_request.dict(),
                              params={"experiment_id": experiment_id})
         return ExperimentModel.parse_obj(response.json())
 
     def delete_experiment_by_id(self,
                                 experiment_id: uuid.UUID):
-        self.delete(f"{self.url}/experiment",
+        self.delete(f"/experiment",
                     headers={"Authorization": f"Bearer {self.token}"},
                     params={"experiment_id": experiment_id})
 
     def perform_experiment(self, request: ExperimentStartRequest, timeout=120):
-        response = self.post(f"{self.url}/experiment/start",
+        response = self.post(f"/experiment/start",
                              headers={"Authorization": f"Bearer {self.token}"},
                              json=request.dict())
         experiment = ExperimentModel.parse_obj(response.json())
 
         sleep_counter = 0
         images_captured = 0
```

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.26/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.25
+Version: 0.0.26
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.25/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.26/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.25/setup.cfg` & `papertronics-sdk-0.0.26/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.25
+version = 0.0.26
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

